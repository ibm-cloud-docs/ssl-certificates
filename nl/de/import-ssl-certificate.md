---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: importing SSL certificates,SSL import, SSL certificate details

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL-Zertifikate importieren
{: #importing-ssl-certificates}

Nachdem ein SSL-Zertifikat für eine Website ausgestellt wurde, kann es in die {{site.data.keyword.cloud}}-Konsole importiert werden. Durch den Import von SSL-Zertifikaten in die {{site.data.keyword.cloud_notm}}-Konsole können die Zertifikate auf Produkte und Services angewendet werden, für die sie möglicherweise erforderlich sind, beispielsweise die [SSL-Auslagerung](/docs/infrastructure/local-load-balancer?topic=local-load-balancer-configuring-ssl-offloading-on-a-load-balancer) der Lastausgleichsfunktion. Standardmäßig werden von {{site.data.keyword.cloud_notm}} ausgestellte SSL-Zertifikate nicht in die Liste importiert, da sie nur vom Empfänger selbst bearbeitet werden sollen. Daher müssen SSL-Zertifikate, die mit einem {{site.data.keyword.cloud_notm}}-Produkt oder -Service verwendet werden, manuell durch einen berechtigten Benutzer für das Konto importiert werden.
{:shortdesc}

## SSL-Zertifikate importieren

Führen Sie die nachfolgenden Schritte aus, um ein SSL-Zertifikat zu importieren.

1. Navigieren Sie zum Sicherheitsmenü Ihrer Konsole. Weitere Informationen finden Sie unter [Zu Einheiten navigieren](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. Wählen Sie im Menü **Sicherheit** die Option **SSL > Zertifikate** aus.
3. Klicken Sie auf **SSL-Zertifikat importieren**.
4. Geben Sie die **SSL-Zertifikatsdetails** in die entsprechenden Felder ein und klicken Sie auf **Importieren.** Weitere Informationen finden Sie in der folgenden Tabelle.

   Im Fenster **SSL-Zertifikat importieren** angegebene Details müssen genauso eingegeben werden, wie sie von der Zertifizierungsstelle bereitgestellt werden, einschließlich Leerstellen und Zeilenumbrüche. Werden die Details nicht korrekt eingegeben, tritt ein Fehler auf.
   {:note}

| SSL-Zertifikatsdetails     | Beschreibung |
| --------------------------- | ----------- |
|Zertifikat                  | Von der Zertifizierungsstelle bereitgestellte SSL-Zertifikatsdetails. Hierbei handelt es sich für gewöhnlich um einen alphanumerischen Textblock.|
|Privater Schlüssel                  | Von der Zertifizierungsstelle bereitgestellte Details des privaten Schlüssels für das Zertifikat. Hierbei handelt es sich für gewöhnlich um einen alphanumerischen Textblock.|
|Zwischenzertifikat     | Von der Zertifizierungsstelle bereitgestellte Details des Zwischenzertifikats. Zwischenzertifikate sind zwar nicht erforderlich, wenn jedoch die Informationen für das SSL-Zertifikat verfügbar sind, sollten sie eingegeben werden.|
|Zertifikatssignieranforderung| Von der Zertifizierungsstelle bereitgestellte Details der Zertifikatssignieranforderung. Diese Details sind zwar nicht erforderlich, sollten aber bereitgestellt werden, falls sie Teil des Zertifikats sind. **Hinweis:** Die Zertifikatssignieranforderung darf nicht geändert werden. Sie kann einen öffentlichen Schlüssel enthalten, der nicht durch den privaten Schlüssel ersetzt werden darf.|
|Anmerkungen                        | Anmerkungen in Bezug auf das SSL-Zertifikat, die für andere Benutzer hilfreich sein können.|
{: caption="Tabelle 1. Details des SSL-Zertifikats" caption-side="top"}

## Nächste Schritte

Nachdem das SSL-Zertifikat in die {{site.data.keyword.cloud_notm}}-Konsole importiert wurde, wird es so lange in der Anzeige für SSL-Zertifikate gespeichert, bis es [manuell gelöscht](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates) wird. Für alle Produkte und Services, für die SSL-Zertifikatsdetails erforderlich sind, wird das neue SSL-Zertifikat bei der Interaktion mit dem SSL-Feature für das gewünschte Produkt oder den gewünschten Service in der Liste der verfügbaren Zertifikate angezeigt. Das Zertifikat kann jederzeit [aktualisiert](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates) und Details zum Zertifikat [sicher heruntergeladen](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details) werden.
