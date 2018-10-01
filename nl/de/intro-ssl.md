---
copyright:
  years: 2014, 2018
lastupdated: "2018-05-17"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Einführung in die SSL-Technologie

Secure Sockets Layer (SSL) ist eine Technologie, mit der Datenverkehr zwischen der Clientanwendung und der Serveranwendung verschlüsselt wird. Die Verschlüsselung erfolgt durch die Verwendung eines Systems für öffentliche/private Schlüssel, das ein SSL-Zertifikat verwendet.

Das SSL-Zertifikat enthält den öffentlichen Schlüssel des Servers, den Gültigkeitszeitraum des Zertifikats, einen Hostnamen, für den das Zertifikat gilt, und eine Signatur von der ausstellenden Zertifizierungsstelle.

## SSL-Terminologie

SSL-Zertifikate verwenden eine eindeutige Terminologie. Bei der Arbeit mit SSL-Zertifikaten können Sie daher beispielsweise auf die folgenden Begriffe stoßen: 

**Bitgröße:** Verschlüsselungsschlüssel werden anhand ihrer Größe in Bit gemessen. Beispiel: 512 Bit, 1024 Bit, 2048 Bit. In der Regel ist ein längerer Schlüssel zwar sicherer, die Verarbeitung jedoch langsamer. Zum gegenwärtigen Zeitpunkt beträgt die Mindestgröße für in SSL-Zertifikaten verwendete Schlüssel 1024 Bit; für Extended-Validation-Zertifikate (EV) sind jedoch 2048 Bit erforderlich.

**Zertifikatskette:** SSL-Zertifikate werden für gewöhnlich nicht alleine verwendet. In den meisten Implementierungen wird eine Zertifikatskette verwendet. Beispiel:

  Stammzertifikat > Zwischenzertifikat1 > Serverzertifikat

  \> Zwischenzertifikat2 > Zertifikat Server2

In diesem Beispiel wird das Serverzertifikat vom Zwischenzertifikat signiert, welches wiederum vom Stammzertifikat signiert wird. Durch eine Kettung dieser Art kann SSL sicherer gemacht werden, da das Stammzertifikat nicht so häufig verwendet wird (und somit Risiken ausgesetzt wird). Wenn die Sicherheit von Zwischenzertifikat1 beeinträchtigt wurde, könnte das Serverzertifikat gefährdet sein, das Zertifikat für Server2 wäre jedoch nicht gefährdet, da die Zertifikate unterschiedlichen Ketten angehören.

**Zertifikatssignieranforderung:** Die Zertifikatssignieranforderung ist ein Dokument, das Sie auf dem Server generieren und das Informationen enthält, anhand derer die Zertifizierungsstelle Ihr Zertifikat erstellt.

**Allgemeiner Name:** Der allgemeine Name ist der Hostname, für den das Zertifikat gilt (z. B. 'www.domain.com').  

*Hinweis:* 'www.domain.com', 'smtp.domain.com' und 'mail.domain.com' sind drei unterschiedliche Hostnamen, für die nicht dasselbe SSL-Zertifikat verwendet werden kann (es sei denn, Sie verwenden ein Platzhalterzertifikat, das jedoch momentan nicht von {{site.data.keyword.cloud}} angeboten wird).

**Privater/öffentlicher Schlüssel:** SSL nutzt ein Verfahren, das sich Public-Key-Verschlüsselung nennt. Dabei stehen zwei Schlüssel zur Verfügung: der öffentliche und der private Schlüssel. Der öffentliche Schlüssel wird weitreichend verteilt. Niemand sieht den privaten Schlüssel. Benutzer, die sicher mit Ihnen kommunizieren möchten, verschlüsseln die Kommunikation mit Ihrem öffentlichen Schlüssel. Die Public-Key-Verschlüsselung basiert auf dem Anspruch, dass Bits, die mit einem bestimmten öffentlichen Schlüssel verschlüsselt wurden, nur mit dem entsprechenden privaten Schlüssel entschlüsselt werden können (und umgekehrt).

**Stammzertifikat:** Die SSL-Stammzertifikate sind Zertifikate mit Selbstsignierung, die von den entsprechenden Zertifizierungsstellen präsentiert werden. Stammzertifikate für Zertifizierungsstellen sind bereits im Zertifikatsspeicher für Ihren Web-Browser installiert. Somit kann Ihr Browser diesen Zertifikaten vertrauen; dies ist der Anfang der Zertifikatskette, die schließlich zu dem auf dem Server installierten Zertifikat führt.

**Signatur:** SSL-Zertifikate verfügen über eine digitale Signatur, die sie von der Zertifizierungsstelle erhalten. Wenn sie zurück zu einem Trusted-Root-Zertifikat verfolgt wird, wird mit dieser Signatur die Authentizität des Zertifikats bestätigt.

## SSL bei IBM Cloud Infrastructure

{{site.data.keyword.BluSoftlayer_full}} verkauft drei Typen von SSL-Zertifikaten: Domain-Validation (DV), Organization-Validation (OV) und Extended-Validation (EV). 

Domain-Validation-Zertifikate (DV-Zertifikate) sind kosteneffizient und schnell verfügbar. Die von der Zertifizierungsstelle durchgeführte Validierung beschränkt sich auf das Senden einer E-Mail an eine angegebene E-Mail-Adresse in der betreffenden Domäne und dem Erhalt einer positiven Antwort auf diese E-Mail. Für die Bereitstellung von Organization-Validation- (OV) und Extended-Validation-Zertifikaten (EV) werden einige Tage (manchmal eine Woche) benötigt, sie kosten mehr und werden von der Zertifizierungsstelle eingehender überprüft. Die EV-Zertifikate sind so codiert, dass Browser sie als EV-Zertifikate erkennen und sie einen grünen Balken als Teil der Adressleiste aufweisen. 

Wie andere {{site.data.keyword.cloud_notm}}-Services auch können SSL-Zertifikate über das {{site.data.keyword.slportal}} verwaltet werden. Rufen Sie das Menü **Sicherheit** auf und wählen Sie die Option **SSL-Zertifikate** auf, um Zertifikate zu bestellen und zu verwalten.  

**Hinweis:** SSL-Zertifikate, die über {{site.data.keyword.cloud_notm}} angefordert werden, müssen nicht für einen {{site.data.keyword.BluSoftlayer_notm}}-Server verwendet werden. Außerdem können über eine andere Stelle angeforderte Zertifikate auf den hier gehosteten Servern verwendet werden.

Mit SSL-Zertifikaten kann die Sicherheit von Transaktionen erhöht und Benutzern ein sichereres Gefühl verliehen werden. Neben den SSL-Zertifikaten liefert die Kombination aus Dämonensicherheit, physischer Sicherheit, Programmierpraxis und Handhabung von Zertifikaten ein optimales Sicherheitsprofil der Lösung.
