---
copyright:
  years: 2014, 2018
lastupdated: "2018-08-15"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL-Zertifikate anzeigen und aktualisieren

Nach dem Importieren eines SSL-Zertifikats in die Anzeige mit SSL-Zertifikaten können Sie diese jederzeit anzeigen und aktualisieren. Aktualisierungen ähneln dem [Importprozess](import-ssl-certificate.html), da alle Details, die aktualisiert werden, genau dem ursprünglichen Zertifikat entsprechen müssen, einschließlich Leerzeichen und Zeilenumbrüche.

Führen Sie die folgenden Schritte aus, um ein SSL-Zertifikat anzuzeigen und zu aktualisieren.

1. Greifen Sie mit Ihren eindeutigen Berechtigungsnachweisen auf das [{{site.data.keyword.slportal_full}} ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/){: new_window} zu.
2. Wählen Sie im Menü **Sicherheit** die Option **SSL > Zertifikate** aus.
2. Wählen Sie aus der Dropdown-Liste **Aktionen** die Option **Zertifikat anzeigen/aktualisieren** aus.
3. Aktualisieren Sie die **SSL-Zertifikatsdetails** in den entsprechenden Textfeldern.

   **Hinweis:** Im Fenster **SSL-Zertifikat importieren** angegebene Details müssen genauso eingegeben werden, wie sie von der Zertifizierungsstelle bereitgestellt werden, einschließlich von Leerzeichen und Zeilenbrüchen. Werden die Details nicht korrekt eingegeben, tritt ein Fehler auf.

| SSL-Zertifikatsdetails      | Beschreibung|
| --------------------------- | ----------- |
|Zertifikat                   | Von der Zertifizierungsstelle bereitgestellte SSL-Zertifikatsdetails. Hierbei handelt es sich für gewöhnlich um einen alphanumerischen Textblock.|
|Privater Schlüssel           | Von der Zertifizierungsstelle bereitgestellte Details des privaten Schlüssels für das Zertifikat. Hierbei handelt es sich für gewöhnlich um einen alphanumerischen Textblock.|
|Zwischenzertifikat           | Von der Zertifizierungsstelle bereitgestellte Details des Zwischenzertifikats. Zwischenzertifikate sind zwar nicht erforderlich, wenn jedoch die Informationen für das SSL-Zertifikat verfügbar sind, sollten diese eingegeben werden.|
|Zertifikatssignieranforderung| Von der Zertifizierungsstelle bereitgestellte Details der Zertifikatssignieranforderung. Diese Details sind zwar nicht erforderlich, sollten aber bereitgestellt werden, falls sie Teil des Zertifikats sind. **Hinweis:** Die Zertifikatssignieranforderung darf nicht geändert werden. Sie kann einen öffentlichen Schlüssel enthalten, der nicht durch den privaten Schlüssel ersetzt werden darf.|
|Anmerkungen                  | Anmerkungen in Bezug auf das SSL-Zertifikat, die für andere Benutzer hilfreich sein können.|
{: caption="Tabelle 1. Details des SSL-Zertifikats" caption-side="top"}

Klicken Sie auf **Aktualisieren**, um das SSL-Zertifikat zu aktualisieren, oder auf **Abbrechen**, um die Aktion abzubrechen.

## Nächste Schritte

Nachdem die Details für das SSL-Zertifikat aktualisiert wurden, hat diese Änderung keinerlei negative Auswirkungen auf die Produkte oder Services, die das Zertifikat verwenden. Das Zertifikat kann jederzeit erneut aktualisiert werden, indem Sie die oben genannten Schritte wiederholen.
