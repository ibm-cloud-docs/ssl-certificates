---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL-Zertifikate verlängern

## Übersicht

Nachdem ein SSL-Zertifikat über {{site.data.keyword.BluSoftlayer_full}} angefordert wurde, kann es jederzeit verlängert werden. Während des Verlängerungsvorgangs fungiert {{site.data.keyword.BluSoftlayer_notm}} als eine Art Vermittler zwischen dem Kunden (Ihnen) und der Zertifizierungsstelle und kommt während dieses Vorgangs mit keinen Details des SSL-Zertifikats in Berührung. SSL-Zertifikate werden unter denselben Bedingungen wie bei ihrer Anforderung verlängert, daher müssen keine Änderungen an den Details für die Verlängerung (Zertifikatstyp und Zertifizierungsstelle, Gültigkeit, Serverplattform usw.) vorgenommen werden. Zertifikate können vor und nach ihrem Ablauf verlängert werden; um jedoch die Gültigkeit des SSL-Zertifikats zu gewährleisten, verlängern Sie das Zertifikat vor dessen Ablaufdatum. Führen Sie die nachfolgenden Schritte aus, um ein SSL-Zertifikat zu verlängern.

## SSL-Zertifikat verlängern

1. Greifen Sie mit Ihren eindeutigen Berechtigungsnachweisen auf das [{{site.data.keyword.slportal_full}} ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/){: new_window} zu.
2. Wählen Sie im Menü **Sicherheit** die Option **SSL > Bestellungen** aus.
3. Klicken Sie in der Spalte **Verlängern** des entsprechenden SSL-Zertifikats auf den Link zum **Verlängern**.

   **Hinweis:** Es wird ein Popup-Fenster zum Abschließen der Anforderung angezeigt.  
   * Stellen Sie fest, ob alle Details für die Verlängerung und die Zertifikatssignieranforderung korrekt sind:<br /><br /><table border="1"><tr><th>Wenn...</th><th>Dann...</th></tr><tr><td>Details für die Verlängerung und die Zertifikatssignieranforderung korrekt sind</td><td>Fahren Sie mit dem nächsten Schritt fort.</td></tr><tr><td>Details für die Verlängerung falsch sind</td><td><ul><li>Klicken Sie auf den Link zum <strong>Kaufen eines neuen SSL-Zertifikats</strong>, um an die Verkaufsanzeige weitergeleitet zu werden.<br /><blockquote><strong>Hinweis:</strong> Da die Details für die Verlängerung, wie Zertifikatstyp, Zertifizierungsstelle und Genehmigungs-E-Mail, nicht geändert werden können, können die Details für das SSL-Zertifikat einer Website ausschließlich durch das Anfordern eines neuen Zertifikats aktualisiert werden.</blockquote></li><li>Füllen Sie die Anzeigen auf der Bestellseite mit den gewünschten Informationen für das SSL-Zertifikat aus. Bei der Verwendung dieser Methode sind keine zusätzlichen Aktionen erforderlich.</li></ul></td></tr><tr><td>Details der Zertifikatssignieranforderung falsch sind</td><td><ul><li>Klicken Sie auf die Schaltfläche zum **Ändern der Zertifikatssignieranforderung**.</li><li>Geben Sie die **neuen Details für die Zertifikatssignieranforderung** im Textfeld für die **Zertifikatssignieranforderung** ein.</li><li>Klicken Sie auf die Schaltfläche zum **Wiederherstellen der Zertifikatssignieranforderung**.</li></ul></td></tr></table>
4. Klicken Sie auf die Schaltfläche zum **Verlängern**, um das SSL-Zertifikat zu verlängern, oder auf **Abbrechen**, um die Aktion abzubrechen.

## Nächste Schritte

Nachdem Sie die Verlängerung eines SSL-Zertifikats angefordert haben, leitet {{site.data.keyword.BluSoftlayer_notm}} die Anforderung an die Zertifizierungsstelle weiter, um die Websiteprüfung abzuschließen, die für die Verlängerung erforderlich ist. Sobald das Zertifikat verlängert wird, wird das neue Ablaufdatum im Feld mit dem Ablaufdatum angezeigt.
