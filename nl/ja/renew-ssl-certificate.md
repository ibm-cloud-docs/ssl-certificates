---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords:  renewing SSL certificates, renewal SSL, SSL certificate renewal process, renewing, renewal

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL 証明書の更新
{: #renewing-ssl-certificates}

{{site.data.keyword.cloud}} を介して SSL 証明書を注文した後は、いつでも証明書を更新できます。 更新処理中、{{site.data.keyword.cloud_notm}} はユーザーと認証局の間の仲介役として行動し、SSL 証明書の詳細にかかわる更新処理のいかなる部分も見たり制御したりしません。SSL 証明書は、注文時と同じご利用条件に基づいて更新されるため、更新の詳細 (証明書のタイプおよび権限、有効期間の月、サーバー・プラットフォームなど) は変更できません。 証明書は、有効期限の前でも後でも更新できますが、SSL 証明書の有効期間を維持するために、有効期限の前に証明書を更新してください。{:shortdesc}

## SSL 証明書の更新
以下の手順を実行して、SSL 証明書を更新します。

1. コンソールのセキュリティー・メニューにナビゲートします。詳しくは、[デバイスへのナビゲート](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)を参照してください。
2. **「セキュリティー」**メニューで、**「SSL」>「注文」**を選択します。
3. 必要な SSL 証明書の**「更新」**列の**「更新」**をクリックします。
4. SSL 証明書を更新する前に、更新および CSR の詳細がすべて正しいかどうかを判断します。詳しくは、次の表を参照してください。  

| 詳細      | アクション |
| ------------------------------- | ------- |
| 正しい更新および CSR の詳細| **「更新」**を選択して、SSL 証明書を更新します。|
| 正しくない更新の詳細|**「新しい SSL 証明書の購入 (Purchase a new SSL certificate)」**を選択して、新しい証明書を注文します。更新の詳細 (証明書タイプ、権限、承認 E メールなど) は変更できないため、Web サイトの SSL 証明書の詳細を更新する唯一の方法は、新しい証明書を注文することです。|
| 正しくない CSR の詳細| **「CSR の変更 (Change CSR)」**を選択し、**「CSR テキスト・ボックス (CSR text box)」**に新しい CSR の詳細を入力し、**「CSR の復元 (Restore CSR)」**を選択します。|
{: caption="表 1. 更新および CSR の詳細" caption-side="top"}

## 次の手順

SSL 証明書の更新を要求すると、更新に必要な Web サイト検証を実行するために、{{site.data.keyword.cloud_notm}} は要求を認証局に転送します。 証明書が更新されると、**「有効期限」**フィールドに新しい有効期限が表示されます。
