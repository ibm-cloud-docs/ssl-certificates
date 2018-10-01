---
copyright:
  years: 2014, 2018
lastupdated: "2018-08-15"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 入門チュートリアル  


## 始める前に

SSL を開始するには、多少の計画が必要です。 以下の前提条件を完了してください。

1. 証明書を取得する場所を決定する
2. 証明書のタイプ、鍵の長さ、および期間について学習する
3. 共通名を選択する
4. ソケット・ルールについて学習する
5. CSR を生成する

詳しくは、[SSL 証明書の計画](planning-ahead-ssl.html)を参照してください。

## SSL 証明書の注文

1. ユーザー固有の資格情報を使用して、[{{site.data.keyword.slportal_full}} ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://control.softlayer.com/){: new_window} にアクセスします。
2. **「セキュリティー」>「SSL 証明書」>**を選択して、SSL 証明書画面にアクセスします。
3. 証明書のタイプと期間を選択し、CSR のテキストを送信し、いくつかの追加詳細を入力して、支払いを確認する必要があります。

## インストールおよびテスト
注文と検証の処理が完了した後、認証局から、証明書と必要な中間証明書が含まれた E メールを受け取ります。 これらのインストール方法は、使用しているソフトウェアによって異なりますが、結果は同じです。 インストールが完了すると、<http://host.yourdomain.com> にアクセスして内容を確認できます。同時に、ブラウザーが暗号化セッションを表示するために使用する SSL パッドロックも確認できます。 警告を受けた場合は、実行する必要がある手順が用意されています。

## 次のステップ

テストに成功した後、SSL 証明書画面にアクセスして、[更新](view-and-update-ssl-certificate.html)、[ダウンロード](download-ssl-certificate-details.html)、[削除](delete-ssl-certificate.html)、またはツールへの既存の SSL 証明書の[インポート](import-ssl-certificate.html)を行うことができます。
