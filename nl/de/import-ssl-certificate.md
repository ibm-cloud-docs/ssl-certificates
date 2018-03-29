---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL-Zertifikate importieren

Nachdem ein SSL-Zertifikat für eine Website ausgestellt wurde, kann es in das {{site.data.keyword.slportal_full}} importiert werden. Durch den Import von SSL-Zertifikaten in das {{site.data.keyword.slportal}} können diese Zertifikate auf Produkte und Services angewendet werden, für die solche Zertifikate erforderlich sind, beispielsweise die [SSL-Auslagerung](/docs/infrastructure/local-load-balancer/configure-ssl-offloading-load-balancer.html){:new_window} der Lastausgleichsfunktion. Standardmäßig werden von {{site.data.keyword.BluSoftlayer_full}} ausgestellte SSL-Zertifikate nicht in die Liste importiert, da sie nur vom Empfänger selbst bearbeitet werden sollen. Daher müssen SSL-Zertifikate, die mit einem {{site.data.keyword.BluSoftlayer_notm}}-Produkt oder -Service verwendet werden sollen, manuell durch einen berechtigten Benutzer für das Konto importiert werden. Führen Sie die nachfolgenden Schritte aus, um ein SSL-Zertifikat in das {{site.data.keyword.slportal}} zu importieren.

## SSL-Zertifikate importieren

1. Greifen Sie mit Ihren eindeutigen Berechtigungsnachweisen auf das [{{site.data.keyword.slportal_full}} ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/){: new_window} zu.
2. Wählen Sie im Menü **Sicherheit** die Option **SSL > Zertifikate** aus.
3. Klicken Sie oben in der Anzeige auf den Link **SSL-Zertifikat importieren**.
4. Geben Sie die **SSL-Zertifikatsdetails** in die entsprechenden Felder ein und klicken Sie auf **Importieren**.

   **Hinweis:** Im Fenster **SSL-Zertifikat importieren** angegebene Details müssen genauso eingegeben werden, wie sie von der Zertifizierungsstelle bereitgestellt werden, einschließlich von Leerzeichen und Zeilenbrüchen. Werden die Details nicht korrekt eingegeben, tritt ein Fehler auf.

| Textfeld | Eingabe |
| -------- | ----- |
|Zertifikat |Von der Zertifizierungsstelle bereitgestellte SSL-Zertifikatsdetails. Hierbei handelt es sich für gewöhnlich um einen alphanumerischen Textblock.|
|Privater Schlüssel | Von der Zertifizierungsstelle bereitgestellte Details des privaten Schlüssels für das Zertifikat. Hierbei handelt es sich für gewöhnlich um einen alphanumerischen Textblock.|
|Zwischenzertifikat | Von der Zertifizierungsstelle bereitgestellte Details des Zwischenzertifikats. Zwischenzertifikate sind zwar nicht erforderlich, wenn jedoch die Informationen für das SSL-Zertifikat verfügbar sind, sollten diese eingegeben werden.|
| Zertifikatssignieranforderung | Von der Zertifizierungsstelle bereitgestellte Details der Zertifikatssignieranforderung. Diese Details sind zwar nicht erforderlich, sollten aber bereitgestellt werden, falls sie Teil des Zertifikats sind. **Hinweis:** Die Zertifikatssignieranforderung darf nicht geändert werden. Sie kann einen öffentlichen Schlüssel enthalten, der nicht durch den privaten Schlüssel ersetzt werden darf.|
|Anmerkungen | Anmerkungen in Bezug auf das SSL-Zertifikat, die für andere Benutzer hilfreich sein können.


## Nächste Schritte

Nachdem das SSL-Zertifikat in das {{site.data.keyword.slportal}} importiert wurde, wird es so lange in der Anzeige mit den SSL-Zertifikaten gespeichert, bis es [manuell gelöscht](delete-ssl-certificate.html) wird. Für alle Produkte und Services, für die SSL-Zertifikatsdetails erforderlich sind, wird das neue SSL-Zertifikat bei der Interaktion mit dem SSL-Feature für das gewünschte Produkt oder den gewünschten Service in der Liste der verfügbaren Zertifikate angezeigt. Das Zertifikat kann jederzeit [aktualisiert](view-and-update-ssl-certificate.html) und Details zum Zertifikat [sicher heruntergeladen](download-ssl-certificate-details.html) werden.
