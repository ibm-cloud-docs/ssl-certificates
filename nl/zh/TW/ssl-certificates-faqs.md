---

copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"

keywords: SSL certificates FAQ, SSL FAQ

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:faq: data-hd-content-type='faq'}

<a name="top"></a>
# 常見問題：SSL 憑證
{: #faqs-ssl-certificates}

## 我訂購的 SSL 憑證為何未自動顯示在 SSL 憑證畫面上？
{:faq}

SSL 憑證由第三方憑證管理中心核發，該單位會以機密電子郵件，將所有憑證詳細資料直接傳送給您。收到該封電子郵件之後，您可以選擇[將 SSL 憑證匯入](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates)至 {{site.data.keyword.slportal_full}}（如果您選擇使用憑證搭配 {{site.data.keyword.BluSoftlayer_full}} 產品及服務的話）。因為 {{site.data.keyword.cloud_notm}} 絕不會收到 SSL 憑證的詳細資料，所以無法自動匯入資料。

## 何謂 SSL 憑證？
{:faq}

網站會啟用 SSL 憑證，作為保護使用者的安全措施。它們通常用於您需要將機密資訊（例如，姓名、地址、信用卡號碼及其他個人資料）傳輸至網站時，或是用於您管理需要鑑別的資料時（例如，在 {{site.data.keyword.slportal}} 內）。SSL 憑證由經營網站的公司要求，但由可確保網站有效性的信任第三方公司發出。在 URL 中，安全的網站前面會加上 HTTPS，而不是標準 HTTP。

## 如何訂購 SHA2 SSL？
{:faq}

如果您已訂購 SSL，且畫面上顯示 SSL 憑證使用 SHA-1 而非 SHA-2 的錯誤，則您需要要求重新發出 SSL。您可以提交問題單來達成此目的。

如果您尚未向 {{site.data.keyword.cloud_notm}} 訂購 SSL，而需要訂購使用 SHA-2 的 SSL，請提交問題單，以針對討論中的網域手動訂購 SSL。{{site.data.keyword.slportal}} 仍會使用 SHA-1 自動建立 SSL 憑證，因此如果您這樣做，則您將需要讓我們重新發出 SSL 憑證。
