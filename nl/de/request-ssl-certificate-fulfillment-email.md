---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificate fulfillment email, fulfillment email

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Auftragserfüllungs-E-Mail für SSL-Zertifikat anfordern
{: #requesting-an-ssl-certificate-fulfillment-email}

Nach dem Bestellen eines neuen SSL-Zertifikats über {{site.data.keyword.cloud}} sendet die Zertifizierungsstelle eine Auftragserfüllungs-E-Mail an den während des Bestellprozesses angegebenen Domänenadministrator. Diese E-Mail enthält alles Details zu dem SSL-Zertifikat. Die Auftragserfüllungs-E-Mail kann jederzeit erneut über die Anzeige für SSL-Bestellungen in der {{site.data.keyword.cloud_notm}}-Konsole angefordert werden.
{:shortdesc}

## Auftragserfüllungs-E-Mail anfordern
Führen Sie die nachfolgenden Schritte aus, um die SSL-Auftragserfüllungs-E-Mail von der Zertifizierungsstelle anzufordern.

1. Navigieren Sie zum Sicherheitsmenü Ihrer Konsole. Weitere Informationen finden Sie unter [Zu Einheiten navigieren](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. Wählen Sie im Menü **Sicherheit** die Option **SSL > Bestellungen** aus.
3. Klicken Sie auf **Senden** in der Spalte **E-Mail** für das gewünschte SSL-Zertifikat.

  Es wird ein Popup-Fenster für die Bestätigung der Anforderung angezeigt. Dieses Fenster enthält die E-Mail-Adresse für den Domänenadministrator, die beim Anfordern des SSL-Zertifikats angegeben wurde.{:note}

4. Klicken Sie auf **E-Mail erneut senden**, um die Auswahl zu bestätigen und eine zusätzliche Auftragserfüllungs-E-Mail von der Zertifizierungsstelle anzufordern.

## Nächste Schritte

Nach dem Anfordern einer zusätzlichen Auftragserfüllungs-E-Mail wird die Anforderung zum Abschließen an die entsprechende Zertifizierungsstelle gesendet. Da die Details eines SSL-Zertifikats vertraulich sind, speichert {{site.data.keyword.cloud_notm}} die Daten des SSL-Zertifikats nicht in seinem System. Nach dem Erhalt der SSL-Zertifikatsdetails per E-Mail können diese bei Bedarf manuell in die {{site.data.keyword.cloud_notm}}-Konsole [importiert](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates) werden.
