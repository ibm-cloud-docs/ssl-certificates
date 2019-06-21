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

# SSL 証明書の完了 E メールの要求
{: #requesting-an-ssl-certificate-fulfillment-email}

{{site.data.keyword.cloud}} を通じて新規 SSL 証明書を注文すると、認証局は、注文プロセスで入力されたドメイン管理者に、完了 E メールを送信します。 この E メールには、SSL 証明書に関連したすべての詳細が含まれます。 {{site.data.keyword.cloud_notm}} コンソールの「SSL 注文」画面から、いつでも完了 E メールを再要求できます。{:shortdesc}

## 完了 E メールの要求
以下の手順を実行して、認証局からの SSL 完了 E メールを要求します。

1. コンソールのセキュリティー・メニューにナビゲートします。詳しくは、[デバイスへのナビゲート](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)を参照してください。
2. **「セキュリティー」**メニューで、**「SSL」>「注文」**を選択します。
3. 必要な SSL 証明書の**「E メール」**列の**「送信」**をクリックします。

  要求を確認するポップアップ・ウィンドウが表示されます。このウィンドウには、SSL 証明書を要求するときに入力されたドメイン管理者の E メール・アドレスが入っています。{:note}

4. **「E メールの再送」**をクリックし、選択内容を確認して、認証局からの追加の完了 E メールを要求します。

## 次の手順

追加の完了 E メールを要求すると、要求は、完了のために当該認証局に転送されます。 SSL 証明書の詳細は機密であるため、{{site.data.keyword.cloud_notm}} はシステム上に SSL 証明書データを保管しません。 E メールで SSL 証明書の詳細を受け取った後、必要に応じて、手動で {{site.data.keyword.cloud_notm}} コンソールに[ インポート](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates)できます。
