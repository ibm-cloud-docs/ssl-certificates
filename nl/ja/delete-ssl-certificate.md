---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL 証明書の削除

SSL 証明書の詳細を {{site.data.keyword.slportal_full}} にインポートした後、いつでもそれを削除して、すべてのデータが {{site.data.keyword.slportal}} に保存されないようにすることができます。

SSL 証明書を削除するには、以下の手順を実行します。

1. ユーザー固有の資格情報を使用して、[{{site.data.keyword.slportal}} ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://control.softlayer.com/){: new_window} にアクセスします。
2. **「セキュリティー」**メニューで、**「SSL」>「証明書」**を選択します。
3. **「アクション」**メニューで、対象の SSL 証明書の**「削除」**を選択します。

  **注:** 削除を確認するウィンドウが表示されます。
4. SSL 証明書を削除する場合は**「はい」**をクリックし、アクションを取り消す場合は**「いいえ」**をクリックします。

## 次のステップ

SSL 証明書を削除すると、その証明書にリンクされていたすべてのサービスが、その情報を使用しなくなります。その証明書は、{{site.data.keyword.slportal}} 内の SSL 証明書画面に表示されなくなります。

削除された証明書を以前に使用していたすべてのサービスを更新して、アカウントに関連付けられている有効な SSL 証明書に関連付けることをお勧めします。

**注:** いつでも、[インポート](import-ssl-certificate.html)処理を使用して、SSL 証明書を {{site.data.keyword.slportal}} に再度追加することができます。
