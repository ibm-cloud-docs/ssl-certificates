---


copyright:
  years: 2014, 2018
lastupdated: "2018-05-17"

keywords: SSL certificate details, preferred Download Option, SSL certificate download details

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 下載 SSL 憑證詳細資料
{: #downloading-ssl-certificate-details}

將 SSL 憑證新增至 {{site.data.keyword.slportal_full}} 之後，即可隨時下載其詳細資料。下載可包括憑證、金鑰或 PEM，其中包括所有與 SSL 憑證相關聯的可用詳細資料。SSL 憑證詳細資料會安全地下載，因此透過此方法擷取詳細資料不會有相關聯的風險。

若要下載 SSL 憑證的詳細資料，請完成下列步驟。

1. 使用您的唯一認證來存取 [{{site.data.keyword.slportal_full}} ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/){: new_window}。
2. 從**安全**功能表，選取 **SSL > 憑證**。
3. 從**動作**功能表，針對憑證選取偏好的**下載選項**。如需相關資訊，請參閱下表：

|下載選項|下載資訊|
| -------------------- | -------------------- |
|下載憑證|只下載憑證部分，不包括私密金鑰、中繼憑證、憑證簽署要求或附註詳細資料。|
|下載金鑰|只下載私密金鑰，不包括憑證、中繼憑證、憑證簽署要求或附註詳細資料。|
|下載 PEM|下載與 SSL 憑證相關聯的所有詳細資料，包括憑證、私密金鑰、中繼憑證、憑證簽署要求和附註。|
{: caption="表 1. 下載選項" caption-side="top"}

## 後續步驟

要求下載的 SSL 憑證詳細資料之後，會自動在 Web 瀏覽器中下載它們。請選取「下載」以開啟檔案。檔案也可以儲存至您的工作站以供日後參考；不過，可以隨時重複先前的步驟，自動下載 SSL 憑證畫面上存在之任何 SSL 憑證的資料。
