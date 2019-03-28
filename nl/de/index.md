---

copyright:
  years: 2014, 2018
lastupdated: "2018-08-15"

keywords: types of certificates,SSL certificates, Select Security

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Lernprogramm 'Einführung'
{: #getting-started-tutorial}


## Vorbereitung

Für die ersten Schritte bei der Verwendung von SSL-Zertifikaten ist eine gewisse Planung erforderlich. Schaffen Sie dazu folgende Voraussetzungen.

1. Überlegen Sie, wo Sie das Zertifikat abrufen möchten.
2. Machen Sie sich mit Zertifikatstypen, Schlüssellänge und Gültigkeitsdauer von Zertifikaten vertraut.
3. Wählen Sie einen allgemeinen Namen aus.
4. Machen Sie sich mit der Socketregel vertraut.
5. Generieren Sie die Zertifikatssignieranforderung.

Weitere Informationen finden Sie in [Planung für SSL-Zertifikate](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-planning-for-ssl).

## SSL-Zertifikate bestellen

1. Greifen Sie mit Ihren eindeutigen Berechtigungsnachweisen auf das [{{site.data.keyword.slportal_full}} ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/){: new_window} zu.
2. Wählen Sie **Sicherheit > SSL-Zertifikate >** aus, um auf die Anzeige mit den SSL-Zertifikaten zuzugreifen.
3. Sie müssen den Typ und die Gültigkeitsdauer des Zertifikats auswählen, den Text der Zertifikatssignieranforderung abschicken, einige zusätzliche Details eingeben und dann die Zahlung bestätigen.

## Installation und Test
Nachdem der Bestell- und Validierungsprozess abgeschlossen ist, erhalten Sie von der Zertifizierungsstelle eine E-Mail mit Ihrem Zertifikat und bei Bedarf allen erforderlichen Zwischenzertifikaten. Die Installationsmethode ist zwar von der von Ihnen verwendeten Software abhängig, das Ergebnis sollte aber in allen Fällen gleich sein. Wenn Sie den Vorgang abgeschlossen haben, sollten Sie <http://host.yourdomain.com> aufrufen und Ihre Inhalte sowie das SSL-Schloss sehen können, mit dem in Browsern eine verschlüsselte Sitzung angezeigt wird. Wird eine Warnung angezeigt, gibt es bestimmte Schritte, die Sie ausführen müssen.

## Nächste Schritte

Nach einem erfolgreichen Test können Sie auf die Anzeige mit den SSL-Zertifikaten zugreifen, um vorhandene Zertifikate zu [aktualisieren](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates), [herunterzuladen](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details), zu [löschen](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates) oder in das Tool zu [importieren](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates).
