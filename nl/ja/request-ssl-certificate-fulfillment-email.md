---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL 証明書の完了 E メールの要求

## 概説

{{site.data.keyword.BluSoftlayer_full}} に新規 SSL 証明書を注文すると、認証局は、注文プロセスで入力されたドメイン管理者に、完了 E メールを送信します。この E メールには、SSL 証明書に関連したすべての詳細が含まれています。{{site.data.keyword.slportal_full}} の「SSL 注文」画面から、いつでも完了 E メールを再要求できます。以下の手順に従って、認証局からの SSL 完了 E メールを要求します。

## 完了 E メールの要求

1. ユーザー固有の資格情報を使用して、[{{site.data.keyword.slportal_full}} ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://control.softlayer.com/){: new_window} にアクセスします。
2. **「セキュリティー」**メニューで、**「SSL」>「注文」**を選択します。
3. 必要な SSL 証明書の**「E メール」**列の**「送信」**リンクをクリックします。<br/>**注:** 要求を確認するポップアップ・ウィンドウが表示されます。このウィンドウには、SSL 証明書を要求するときに入力されたドメイン管理者の E メール・アドレスが入っています。
4. **「E メールの再送」**ボタンをクリックし、選択内容を確認して、認証局からの追加の完了 E メールを要求します。あるいは、**「キャンセル」**をクリックして、アクションを取り消します。

## 次のステップ

追加の完了 E メールを要求すると、要求は、完了のために当該認証局に転送されます。SSL 証明書の詳細は機密であるため、{{site.data.keyword.BluSoftlayer_notm}} はシステム上に SSL 証明書データを保管しません。E メールで SSL 証明書の詳細を受け取った後、必要に応じて、手動で {{site.data.keyword.slportal}} に[インポート](import-ssl-certificate.html)できます。
