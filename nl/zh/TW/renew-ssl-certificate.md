---
copyright:
  years: 2014, 2018
lastupdated: "2018-05-17"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 更新 SSL 憑證

透過 {{site.data.keyword.BluSoftlayer_full}} 訂購 SSL 憑證之後，可以隨時更新它。在更新程序期間，{{site.data.keyword.BluSoftlayer_notm}} 會作為客戶（您）與憑證管理中心之間的引導者，且不會看到或控制涉及 SSL 憑證詳細資料的更新程序的任何部分。SSL 憑證會根據訂購它們的相同條款來更新，因此無法變更「更新詳細資料」（憑證類型及管理中心、有效性月份、伺服器平台等等）。憑證可以在過期之前或之後更新，不過為了維護 SSL 憑證的有效性，請在到期日之前更新憑證。請完成下列步驟，更新 SSL 憑證。

## 更新 SSL 憑證

1. 使用您的唯一認證來存取 [{{site.data.keyword.slportal_full}} ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/){: new_window}。
2. 從**安全**功能表，選取 **SSL > 訂單**。
3. 針對想要的 SSL 憑證，按一下**更新**直欄中的**更新**鏈結。

   **附註：**會出現一個蹦現方框來完成要求。  
   * 判斷所有更新和 CSR 詳細資料是否正確：<br /><br /><table border="1"><caption>表 1. 更新及 CSR 詳細資料</caption><tr><th>如果...</th><th>則...</th></tr><tr><td>所有更新和 CSR 詳細資料都正確</td><td>繼續進行下一步。</td></tr><tr><td>更新詳細資料不正確</td><td><ul><li>按一下<strong>購買新的 SSL 憑證</strong>鏈結以重新導向至採購畫面。<br /><blockquote><strong>附註：</strong>由於無法變更更新詳細資料，包括憑證類型、管理中心、核准電子郵件，所以更新網站 SSL 憑證詳細資料的唯一方法是訂購新的憑證。</blockquote></li><li>利用 SSL 憑證的所需資訊，完成「訂單」頁面上的畫面。使用此程序不需要任何其他動作。</li></ul></td></tr><tr><td>CSR 詳細資料不正確</td><td><ul><li>按一下**變更 CSR** 按鈕。</li><li>在 **CSR** 文字框中輸入**新的 CSR 詳細資料**。</li><li>按一下**還原 CSR** 按鈕。</li></ul></td></tr></table>
4. 按一下**更新**按鈕以更新 SSL 憑證，或按一下**取消**以取消動作。

## 後續步驟

要求 SSL 憑證的更新之後，{{site.data.keyword.BluSoftlayer_notm}} 會將要求轉遞至憑證管理中心，以便完成更新所需的網站驗證。更新憑證時，新的到期日會出現在「到期」欄位中。
