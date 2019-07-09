---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords:  renewing SSL certificates, renewal SSL, SSL certificate renewal process, renewing, renewal

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL-Zertifikate verlängern
{: #renewing-ssl-certificates}

Nachdem ein SSL-Zertifikat über {{site.data.keyword.cloud}} angefordert wurde, kann es jederzeit verlängert werden. Während des Verlängerungsvorgangs fungiert {{site.data.keyword.cloud_notm}} als eine Art Vermittler zwischen Ihnen und der Zertifizierungsstelle und kommt während dieses Vorgangs mit keinen Details des SSL-Zertifikats in Berührung. SSL-Zertifikate werden unter denselben Bedingungen wie bei ihrer Bestellung verlängert, weshalb keine Änderungen an den Details für die Verlängerung (Zertifikatstyp und Zertifizierungsstelle, Gültigkeit, Serverplattform usw.) vorgenommen werden können. Zertifikate können vor und nach ihrem Ablauf verlängert werden; um jedoch die Gültigkeit des SSL-Zertifikats zu gewährleisten, verlängern Sie das Zertifikat vor dessen Ablaufdatum.
{:shortdesc}

## SSL-Zertifikat verlängern
Führen Sie die nachfolgenden Schritte aus, um ein SSL-Zertifikat zu verlängern.

1. Navigieren Sie zum Sicherheitsmenü Ihrer Konsole. Weitere Informationen finden Sie unter [Zu Einheiten navigieren](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. Wählen Sie im Menü **Sicherheit** die Option **SSL > Bestellungen** aus.
3. Klicken Sie auf **Verlängern** in der Spalte **Verlängern** für das gewünschte SSL-Zertifikat.
4. Stellen Sie fest, ob alle Details für die Verlängerung und die Zertifikatssignieranforderung (Certificate Signing Request - CSR) korrekt sind, bevor Sie das SSL-Zertifikat verlängern. Weitere Informationen finden Sie in der folgenden Tabelle.  

| Details                         | Aktion  |
| ------------------------------- | ------- |
| Korrekte Verlängerungs- und CSR-Details | Wählen Sie **Verlängern** aus, um das SSL-Zertifikat zu verlängern. |
| Falsche Verlängerungsdetails | Wählen Sie **Neues SSL-Zertifikat kaufen** aus, um ein neues Zertifikat zu bestellen. Da die Details für die Verlängerung, wie Zertifikatstyp, Zertifizierungsstelle und Genehmigungs-E-Mail, nicht geändert werden können, können die Details für das SSL-Zertifikat einer Website ausschließlich durch das Bestellen eines neuen Zertifikats aktualisiert werden. |
| Falsche CSR-Details | Wählen Sie **CSR ändern** aus, geben Sie die neuen CSR-Details in das **CSR-Textfeld** ein und wählen Sie **CSR wiederherstellen** aus. |
{: caption="Tabelle 1. Details der Verlängerung und der Zertifikatssignieranforderung" caption-side="top"}

## Nächste Schritte

Nachdem Sie die Verlängerung eines SSL-Zertifikats angefordert haben, leitet {{site.data.keyword.cloud_notm}} die Anforderung an die Zertifizierungsstelle weiter, um die Websiteprüfung abzuschließen, die für die Verlängerung erforderlich ist. Sobald das Zertifikat verlängert ist, wird das neue Ablaufdatum im Feld **Ablaufdatum** angezeigt.
