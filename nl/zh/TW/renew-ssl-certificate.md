---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords:  renewing SSL certificates, renewal SSL, SSL certificate renewal process, renewing, renewal

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 更新 SSL 憑證
{: #renewing-ssl-certificates}

透過 {{site.data.keyword.cloud}} 訂購 SSL 憑證之後，可以隨時更新它。在更新過程中，{{site.data.keyword.cloud_notm}} 會作為您與憑證管理中心之間的引導者，且不會看到或控制涉及 SSL 憑證詳細資料之更新程序的任何部分。SSL 憑證會根據訂購它們的相同條款來更新，因此無法變更更新詳細資料（憑證類型及管理中心、有效性月份、伺服器平台等等）。憑證可以在過期之前或之後更新，不過為了維護 SSL 憑證的有效性，請在到期日之前更新憑證。
{:shortdesc}

## 更新 SSL 憑證
請完成下列步驟，更新 SSL 憑證。

1. 導覽至主控台的安全功能表。如需相關資訊，請參閱[導覽至裝置](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)。
2. 從**安全**功能表，選取 **SSL > 訂單**。
3. 針對想要的 SSL 憑證，按一下**更新**直欄中的**更新**。
4. 在更新 SSL 憑證之前，判斷所有更新和 CSR 詳細資料是否正確。請參閱下表，以取得相關資訊。  

|詳細資料|動作|
| ------------------------------- | ------- |
|正確的更新及 CSR 詳細資料|選取**更新**來更新 SSL 憑證。|
|不正確的更新詳細資料|選取**購買新的 SSL 憑證**來訂購新憑證。由於無法變更更新詳細資料，包括憑證類型、管理中心、核准電子郵件，所以更新網站 SSL 憑證詳細資料的唯一方法是訂購新的憑證。|
|不正確的 CSR 詳細資料|選取**變更 CSR**、在 **CSR 文字框**中輸入新的 CSR 詳細資料，然後選取**還原 CSR**。|
{: caption="表 1. 更新及 CSR 詳細資料" caption-side="top"}

## 後續步驟

要求 SSL 憑證的更新之後，{{site.data.keyword.cloud_notm}} 會將要求轉遞至憑證管理中心，以便完成更新所需的網站驗證。更新憑證時，新的到期日會出現在**到期**欄位中。
