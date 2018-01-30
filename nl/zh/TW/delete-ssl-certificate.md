---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-17"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 刪除 SSL 憑證

## 概觀

將 SSL 憑證的詳細資料匯入到 {{site.data.keyword.slportal_full}} 之後，您可以隨時刪除它，以避免將所有資料儲存至 {{site.data.keyword.slportal}}。

若要刪除 SSL 憑證，請完成下列步驟。

## 刪除 SSL 憑證

1. 使用您的唯一認證來存取 [{{site.data.keyword.slportal}} ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/){: new_window}。
2. 從**安全**功能表，選取 **SSL > 憑證**。
3. 從**動作**功能表，針對想要的 SSL 憑證選取**刪除**。

  **附註：**會出現一個視窗，以確認刪除。
4. 按一下**是**以刪除 SSL 憑證，或按一下**否**以取消動作。

## 後續步驟

刪除 SSL 憑證之後，鏈結至該憑證的所有服務將不再利用其資訊。憑證不會再出現在 {{site.data.keyword.slportal}} 的 SSL 憑證畫面中。

建議您更新先前使用被刪除之憑證的所有服務，以建立服務和與帳戶相關聯之有效 SSL 憑證之間的關聯。

**附註：**隨時都可以利用[匯入](import-ssl-certificate.html)程序，將 SSL 憑證新增回 {{site.data.keyword.slportal}}。
