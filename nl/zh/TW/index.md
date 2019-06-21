---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-11"

keywords: types of certificates,SSL certificates, Select Security

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 入門指導教學
{: #getting-started-tutorial}

## 開始之前

開始使用 SSL 需要進行一些規劃。請完成下列必要條件。

1. 決定憑證的取得位置
2. 瞭解憑證類型、金鑰長度及持續時間
3. 選擇通用名稱
4. 瞭解 Socket 規則
5. 產生 CSR

如需相關資訊，請參閱[規劃 SSL 憑證](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-planning-for-ssl#planning-for-ssl)。

## 訂購 SSL 憑證

1. 導覽至主控台的安全功能表。如需相關資訊，請參閱[導覽至裝置](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)。
2. 從**安全**功能表中，選取 **安全 > SSL > 憑證**。
3. 選取**訂購 SSL 憑證**。
3. 選取憑證的類型和持續時間、提交 CSR 的文字、選取伺服器平台，然後確認付款。

## 安裝和測試
訂購及驗證程序完成之後，您會收到來自憑證管理中心的電子郵件，其中包括您的憑證以及任何必要的中繼憑證。安裝方法視您使用的軟體而定，但結果應該相同。完成後，您應該能夠前往 `http://host.yourdomain.com` 並查看您的內容，同時還會看到瀏覽器用來表示已加密階段作業的 SSL 小鎖。如果您收到警告，則必須執行一些步驟。

## 後續步驟

在順利測試之後，您可以在 {{site.data.keyword.cloud_notm}} 主控台存取 SSL 憑證，以[更新](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates#viewing-and-updating-ssl-certificates)、[下載](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details#downloading-ssl-certificate-details)或[刪除](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates)現有的 SSL 憑證，或將現有的 SSL 憑證[匯入](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates)到工具中。
