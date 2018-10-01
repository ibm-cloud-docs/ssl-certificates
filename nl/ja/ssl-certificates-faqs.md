---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

<a name="top"></a>
# FAQ: SSL 証明書

## 注文した SSL 証明書が自動的に SSL 証明書画面に表示されないのはなぜですか

SSL 証明書は、サード・パーティーの認証局によって発行されます。認証局はすべての証明書の詳細を、機密 E メールでユーザーに直接送信します。 その E メールを受信した後、証明書を {{site.data.keyword.BluSoftlayer_full}} の製品やサービスで使用したい場合は、{{site.data.keyword.slportal_full}} に [SSL 証明書をインポート](import-ssl-certificate.html)することを選択できます。 {{site.data.keyword.cloud_notm}} は SSL 証明書の詳細を受け取ることはないため、データを自動的にインポートすることはできません。

## SSL 証明書とは何ですか

SSL 証明書は、ユーザーを保護するためのセキュリティー手段として、Web サイトによって使用可能にされます。 一般に、名前、住所、クレジット・カード番号、その他の個人データなどの機密情報を Web サイトに送信する必要がある場合や、認証を必要とするデータ ({{site.data.keyword.slportal}} 内など) を管理している場合に使用されます。 SSL 証明書は、Web サイトを稼働する会社によって要求されますが、発行するのは、Web サイトの妥当性を保証する信頼できるサード・パーティーの会社です。 セキュアな Web サイトは、URL の前に、標準の HTTP ではなく HTTPS が付きます。

## SHA2 SSL の注文方法はどのようにするのですか

既に SSL を注文しており、その SSL 証明書が SHA-2 ではなく SHA-1 を使用しているというエラーを示している場合は、SSL の再発行を要求する必要があります。 これは、チケットを送信することで行えます。

{{site.data.keyword.cloud_notm}} からまだ SSL を注文しておらず、SHA-2 を使用した SSL を注文する必要がある場合は、チケットを送信して、対象ドメインの SSL を手動で注文してください。 {{site.data.keyword.slportal}} ではまだ SHA-1 を使用した SSL 証明書を自動的に作成するため、自動的に作成した場合は、再発行が必要になります。
