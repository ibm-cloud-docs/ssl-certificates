---
copyright:
  years: 2014, 2018
lastupdated: "2018-06-20"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL 証明書のインポート

Web サイトに対して SSL 証明書が発行された後、その証明書を {{site.data.keyword.slportal_full}} にインポートできます。 SSL 証明書を {{site.data.keyword.slportal}} にインポートすると、証明書を必要とする可能性がある製品やサービス (ロード・バランサーの [SSL オフロード](/docs/infrastructure/local-load-balancer/configure-ssl-offloading-load-balancer.html){:new_window}など) に適用できます。 デフォルトでは、{{site.data.keyword.BluSoftlayer_full}} で発行された SSL 証明書は、受信者による操作のみを意図しているため、リストにインポートされません。 そのため、{{site.data.keyword.BluSoftlayer_notm}} 製品やサービスで使用する SSL 証明書は、アカウント上で権限のあるユーザーが手動でインポートする必要があります。 以下の手順を実行して、{{site.data.keyword.slportal}} に SSL 証明書をインポートします。

1. ユーザー固有の資格情報を使用して、[{{site.data.keyword.slportal_full}} ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://control.softlayer.com/){: new_window} にアクセスします。
2. **「セキュリティー」**メニューで、**「SSL」>「証明書」**を選択します。
3. **「SSL 証明書のインポート」**をクリックします。
4. アプリケーション・フィールドに **SSL 証明書の詳細**を入力して、**「インポート」**をクリックします。

   **注:** **「SSL 証明書のインポート」**ウィンドウに入力される詳細は、スペーシングや改行を含めて、認証局によって指定されたとおり正確に入力する必要があります。 そうしないと、エラーが発生します。

| SSL 証明書の詳細 | 説明 |
| --------------------------- | ----------- |
|証明書                  | 認証局によって提供される SSL 証明書の詳細。これは通常、英数字のテキスト・ブロックです。|
|秘密鍵                  | 認証局によって提供される、証明書の秘密鍵の詳細。これは通常、英数字のテキスト・ブロックです。|
|中間証明書     | 認証局によって提供される中間証明書の詳細。中間証明書は必須ではありませんが、その SSL 証明書に関する情報が使用可能である場合は、入力する必要があります。|
|証明書署名要求  | 認証局によって提供される、証明書署名要求 (CSR) の詳細。CSR の詳細は必須ではありませんが、証明書の一部である場合は、指定する必要があります。 **注:** CSR は絶対に変更しないでください。 公開鍵が CSR に含まれている場合があり、秘密鍵で置き換えてはなりません。|
|メモ                        | 他のユーザーに役立つ可能性がある、SSL 証明書に関するメモ。|
{: caption="表 1. SSL 証明書の詳細" caption-side="top"}

## 次のステップ

SSL 証明書が {{site.data.keyword.slportal}} にインポートされた後、その証明書は[手動で削除](delete-ssl-certificate.html)されるまで、SSL 証明書画面に保管されます。 SSL 証明書の詳細を必要とするすべての製品やサービスのために、新しい SSL 証明書は、使用可能な証明書のリストに表示され、必要な製品やサービスの SSL 機能との対話に使用されます。 いつでも、証明書を[更新](view-and-update-ssl-certificate.html)し、証明書に関する詳細を[安全にダウンロード](download-ssl-certificate-details.html)できます。
