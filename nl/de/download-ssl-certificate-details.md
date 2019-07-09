---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificate details, preferred Download Option, SSL certificate download details

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL-Zertifikatsdetails herunterladen
{: #downloading-ssl-certificate-details}

Nachdem ein SSL-Zertifikat der {{site.data.keyword.cloud}}-Konsole hinzugefügt wurde, können die Details dieses Zertifikats jederzeit heruntergeladen werden. Zu den herunterladbaren Inhalten zählen das Zertifikat, der Schlüssel oder die PEM-formatierte Version des Zertifikats mit allen verfügbaren Details zu dem SSL-Zertifikat. SSL-Zertifikatsdetails werden sicher heruntergeladen; es bestehen daher keine Risiken beim Abrufen der Details mit dieser Methode.
{:shortdesc}

Führen Sie die folgenden Schritte aus, um die Details für das SSL-Zertifikat herunterzuladen.

1. Navigieren Sie zum Sicherheitsmenü Ihrer Konsole. Weitere Informationen finden Sie unter [Zu Einheiten navigieren](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. Wählen Sie im Menü **Sicherheit** die Option **SSL > Zertifikate** aus.
3. Wählen Sie aus dem Menü **Aktionen** die bevorzugte **Downloadoption** für das Zertifikat aus. Weitere Informationen hierzu finden Sie in der folgenden Tabelle:

| Downloadoption      | Downloadinformationen |
| -------------------- | -------------------- |
| Zertifikat herunterladen | Lädt nur den Zertifikatsteil herunter und enthält nicht den privaten Schlüssel, das Zwischenzertifikat, die Zertifikatssignieranforderung oder Anmmerkungsdetails. |
| Schlüssel herunterladen         | Lädt nur den privaten Schlüssel herunter und umfasst nicht das Zertifikat, das Zwischenzertifikat, die Zertifikatssignieranforderung oder Anmerkungsdetails. |
| PEM herunterladen         | Lädt alle Details zum SSL-Zertifikat herunter, darunter das Zertifikat, der private Schlüssel, das Zwischenzertifikat, die Zertifikatssignieranforderung und Anmerkungsdetails. |
{: caption="Tabelle 1. Downloadoptionen" caption-side="top"}

## Nächste Schritte

Nachdem Sie das Herunterladen der SSL-Zertifikatsdetails angefordert haben, werden diese automatisch im Web-Browser heruntergeladen. Wählen Sie den Download aus, um die Datei zu öffnen. Sie können die Datei auch als zukünftige Referenz auf Ihrer Workstation speichern. Jedoch können Daten für alle SSL-Zertifikate, die in der Anzeige mit den SSL-Zertifikaten enthalten sind, jederzeit automatisch heruntergeladen werden, indem Sie die oben aufgeführten Schritte wiederholen.

