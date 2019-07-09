---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificates delete, SSL delete

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL-Zertifikate löschen
{: #deleting-ssl-certificates}

Nachdem die Details eines SSL-Zertifikats in die {{site.data.keyword.cloud}}-Konsole importiert wurden, kann es jederzeit gelöscht werden, um alle gespeicherten Daten aus der {{site.data.keyword.cloud_notm}}-Konsole zu entfernen.

Führen Sie die nachfolgenden Schritte aus, um ein SSL-Zertifikat zu löschen.

1. Navigieren Sie zum Sicherheitsmenü Ihrer Konsole. Weitere Informationen finden Sie unter [Zu Einheiten navigieren](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. Wählen Sie im Menü **Sicherheit** die Option **SSL > Zertifikate** aus.
3. Wählen Sie aus dem Menü **Aktionen** für das gewünschte SSL-Zertifikat die Option **Löschen** aus.
4. Klicken Sie auf **Ja**, um das SSL-Zertifikat zu löschen.

## Nächste Schritte

Nach dem Löschen des SSL-Zertifikats können alle Services, die mit diesem Zertifikat verknüpft sind, die entsprechenden Informationen nicht länger verwenden. Das Zertifikat wird nicht mehr in der Anzeige für SSL-Zertifikate in der {{site.data.keyword.cloud_notm}}-Konsole angezeigt.

Aktualisieren Sie alle Services, die das gelöschte Zertifikat bisher verwendet haben, um sie einem gültigen SSL-Zertifikat zuzuordnen, das dem Konto zugewiesen ist.

Das SSL-Zertifikat kann der {{site.data.keyword.cloud_notm}}-Konsole jederzeit mithilfe des [Importprozesses](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates) wieder hinzugefügt werden.
{:note}
