---

copyright:
  years: 2014, 2018
lastupdated: "2018-05-17"

keywords: PPTP VPN access, PPTP VPN, PPTP access

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 啟動或取消啟動 PPTP VPN 存取
{: #activating-or-deactivating-pptp-vpn-access}

PPTP VPN 可讓使用者利用在桌上型電腦或專用裝置上執行的特殊化用戶端軟體，來形成與 {{site.data.keyword.BluSoftlayer_full}} 專用網路的安全通道。PPTP 存取是針對需要連接整個辦公室或無法使用 SSL VPN 解決方案的客戶而設計的。每一位客戶會分配到一條 PPTP 連線，並且可以使用額外的連線，但需要要求支援才能啟用無限制的 PPTP 存取（不需另外付費）。若要啟動或取消啟動使用者的 PPTP VPN 存取，請完成下列步驟。

1. 使用您的唯一認證，以管理者的身分存取 [{{site.data.keyword.slportal_full}} ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/){: new_window}。
2. 找到您要修改存取的使用者，並檢視 **VPN 存取**直欄，以檢視其現行存取層次。
3. 從**動作**功能表，選取**編輯 VPN 存取**。
4. 輸入 VPN 類型及子網路存取詳細資料。

|欄位名稱|選項|
| -----------| ------------ |
|VPN 類型|無、SSL、PPTP 或兩者（SSL 和 PPTP）|
|子網路存取|自動或手動|           
{: caption="表 1. VPN 及子網路詳細資料" caption-side="top"}   
5. 按一下**儲存**，以儲存您的變更。

   **附註：**必須啟動 PPTP 存取，使用者才能使用 PPTP 進行連接。
