---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# VPN-Zugriff über PPTP aktivieren oder inaktivieren

Mit PPTP VPN können Benutzer einen sicheren Tunnel zum privaten {{site.data.keyword.BluSoftlayer_full}}-Netz mit einer speziellen Client-Software einrichten, die auf ihrem Desktop oder dedizierten Gerät ausgeführt wird. Der Zugriff über PPTP ist für Kunden geeignet, die Verbindungen für ein gesamtes Büro einrichten müssen oder nicht die VPN-Lösung über SSL verwenden können. Jedem Kunden wird eine PPTP-Verbindung zugewiesen, wobei zusätzliche Verbindungen verfügbar sind; für unbegrenzten PPTP-Zugriff muss jedoch Unterstützung angefordert werden, die aber kostenlos zur Verfügung steht. Um den VPN-Zugriff über PPTP für einen Benutzer zu aktivieren oder zu inaktivieren, führen Sie die folgenden Schritte aus.

1. Greifen Sie als Administrator mit Ihren eindeutigen Berechtigungsnachweisen auf das [{{site.data.keyword.slportal_full}} ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/){: new_window} zu.
2. Suchen Sie nach dem Benutzer, dessen Zugriff Sie ändern möchten, und sehen Sie sich die Spalte für den **VPN-Zugriff** an, um die aktuelle Zugriffsebene des Benutzers herauszufinden.
3. Wählen Sie aus dem Menü **Aktionen** die Option **VPN-Zugriff bearbeiten**.
4. Geben Sie den VPN-Typ und die Details für den Teilnetzzugriff ein.

|Feldname  |Optionen   |
| -----------| ------------ |
| VPN-Typ   | Keiner, SSL, PPTP oder beide (SSL und PPTP) |
|Teilnetzzugriff | Autom. oder manuell |           
{: caption="Tabelle 1. Optionen für die Bearbeitung des VPN-Zugriffs" caption-side="top"}   
5. Klicken Sie auf **Speichern**, um die Änderungen zu speichern.

   **Hinweis:** Der Zugriff über PPTP muss aktiviert sein, damit ein Benutzer über PPTP eine Verbindung herstellen kann.
