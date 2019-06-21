---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-11"

keywords: types of certificates,SSL certificates, Select Security

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 入門チュートリアル
{: #getting-started-tutorial}

## 始める前に

SSL を開始するには、多少の計画が必要です。 以下の前提条件を完了してください。

1. 証明書を取得する場所を決定する
2. 証明書のタイプ、鍵の長さ、および期間について学習する
3. 共通名を選択する
4. ソケット・ルールについて学習する
5. CSR を生成する

詳しくは、[SSL 証明書の計画](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-planning-for-ssl#planning-for-ssl)を参照してください。

## SSL 証明書の注文

1. コンソールのセキュリティー・メニューにナビゲートします。詳しくは、[デバイスへのナビゲート](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)を参照してください。
2. **「セキュリティー」**メニューで、**「セキュリティー」>「SSL」>「証明書」**を選択します。
3. **「SSL 証明書の注文 (Order SSL Certificate)」**を選択します。
3. 証明書のタイプと期間を選択し、CSR のテキストを送信し、サーバー・プラットフォームを選択して、支払いを確認します。

## インストールおよびテスト
注文と検証の処理が完了した後、認証局から、証明書と必要な中間証明書が含まれた E メールを受け取ります。 これらのインストール方法は、使用しているソフトウェアによって異なりますが、結果は同じです。 インストールが完了すると、`http://host.yourdomain.com` にアクセスして内容を確認できます。同時に、ブラウザーが暗号化セッションを表示するために使用する SSL パッドロックも確認できます。警告を受けた場合は、実行する必要がある手順が用意されています。

## 次の手順

テストに成功した後、{{site.data.keyword.cloud_notm}} コンソールの SSL 証明書にアクセスして、[更新](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates#viewing-and-updating-ssl-certificates)、[ダウンロード](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details#downloading-ssl-certificate-details)、[削除](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates)、またはツールへの既存の SSL 証明書の[インポート](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates)を行うことができます。
