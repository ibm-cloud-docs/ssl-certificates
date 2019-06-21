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

# 啟動或取消啟動 PPTP VPN 存取
{: #activating-or-deactivating-pptp-vpn-access}

PPTP VPN 可讓您利用在桌上型電腦或專用裝置上執行的特殊化用戶端軟體，來形成與 {{site.data.keyword.cloud}} 專用網路的安全通道。PPTP 存取的設計是針對您需要連接整個辦公室，或是無法使用 SSL VPN 解決方案的情況。您會分配到一條 PPTP 連線，並且可以使用額外的連線，也可以要求支援以啟用無限制的 PPTP 存取（不需另外付費）。若要啟動或取消啟動使用者的 PPTP VPN 存取，請完成下列步驟。
{:shortdesc}

1. 在 {{site.data.keyword.cloud_notm}} 主控台中，登入[存取 (IAM)](https://cloud.ibm.com/iam/overview){: external} 頁面。
2. 找到您要修改存取的使用者，並檢視 **VPN 存取**直欄，以檢視其現行存取層次。
3. 從**動作**功能表，選取**編輯 VPN 存取**。
4. 輸入 VPN 類型及子網路存取詳細資料，然後按一下**儲存**，以儲存您的變更。請參閱下表，以取得相關資訊。

|欄位名稱|選項|
| -----------| ------------ |
|VPN 類型|無、SSL、PPTP 或兩者（SSL 和 PPTP）|
|子網路存取|自動或手動|           
{: caption="表 1. VPN 及子網路詳細資料" caption-side="top"}   

必須啟動 PPTP 存取，使用者才能使用 PPTP 進行連接。
{:note}
