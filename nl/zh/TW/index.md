---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-21"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 開始使用 SSL 憑證  


## 開始之前

開始使用 SSL 需要進行一些規劃。請完成下列必要條件。

1. 決定憑證的取得位置
2. 瞭解憑證類型、金鑰長度及持續時間
3. 選擇通用名稱
4. 瞭解 Socket 規則
5. 產生 CSR

如需相關資訊，請參閱[規劃 SSL 憑證](planning-ahead-ssl.html)。

## 訂購 SSL 憑證

1. 使用您的唯一認證來存取 [{{site.data.keyword.slportal_full}} ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/){: new_window}。
2. 選取**安全 > SSL 憑證**來存取 SSL 憑證畫面。
3. 您必須選取憑證的類型和持續時間、提交 CSR 的文字、輸入其他詳細資料，然後確認付款。

## 安裝和測試
訂購及驗證程序完成之後，您會收到來自憑證管理中心的電子郵件，其中包括您的憑證以及任何必要的中繼憑證。安裝方法視您使用的軟體而定，但結果應該相同。完成後，您應該能夠前往 <http://host.yourdomain.com> 並查看您的內容，同時還會看到瀏覽器用來表示已加密階段作業的 SSL 小鎖。如果您收到警告，則必須執行一些步驟。

## 後續步驟

在順利測試之後，您可以存取 SSL 憑證畫面，以[更新](view-and-update-ssl-certificate.html)、[下載](download-ssl-certificate-details.html)或[刪除](delete-ssl-certificate.html)現有的 SSL 憑證，或將現有的 SSL 憑證[匯入](import-ssl-certificate.html)到工具中。
