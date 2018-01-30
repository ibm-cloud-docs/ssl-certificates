---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 匯入 SSL 憑證

## 概觀

發出網站的 SSL 憑證之後，它可以匯入到 {{site.data.keyword.slportal_full}} 中。透過將 SSL 憑證匯入到 {{site.data.keyword.slportal}}，憑證可以套用至可能需要它們的產品和服務，例如負載平衡器的 [SSL 卸載](configure-ssl-offloading-load-balancer.html){:new_window}。依預設，{{site.data.keyword.BluSoftlayer_full}} 所發出的 SSL 憑證不會匯入到清單中，因為它們只供收件者操作之用。因此，必須由帳戶上的授權使用者手動匯入要與 {{site.data.keyword.BluSoftlayer_notm}} 產品或服務搭配使用的任何 SSL 憑證。請遵循下列步驟，將 SSL 憑證匯入到 {{site.data.keyword.slportal}} 中。

## 匯入 SSL 憑證

1. 使用您的唯一認證來存取 [{{site.data.keyword.slportal_full}} ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/){: new_window}。
2. 從**安全**功能表，選取 **SSL > 憑證**。
3. 按一下畫面頂端的**匯入 SSL 憑證**鏈結。
4. 在適合的欄位中輸入 **SSL 憑證詳細資料**，然後按一下**匯入**。

   **附註：****匯入 SSL 憑證**視窗中輸入的詳細資料，輸入時必須與憑證管理中心提供的資料完全相同，包括間距和換行。否則會發生錯誤。

| 文字框 | 項目|
| -------- | ----- |
|憑證|憑證管理中心所提供的 SSL 憑證詳細資料。這通常是一個英數文字區塊。|
|私密金鑰| 憑證管理中心所提供的憑證私密金鑰詳細資料。這通常是一個英數文字區塊。|
|中繼憑證| 憑證管理中心所提供的中繼憑證詳細資料。中繼憑證不是必要項目，不過如果該資訊可用於 SSL 憑證，則應輸入。|
| 憑證簽署要求| 憑證管理中心所提供的憑證簽署要求 (CSR) 詳細資料。CSR 詳細資料不是必要項目，但如果它們是憑證的一部分，則應提供。**附註：**請勿以任何方式變更 CSR。公開金鑰可能附在 CSR 且不應該以私密金鑰取代。|
|附註| 有關 SSL 憑證，可能有助於其他使用者的任何附註。


## 後續步驟

SSL 憑證匯入到 {{site.data.keyword.slportal}} 之後，它會儲存在 SSL 憑證畫面中，直到[手動刪除](delete-ssl-certificate.html)為止。對於所有需要 SSL 憑證詳細資料的產品或服務，新的 SSL 憑證會出現在可用的憑證清單裡，以便與所需產品或服務的 SSL 特性互動時使用。憑證可以隨時[更新](view-and-update-ssl-certificate.html)，而有關憑證的詳細資料可以隨時[安全地下載](download-ssl-certificate-details.html)。
