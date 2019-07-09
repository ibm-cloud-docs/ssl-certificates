---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-11"

keywords: types of certificates,SSL certificates, Select Security

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Lernprogramm 'Einführung'
{: #getting-started-tutorial}

## Vorbereitung

Für die ersten Schritte bei der Verwendung von SSL-Zertifikaten ist eine gewisse Planung erforderlich. Schaffen Sie dazu folgende Voraussetzungen.

1. Überlegen Sie, wo Sie das Zertifikat abrufen möchten.
2. Machen Sie sich mit Zertifikatstypen, Schlüssellänge und Gültigkeitsdauer von Zertifikaten vertraut.
3. Wählen Sie einen allgemeinen Namen aus.
4. Machen Sie sich mit der Socketregel vertraut.
5. Generieren Sie die Zertifikatssignieranforderung.

Weitere Informationen finden Sie in [Planung für SSL-Zertifikate](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-planning-for-ssl#planning-for-ssl).

## SSL-Zertifikate bestellen

1. Navigieren Sie zum Sicherheitsmenü Ihrer Konsole. Weitere Informationen finden Sie unter [Zu Einheiten navigieren](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. Wählen Sie im Menü **Sicherheit** die Optionen **Sicherheit > SSL > Zertifikate** aus.
3. Wählen Sie **SSL-Zertifikat bestellen** aus.
3. Wählen Sie den Typ und die Gültigkeitsdauer des Zertifikats aus, schicken Sie den Text der Zertifikatssignieranforderung ab, wählen Sie Ihre Serverplattform aus und bestätigen Sie dann die Zahlung.

## Installation und Test
Nachdem der Bestell- und Validierungsprozess abgeschlossen ist, erhalten Sie von der Zertifizierungsstelle eine E-Mail mit Ihrem Zertifikat und bei Bedarf allen erforderlichen Zwischenzertifikaten. Die Installationsmethode ist zwar von der von Ihnen verwendeten Software abhängig, das Ergebnis sollte aber in allen Fällen gleich sein. Wenn Sie den Vorgang abgeschlossen haben, sollten Sie `http://host.yourdomain.com` aufrufen und Ihre Inhalte sowie das SSL-Schloss sehen können, mit dem in Browsern eine verschlüsselte Sitzung angezeigt wird. Wird eine Warnung angezeigt, gibt es bestimmte Schritte, die Sie ausführen müssen.

## Nächste Schritte

Nach einem erfolgreichen Test können Sie auf Ihre SSL-Zertifikate in der {{site.data.keyword.cloud_notm}}-Konsole zugreifen, um vorhandene SSL-Zertifikate zu [aktualisieren](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates#viewing-and-updating-ssl-certificates), [herunterzuladen](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details#downloading-ssl-certificate-details), zu [löschen](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates) oder in das Tool zu [importieren](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates).
