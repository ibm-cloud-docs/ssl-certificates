---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: view SSL certificates, update SSL certificates, original certificates

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 檢視及更新 SSL 憑證
{: #viewing-and-updating-ssl-certificates}

將 SSL 憑證匯入到 SSL 憑證畫面之後，您可以隨時檢視及更新它。更新的運作類似於[匯入程序](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates)，因為所有更新的詳細資料都必須與原始憑證完全相符，包括間距和換行。
{:shortdesc}

若要檢視及更新 SSL 憑證，請完成下列步驟。

1. 導覽至主控台的安全功能表。如需相關資訊，請參閱[導覽至裝置](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)。
2. 從**安全**功能表，選取 **SSL > 憑證**。
3. 從**動作**下拉清單中，選取**檢視/更新憑證**。
4. 在適合的文字框中更新 **SSL 憑證詳細資料**，然後按一下**更新**以套用您的變更。請參閱下表，以取得相關資訊。

   **匯入 SSL 憑證**視窗中輸入的詳細資料，輸入時必須與憑證管理中心提供的資料完全相同，包括間距和換行。否則會發生錯誤。
   {:note}

|SSL 憑證詳細資料|說明|
| --------------------------- | ----------- |
|憑證|憑證管理中心所提供的 SSL 憑證詳細資料。這通常是一個英數文字區塊。|
|私密金鑰|憑證管理中心所提供的憑證私密金鑰詳細資料。這通常是一個英數文字區塊。|
|中繼憑證|憑證管理中心所提供的中繼憑證詳細資料。中繼憑證不是必要項目，不過如果該資訊可用於 SSL 憑證，則應輸入。|
|憑證簽章要求|憑證管理中心所提供的憑證簽署要求 (CSR) 詳細資料。CSR 詳細資料不是必要項目，但如果它們是憑證的一部分，則應提供。**附註：**請勿以任何方式變更 CSR。公開金鑰可以附在 CSR 且不應該以私密金鑰取代。|
|附註|有關 SSL 憑證，可能有助於其他使用者的任何附註。|
{: caption="表 1. SSL 憑證詳細資料" caption-side="top"}

## 後續步驟

更新 SSL 憑證的詳細資料之後，使用該憑證的任何產品或服務不會受到變更的負面影響。您可以隨時重複先前的步驟，再次更新憑證。
