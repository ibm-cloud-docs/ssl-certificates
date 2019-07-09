---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: PPTP VPN access, PPTP VPN, PPTP access

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:external: target="_blank" .external}

# VPN-Zugriff über PPTP aktivieren oder inaktivieren
{: #activating-or-deactivating-pptp-vpn-access}

Mit PPTP VPN können Sie einen sicheren Tunnel zum privaten {{site.data.keyword.cloud}}-Netz mit einer speziellen Client-Software einrichten, die auf Ihrem Desktop oder Ihrer dedizierten Einheit ausgeführt wird. Der PPTP-Zugriff ist geeignet, wenn Sie die Verbindungen für ein gesamtes Büro einrichten müssen oder nicht die SSL-VPN-Lösung verwenden können. Ihnen wird eine PPTP-Verbindung zugewiesen, wobei weitere Verbindungen verfügbar sind, und Sie können Unterstützung für die Einrichtung unbegrenzten PPTP-Zugriffs anfordern, der ohne Aufpreis verfügbar ist. Um den VPN-Zugriff über PPTP für einen Benutzer zu aktivieren oder zu inaktivieren, führen Sie die folgenden Schritte aus.
{:shortdesc}

1. Melden Sie sich auf der Seite [Zugriff (IAM)](https://cloud.ibm.com/iam/overview){: external} in der {{site.data.keyword.cloud_notm}}-Konsole an.
2. Suchen Sie nach dem Benutzer, dessen Zugriff Sie ändern möchten, und sehen Sie sich die Spalte für den **VPN-Zugriff** an, um die aktuelle Zugriffsebene des Benutzers herauszufinden.
3. Wählen Sie aus dem Menü **Aktionen** die Option **VPN-Zugriff bearbeiten**.
4. Geben Sie den VPN-Typ und die Teilnetzzugriffsdetails ein und klicken Sie auf **Speichern**, um Ihre Änderungen zu speichern. Weitere Informationen finden Sie in der folgenden Tabelle.

|Feldname  |Optionen   |
| -----------| ------------ |
| VPN-Typ   | Keiner, SSL, PPTP oder beide (SSL und PPTP) |
| Teilnetzzugriff | Automatisch oder Manuell |           
{: caption="Tabelle 1. VPN- und Teilnetzdetails" caption-side="top"}   

Der PPTP-Zugriff muss aktiviert sein, damit ein Benutzer über PPTP eine Verbindung herstellen kann.
{:note}
