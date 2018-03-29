---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-21"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Planung für SSL

Für die ersten Schritte bei der Verwendung von SSL-Zertifikaten ist eine gewisse Planung erforderlich. Schaffen Sie dazu folgende Voraussetzungen.

1. Entscheiden, wo das Zertifikat abgerufen werden soll
2. Informationen zu Zertifikatstypen, Schlüssellänge und Gültigkeitsdauer
3. Allgemeinen Namen auswählen
4. Informationen zur Socketregel
5. Zertifikatssignieranforderung generieren

## Entscheiden, wo das Zertifikat abgerufen werden soll

SSL-Zertifikate können Sie intern in Ihrer Organisation oder von einer Zertifizierungsstelle, wie Verisign, RapidSSL, Thawte und anderen, erhalten.  

Für eine kleine Gruppe in einer gesteuerten Architektur, wie Mitarbeiter, die eine Intranet-Site verwenden, können Sie ein selbstsigniertes Zertifikat anfordern, das jeder Mitarbeiter für seinen Browser installiert. Sie können auch selbst eine lokale Zertifizierungsstelle einrichten, um Zertifikate für die Verwendung in Ihrer Organisation zu generieren.

Bei einer größeren und vielfältigeren Gruppe ist bei der Verwendung eines SSL-Zertifikats von einer Standardquelle ein Zugriff ohne eine spezielle Konfiguration möglich. Moderne Web-Browser sind so konfiguriert, dass SSL-Zertifikaten, die von einer Zertifizierungsstelle ausgestellt wurden, vertraut wird.

## Informationen zu Zertifikatstypen, Schlüssellänge und Gültigkeitsdauer

Nachdem Sie sich entschieden haben, woher Sie Ihr Zertifikat beziehen, überprüfen Sie die folgenden Optionen zu Zertifikatstypen und deren entsprechende Verfügbarkeit, Schlüssellänge und Gültigkeitsdauer.

|              Zertifikatstypen          |  Verfügbarkeit                     |  Schlüssellänge                |  Gültigkeitsdauer                  |
| --------------------------------------- | --------------------------------- | -------------------------- | -------------------------- |
|Domain-Validation (DV)                   | Schnell verfügbar                 | 1024 Bit oder 2048 Bit       | 1 oder 2 Jahr(e)             |
|Organization-Validation (OV)             | 2-3 Tage oder bis zu einer Woche          | 1024 Bit oder 2048 Bit       | 1 oder 2 Jahr(e)             |
|Extended-Validation (EV)                 | 2-3 Tage oder bis zu einer Woche          | Nur 2048 Bit              | 1 oder 2 Jahr(e)             |
{: caption="Tabelle 1. Zertifikatstypen" caption-side="top"}   


## Allgemeinen Namen auswählen

Der im Zertifikat verwendete allgemeine Name ist der Hostname für die Website. Der Hostname und der allgemeine Name des Zertifikats müssen übereinstimmen, da der Browser ansonsten eine Warnung ausgibt. Wenn Ihre Site 'web1.mydomain.com' ist, verwenden Sie diese als den allgemeinen Namen. Bei zusätzlicher Verwendung von 'images.mydomain.com' benötigen Sie entweder ein Platzhalterzertifikat (das nicht über {{site.data.keyword.cloud}} verfügbar ist) oder müssen mehrere Zertifikate einrichten. Wenn Sie den falschen allgemeinen Namen auswählen, können Sie mit bestimmten Schritten eine Zertifikatsfolge korrigieren und das Zertifikat widerrufen und mit dem richtigen allgemeinen Namen erneut ausgeben.  

## Informationen zur Socketregel

Es darf nur ein Zertifikat pro Socket verwendet werden. Ein Socket ist eine IP-Adresse und eine Portkombination, beispielsweise '1.2.3.4:443'. '1.2.3.4:444' wäre ein anderes Socket. Für Anwendungen wie SMTP/POP3 oder FTP spielt dies keine Rolle. Für HTTP hingegen ist dies jedoch wegen der Einbindung beim virtuellen Hosting wichtig.

Virtuelles Hosting ist eine Methode, mit der bis zu 100 Websites auf einer IP-Adresse gehostet werden können. Dies geht, da moderne Browser ein Feld des Typs 'host reader' als Teil ihrer Anforderung übergeben. Das Feld, das die Syntax 'Host: web1.mydomain.com' aufweist, zeigt dem Web-Server an, auf welche Site zugegriffen werden soll. Im Fall von HTTPS (HTTP over SSL) muss der Web-Server das SSL-Zertifikat auswählen, das an den Client gesendet werden soll, bevor er den Host-Header sieht. Dies ist der Grund, warum ein Socket nur ein Zertifikat haben kann.

Sie können jede SSL-fähige Website einem eigenen Socket zuweisen. Dies ist möglich, indem Sie die IP-Adresse oder den Port abändern. Wenn Sie den Port von 443/tcp ändern, beachten Sie, dass Benutzer die Portnummer in die URL einschließen müssen. Beispiel: https://web1.mydomain.com:444.

## Zertifikatssignieranforderung generieren

Sie können die Zertifikatssignieranforderung mithilfe einer bestimmten Software auf dem Web-Server generieren. Verwenden Sie für UNIX-Systeme das OpenSSL-Paket. Unter Windows gibt es einen Assistenten, auf den Sie über die Registerkarte zur Verzeichnissicherheit der Websiteeigenschaften in IIS Manager zugreifen können. Wenn Sie die Systemsteuerung verwenden, sind die durchzuführenden Schritte je nach Betriebssystem etwas anders.

Beim Generieren der Zertifikatssignieranforderung wird ein privater Schlüssel erstellt. Verlieren, löschen oder teilen Sie diesen privaten Schlüssel nicht. Er muss als vertraulich auf dem Web-Server gespeichert werden. Mit einigen Dienstprogrammen zur Generierung der Zertifikatssignieranforderung können Sie auch eine Kennphrase für den privaten Schlüssel erstellen. Nutzen Sie diese Möglichkeit nur dann, wenn Sie sich jedes Mal beim Neustart der Web-Server-Software wieder beim Server anmelden möchten.  Wenden Sie außerdem keine Sicherheitsabfrage auf die Zertifikatssignieranforderung an.

