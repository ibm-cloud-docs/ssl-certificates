---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: view SSL certificates, update SSL certificates, original certificates

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL-Zertifikate anzeigen und aktualisieren
{: #viewing-and-updating-ssl-certificates}

Nach dem Importieren eines SSL-Zertifikats in die Anzeige für SSL-Zertifikate können Sie es jederzeit anzeigen und aktualisieren. Aktualisierungen ähneln dem [Importprozess](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates), da alle Details, die aktualisiert werden, genau dem ursprünglichen Zertifikat entsprechen müssen, einschließlich Leerzeichen und Zeilenumbrüche.
{:shortdesc}

Führen Sie die folgenden Schritte aus, um ein SSL-Zertifikat anzuzeigen und zu aktualisieren.

1. Navigieren Sie zum Sicherheitsmenü Ihrer Konsole. Weitere Informationen finden Sie unter [Zu Einheiten navigieren](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. Wählen Sie im Menü **Sicherheit** die Option **SSL > Zertifikate** aus.
3. Wählen Sie aus der Dropdown-Liste **Aktionen** die Option **Zertifikat anzeigen/aktualisieren** aus.
4. Aktualisieren Sie die **SSL-Zertifikatsdetails** in den entsprechenden Textfeldern und klicken Sie auf **Aktualisieren**, um Ihre Änderungen anzuwenden. Weitere Informationen finden Sie in der folgenden Tabelle.

   Im Fenster **SSL-Zertifikat importieren** angegebene Details müssen genauso eingegeben werden, wie sie von der Zertifizierungsstelle bereitgestellt werden, einschließlich Leerstellen und Zeilenumbrüche. Werden die Details nicht korrekt eingegeben, tritt ein Fehler auf.
   {:note}

| SSL-Zertifikatsdetails     | Beschreibung |
| --------------------------- | ----------- |
|Zertifikat                  | Von der Zertifizierungsstelle bereitgestellte SSL-Zertifikatsdetails. Hierbei handelt es sich für gewöhnlich um einen alphanumerischen Textblock.|
|Privater Schlüssel                  | Von der Zertifizierungsstelle bereitgestellte Details des privaten Schlüssels für das Zertifikat. Hierbei handelt es sich für gewöhnlich um einen alphanumerischen Textblock.|
|Zwischenzertifikat     | Von der Zertifizierungsstelle bereitgestellte Details des Zwischenzertifikats. Zwischenzertifikate sind zwar nicht erforderlich, wenn jedoch die Informationen für das SSL-Zertifikat verfügbar sind, sollten sie eingegeben werden.|
|Zertifikatssignieranforderung| Von der Zertifizierungsstelle bereitgestellte Details der Zertifikatssignieranforderung. Diese Details sind zwar nicht erforderlich, sollten aber bereitgestellt werden, falls sie Teil des Zertifikats sind. **Hinweis:** Die Zertifikatssignieranforderung darf nicht geändert werden. Sie kann einen öffentlichen Schlüssel enthalten, der nicht durch den privaten Schlüssel ersetzt werden darf.|
|Anmerkungen                        | Anmerkungen in Bezug auf das SSL-Zertifikat, die für andere Benutzer hilfreich sein können.|
{: caption="Tabelle 1. Details des SSL-Zertifikats" caption-side="top"}

## Nächste Schritte

Nachdem die Details für das SSL-Zertifikat aktualisiert wurden, hat diese Änderung keinerlei negative Auswirkungen auf die Produkte oder Services, die das Zertifikat verwenden. Das Zertifikat kann jederzeit erneut aktualisiert werden, indem Sie die oben genannten Schritte wiederholen.
