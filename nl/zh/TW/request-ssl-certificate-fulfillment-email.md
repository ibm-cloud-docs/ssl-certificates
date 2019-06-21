---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificate fulfillment email, fulfillment email

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 要求 SSL 憑證履行電子郵件
{: #requesting-an-ssl-certificate-fulfillment-email}

透過 {{site.data.keyword.cloud}} 訂購新的 SSL 憑證之後，憑證管理中心會傳送履行電子郵件給訂購程序期間所提供的網域管理者。此電子郵件會包含與 SSL 憑證相關聯的所有詳細資料。您隨時都可以從 {{site.data.keyword.cloud_notm}} 主控台的「SSL 訂單」畫面中再次要求履行電子郵件。
{:shortdesc}

## 要求履行電子郵件
請完成下列步驟，以要求來自憑證管理中心的 SSL 履行電子郵件。

1. 導覽至主控台的安全功能表。如需相關資訊，請參閱[導覽至裝置](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)。
2. 從**安全**功能表，選取 **SSL > 訂單**。
3. 針對想要的 SSL 憑證，按一下**電子郵件**直欄中的**傳送**。

  即會出現一個蹦現視窗，以確認要求。這個視窗包含要求 SSL 憑證時所提供的網域管理者的電子郵件位址。
  {:note}

4. 按一下**重新傳送電子郵件**以確認選項，並要求來自憑證管理中心的額外履行電子郵件。

## 後續步驟

在要求額外的履行電子郵件之後，該要求會轉遞至適合的憑證管理中心進行完成。由於 SSL 憑證詳細資料是機密，所以 {{site.data.keyword.cloud_notm}} 不會將 SSL 憑證資料儲存在它的系統上。透過電子郵件接收 SSL 憑證詳細資料之後，必要的話，可以手動將它們[匯入](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates)至 {{site.data.keyword.cloud_notm}} 主控台。
