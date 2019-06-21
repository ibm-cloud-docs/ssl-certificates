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

# SSL 証明書の削除
{: #deleting-ssl-certificates}

SSL 証明書の詳細を {{site.data.keyword.cloud}} コンソールにインポートした後、いつでもそれを削除して、すべてのデータが {{site.data.keyword.cloud_notm}} コンソールに保存されないようにすることができます。

SSL 証明書を削除するには、以下の手順を実行します。

1. コンソールのセキュリティー・メニューにナビゲートします。詳しくは、[デバイスへのナビゲート](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)を参照してください。
2. **「セキュリティー」**メニューで、**「SSL」>「証明書」**を選択します。
3. **「アクション」**メニューで、対象の SSL 証明書の**「削除」**を選択します。
4. **「はい」**をクリックして SSL 証明書を削除します。

## 次の手順

SSL 証明書を削除すると、その証明書にリンクされていたすべてのサービスが、その情報を使用しなくなります。 その証明書は、{{site.data.keyword.cloud_notm}} コンソール内の SSL 証明書画面に表示されなくなります。

削除された証明書を以前に使用していたすべてのサービスを更新して、アカウントに関連付けられている有効な SSL 証明書に関連付けます。

いつでも、[インポート](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates)処理を使用して、SSL 証明書を {{site.data.keyword.cloud_notm}} コンソールに再度追加することができます。{:note}
