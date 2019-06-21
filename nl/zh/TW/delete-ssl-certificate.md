---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificates delete, SSL delete

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 刪除 SSL 憑證
{: #deleting-ssl-certificates}

將 SSL 憑證的詳細資料匯入到 {{site.data.keyword.cloud}} 主控台之後，您可以隨時刪除它，以避免將所有資料儲存至 {{site.data.keyword.cloud_notm}} 主控台。

若要刪除 SSL 憑證，請完成下列步驟。

1. 導覽至主控台的安全功能表。如需相關資訊，請參閱[導覽至裝置](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)。
2. 從**安全**功能表，選取 **SSL > 憑證**。
3. 從**動作**功能表，針對想要的 SSL 憑證選取**刪除**。
4. 按一下**是**以刪除 SSL 憑證。

## 後續步驟

刪除 SSL 憑證之後，鏈結至該憑證的所有服務便不再使用其資訊。憑證不會再出現在 {{site.data.keyword.cloud_notm}} 主控台的 SSL 憑證畫面中。

更新先前使用被刪除之憑證的所有服務，以建立服務和與帳戶相關聯之有效 SSL 憑證之間的關聯。

隨時都可以利用[匯入](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates)處理程序，將 SSL 憑證新增回到 {{site.data.keyword.cloud_notm}} 主控台。
{:note}
