---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:faq: data-hd-content-type='faq'}

<a name="top"></a>
# Häufig gestellte Fragen: SSL-Zertifikate

## Warum wird das von mir bestellte SSL-Zertifikat nicht automatisch in der Anzeige mit den SSL-Zertifikaten angezeigt?
{:faq}

SSL-Zertifikate werden von einer unabhängigen Zertifizierungsstelle ausgestellt, die Ihnen alle Zertifikatsdetails direkt in einer vertraulichen E-Mail zukommen lässt. Nach dem Erhalt dieser E-Mail können Sie das SSL-Zertifikat in das {{site.data.keyword.slportal_full}} [importieren](import-ssl-certificate.html), falls Sie das Zertifikat mit {{site.data.keyword.BluSoftlayer_full}}-Produkten und -Services verwenden möchten. Da {{site.data.keyword.cloud_notm}} nie die SSL-Zertifikatsdetails erhält, können Daten nicht automatisch importiert werden.

## Was ist ein SSL-Zertifikat?
{:faq}

SSL-Zertifikate werden von Websites als Sicherheitsmechanismus zum Schutz des Benutzers implementiert. Diese Zertifikate werden in der Regel verwendet, wenn Sie vertrauliche Informationen, wie Name, Adresse, Kreditkartennummer und andere persönliche Daten, an eine Website übertragen müssen. Außerdem werden mit den Zertifikaten Daten verwaltet, für die eine Authentifizierung (wie im {{site.data.keyword.slportal}}) erforderlich ist. SSL-Zertifikate werden von dem Unternehmen angefordert, das die Website betreibt, jedoch von einem vertrauenswürdigen Drittanbieter ausgestellt, der die Gültigkeit der Website sicherstellt. Sichere Websites sind im Gegensatz zum standardmäßig verwendeten 'HTTP' leicht durch das vorgestellte 'HTTPS' in der URL erkennbar.

## Wie kann ich ein SSL-Zertifikat mit dem Hash-Algorithmus SHA-2 bestellen?
{:faq}

Wenn Sie bereits ein SSL-Zertifikat angefordert haben und Fehler angezeigt werden, die angeben, dass das SSL-Zertifikat SHA-1 anstelle von SHA-2 verwendet, müssen Sie die erneute Ausstellung des SSL-Zertifikats anfordern. Dies können Sie durch das Einreichen eines Tickets erreichen.

Wenn Sie noch kein SSL-Zertifikat bei {{site.data.keyword.cloud_notm}} angefordert haben und ein Zertifikat mit SHA-2 benötigen, reichen Sie ein Ticket ein, um manuell ein SSL-Zertifikat für die entsprechende Domäne anzufordern. Da über das {{site.data.keyword.slportal}} immer noch automatisch SSL-Zertifikate mit SHA-1 erstellt werden, müssen Sie das ausgestellte Zertifikat erneut anfordern.
