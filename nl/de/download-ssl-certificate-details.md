---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL-Zertifikatsdetails herunterladen

Nachdem ein SSL-Zertifikat zum {{site.data.keyword.slportal_full}} hinzugefügt wurde, können die Details dieses Zertifikats jederzeit heruntergeladen werden. Zu den heruntergeladenen Inhalten zählen das Zertifikat, der Schlüssel oder die PEM-formatierte Version des Zertifikats mit allen verfügbaren Details zu dem SSL-Zertifikat. SSL-Zertifikatsdetails werden sicher heruntergeladen; es bestehen daher keine Risiken beim Abrufen der Details mit dieser Methode.

Führen Sie die folgenden Schritte aus, um die Details für das SSL-Zertifikat herunterzuladen.

1. Greifen Sie mit Ihren eindeutigen Berechtigungsnachweisen auf das [{{site.data.keyword.slportal_full}} ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/){: new_window} zu.
2. Wählen Sie im Menü **Sicherheit** die Option **SSL > Zertifikate** aus.
3. Wählen Sie aus dem Menü **Aktionen** die bevorzugte **Downloadoption** für das Zertifikat aus. Weitere Informationen hierzu finden Sie in der folgenden Tabelle:<br /> <br /><table border="1"><tr><th>Downloadoption</th><th>Heruntergeladene Informationen</th></tr><tr><td>Zertifikat herunterladen</td><td>Lädt nur den Zertifikatsteil herunter und enthält nicht den privaten Schlüssel, das Zwischenzertifikat, die Zertifikatssignieranforderung oder Anmmerkungsdetails.</td></tr><tr><td>Schlüssel herunterladen</td><td>Lädt nur den privaten Schlüssel herunter und umfasst nicht das Zertifikat, das Zwischenzertifikat, die Zertifikatssignieranforderung oder Anmerkungsdetails.</td></tr><tr><td>PEM herunterladen</td><td>Lädt alle Details zum SSL-Zertifikat herunter, darunter das Zertifikat, der private Schlüssel, das Zwischenzertifikat, die Zertifikatssignieranforderung und Anmerkungen.</td></tr></table>

## Nächste Schritte

Nachdem Sie das Herunterladen der SSL-Zertifikatsdetails angefordert haben, werden diese automatisch im Web-Browser heruntergeladen. Wählen Sie den Download aus, um die Datei zu öffnen. Sie können die Datei auch als zukünftige Referenz auf Ihrer Workstation speichern. Jedoch können Daten für alle SSL-Zertifikate, die in der Anzeige mit den SSL-Zertifikaten enthalten sind, jederzeit automatisch heruntergeladen werden, indem Sie die oben aufgeführten Schritte wiederholen.
