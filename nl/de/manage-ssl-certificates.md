---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: management of certificates, add certificate, managing certificates

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL-Zertifikate verwalten
{: #managing-ssl-certificates}

Sie können Ihre SSL-Zertifikate in der {{site.data.keyword.cloud}}-Konsole verwalten. Dieses kann nicht nur als Repository für die Verwaltung der Zertifikate dienen, sondern ist auch bei der Nutzung von Services und beim Anfordern von Zertifikaten erforderlich.

1. Navigieren Sie zum Sicherheitsmenü Ihrer Konsole. Weitere Informationen finden Sie unter [Zu Einheiten navigieren](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. Wählen Sie aus dem Menü **Sicherheit** die Option **SSL > Zertifikate > Zertifikate verwenden** aus.


Es werden eine Liste der aktuellen Zertifikate sowie entsprechende Statusinformationen angezeigt.

Sie können ein Zertifikat durchsuchen, Teile oder eine PEM-formatierte Version des Zertifikats herunterladen oder das Ablaufdatum für die Zertifikate überprüfen. Außerdem können Sie sehen, wie viele Services die einzelnen Zertifikate momentan verwenden. Dies zeigt Ihnen, ob Maßnahmen ergriffen werden müssen, wenn ein Zertifikat fast abgelaufen ist.

## Zertifikat hinzufügen

Wenn Sie ein Zertifikat hinzufügen möchten, wählen Sie im Navigationsuntermenü oder im Zertifikatslistentitel **Zertifikat hinzufügen** aus. Sie müssen nur das Zertifikat und den entsprechenden privaten Schlüssel angeben. Wenn Ihr Aussteller ein Zwischenzertifikat bereitstellt und Sie dieses nicht angeben, kann dies jedoch zu einer unterbrochenen Zertifikatskette und fehlerhaften Validierung für Benutzer oder zugehörige Services führen.

Private Schlüssel, für die eine Kennphrase erforderlich ist, können nicht gespeichert werden.
{:note}

Sobald sie hinzugefügt wurden, werden die folgenden Felder direkt aus den Zertifikaten abgeleitet:

* Allgemeiner Name
* Organisationsname
* Gültigkeitszeitraum

## Zertifikat bearbeiten

Durch das Aktivieren des Dreiecks links neben einem Zertifikat werden die Bestandteile des Zertifikats in ihrer Gesamtheit sichtbar gemacht. Außerdem können dann die Bestandteile bearbeitet werden. Es kann außerdem eine Anmerkung hinzugefügt werden und bei Bedarf kann das Zertifikat entfernt werden. Zudem wird eine Liste der Services angezeigt, die das Zertifikat momentan verwenden.

Der private Schlüssel, das Zertifikat oder das Zwischenzertifikat als Bestandteile von Zertifikaten können nur für Zertifikate aktualisiert werden, die keinem Service zugeordnet sind. Darüber hinaus kann das Zertifikat nicht entfernt werden. Sie können die Anmerkung jederzeit ändern.

## Zertifikat entfernen

Um ein Zertifikat zu entfernen, befolgen Sie die Schritte zum Bearbeiten des Zertifikats, wählen Sie "Bestätigen der Zertifikatsentfernung" aus und speichern Sie die Änderung.

## API verwenden

Ein Beispiel für die Bearbeitung von Zertifikaten mithilfe der API finden Sie in [SSL-Verwaltung ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](http://sldn.softlayer.com/article/ssl-management){: new_window}.
