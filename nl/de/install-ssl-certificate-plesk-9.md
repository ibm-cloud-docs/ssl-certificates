---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL-Zertifikate in Plesk 9 installieren

Führen Sie die folgenden Schritte aus, um SSL-Zertifikate in Plesk 9 hinzuzufügen.

1. Melden Sie sich bei Plesk an und navigieren Sie zu der Domäne, in der Sie das Zertifikat installieren möchten.
2. Bearbeiten Sie die Konfiguration der Zieldomäne.
3. Klicken Sie auf **SSL-Zertifikate**.
4. Klicken Sie auf **SSL-Zertifikate hinzufügen**.

   **Hinweis:** Wenn Sie bereits über ein SSL-Zertifikat verfügen, überspringen Sie diesen Schritt und fahren Sie mit Schritt 8 fort.
5.  Geben Sie dem Zertifikat einen Namen. Sie können einen beliebigen Namen wählen, es ist jedoch hilfreich, wenn Sie einen beschreibenden Namen mit Zeitmarke verwenden.

   Im vorliegenden Fall wird das Format *JJJJMMTTRR* verwendet, wobei *RR* die Revisionsnummer (00 in diesem Fall, da es für denselben Tag keine Revisionen gibt) ist.
6. Nehmen Sie alle erforderlichen Änderungen an der SSL-Anforderung vor. Diese Informationen werden in das SSL-Zertifikat eingebettet und sollten den Informationen zur Domänenregistrierung ähneln.

  Die E-Mail-Adresse sollte einer der E-Mail-Adressen in der Domäne entsprechen, deren Informationen durch den Registrator der Domäne bereitgestellt wurden.

  **Wichtig:** Falsche Informationen können von Ihrer SSL-Zertifizierungsstelle abgelehnt werden.
7. Navigieren Sie zurück zur Zertifikatskonfiguration.
8. Überprüfen Sie die Zertifikatssignieranforderung und den privaten Schlüssel und speichern Sie den privaten Schlüssel an einer sicheren Position.  

  **Hinweis:** Sollte etwas mit Ihrem Server sein, das dazu führt, dass das Zertifikat erneut eingegeben werden muss, müssen Sie als Mindestanforderung über das Zertifikat und den privaten Schlüssel verfügen.
9. Nehmen Sie die Zertifikatssignieranforderung und übergeben Sie sie an die Zertifizierungsstelle Ihrer Wahl. Im Rahmen von {{site.data.keyword.cloud_notm}} Infrastructure werden keine SSL-Zertifikate bereitgestellt.
10. Nachdem Sie das Zertifikat von der Zertifizierungsstelle erhalten haben, können Sie es in den Textbereich für Zertifikate einfügen.

   **Hinweise:**
   * Wenn es von Ihrer Zertifizierungsstelle verlangt wird, müssen Sie ein eigenes Zertifikat in den Textbereich für die Zertifizierungsstelle (oft auch als CA-Bundle bezeichnet) einfügen.
   * Sie müssen über einen privaten Schlüssel und ein entsprechendes Zertifikat verfügen, um ein Zertifikat verwenden zu können.
11. Navigieren Sie von der Domänenkonfiguration zurück zu den *<span style="text-decoration: underline">Einstellungen für das Web-Hosting</span>*.
12. Wählen Sie das entsprechende Zertifikat aus und klicken Sie auf **OK**.

Das neue Zertifikat wird jetzt für die Domäne verwendet. Wenn Sie das Zertifikat aktualisiert haben, müssen Sie möglicherweise den Browser einmal vollständig schließen, bevor das neue Zertifikat verwendet werden kann.
