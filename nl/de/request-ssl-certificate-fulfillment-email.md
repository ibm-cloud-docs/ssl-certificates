---

copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"

keywords: SSL certificate fulfillment email, fulfillment email

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Auftragserfüllungs-E-Mail für SSL-Zertifikat anfordern
{: #requesting-an-ssl-certificate-fulfillment-email}

Nach dem Bestellen eines neuen SSL-Zertifikats über {{site.data.keyword.BluSoftlayer_full}} sendet die Zertifizierungsstelle eine Auftragserfüllungs-E-Mail an den während des Bestellprozesses angegebenen Domänenadministrator. Diese E-Mail enthält alles Details zu dem SSL-Zertifikat. Die Auftragsbetätigungs-E-Mail kann jederzeit erneut über die Anzeige mit den SSL-Bestellungen im {{site.data.keyword.slportal_full}} angefordert werden. Führen Sie die nachfolgenden Schritte aus, um die SSL-Auftragserfüllungs-E-Mail von der Zertifizierungsstelle anzufordern.

## Auftragserfüllungs-E-Mail anfordern

1. Greifen Sie mit Ihren eindeutigen Berechtigungsnachweisen auf das [{{site.data.keyword.slportal_full}} ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/){: new_window} zu.
2. Wählen Sie im Menü **Sicherheit** die Option **SSL > Bestellungen** aus.
3. Klicken Sie in der Spalte **E-Mail** des gewünschten SSL-Zertifikats auf den Link zum **Senden**.<br/>**Hinweis:** Es wird ein Popup-Fenster angezeigt, in dem Sie die Anforderung bestätigen können. Dieses Fenster enthält die E-Mail-Adresse für den Domänenadministrator, der beim Anfordern des SSL-Zertifikats angegeben wurde.
4. Klicken Sie auf **E-Mail erneut senden**, um die Auswahl zu bestätigen und eine zusätzliche Auftragserfüllungs-E-Mail von der Zertifizierungsstelle anzufordern.  Sie können auch auf **Abbrechen** klicken, um die Aktion abzubrechen.

## Nächste Schritte

Nach dem Anfordern einer zusätzlichen Auftragserfüllungs-E-Mail wird die Anforderung zum Abschließen an die entsprechende Zertifizierungsstelle gesendet. Da die Details eines SSL-Zertifikats vertraulich sind, speichert {{site.data.keyword.BluSoftlayer_notm}} die Daten des SSL-Zertifikats nicht in seinem System. Nach dem Erhalt der SSL-Zertifikatsdetails per E-Mail können diese bei Bedarf manuell in das {{site.data.keyword.slportal}} [importiert](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates) werden.
