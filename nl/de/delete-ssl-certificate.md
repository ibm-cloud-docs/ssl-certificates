---

copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"

keywords: SSL certificates delete, SSL delete

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL-Zertifikate löschen
{: #deleting-ssl-certificates}

Nachdem die Details eines SSL-Zertifikats in das {{site.data.keyword.slportal_full}} importiert wurden, kann es jederzeit gelöscht werden, um alle gespeicherten Daten aus dem {{site.data.keyword.slportal}} zu entfernen.

Führen Sie die nachfolgenden Schritte aus, um ein SSL-Zertifikat zu löschen.

1. Greifen Sie mit Ihren eindeutigen Berechtigungsnachweisen auf das [{{site.data.keyword.slportal}} ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/){: new_window} zu.
2. Wählen Sie im Menü **Sicherheit** die Option **SSL > Zertifikate** aus.
3. Wählen Sie aus dem Menü **Aktionen** für das gewünschte SSL-Zertifikat die Option **Löschen** aus.

  **Hinweis:** Es wird ein Fenster angezeigt, in dem Sie den Löschvorgang bestätigen können.
4. Klicken Sie auf **Ja**, um das SSL-Zertifikat zu löschen, oder auf **Nein**, um die Aktion abzubrechen.

## Nächste Schritte

Nach dem Löschen des SSL-Zertifikats können alle Services, die mit diesem Zertifikat verknüpft sind, die entsprechenden Informationen nicht länger verwenden. Das Zertifikat wird nicht mehr in der Anzeige mit den SSL-Zertifikaten im {{site.data.keyword.slportal}} angezeigt.

Es wird empfohlen, alle Services, die das gelöschte Zertifikat bisher verwendet haben, einem gültigen SSL-Zertifikat zuzuordnen, das dem Konto zugewiesen ist.

**Hinweis:** Das SSL-Zertifikat kann jederzeit mithilfe des [Importprozesses](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates) wieder zum {{site.data.keyword.slportal}} hinzugefügt werden.
