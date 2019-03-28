---

copyright:
  years: 2014, 2018
lastupdated: "2018-05-17"

keywords: PPTP VPN access, PPTP VPN, PPTP access

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# PPTP VPN アクセスのアクティブ化または非アクティブ化
{: #activating-or-deactivating-pptp-vpn-access}

PPTP VPN により、ユーザーはデスクトップまたは専用デバイスで実行される特殊なクライアント・ソフトウェアを使用して、{{site.data.keyword.BluSoftlayer_full}} プライベート・ネットワークへのセキュア・トンネルを形成できます。 PPTP アクセスは、オフィス全体を接続する必要があるお客様、または SSL VPN ソリューションを使用できないお客様向けに設計されています。 各お客様に 1 つの PPTP 接続が割り当てられ、これは複数の接続が利用可能です。ただし、無制限の PPTP アクセス権限を有効にするようにサポートに要求する必要があります。これは追加料金なしで提供されます。 ユーザーのために PPTP VPN アクセスをアクティブ化または非アクティブ化するには、以下の手順を実行します。

1. 管理者として、ユーザー固有の資格情報を使用して、[{{site.data.keyword.slportal_full}} ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://control.softlayer.com/){: new_window} にアクセスします。
2. アクセス権限を変更するユーザーを見つけて、**「VPN アクセス」**列を表示し、現在のアクセス・レベルを確認します。
3. **「アクション」**メニューで、**「VPN のアクセス権限の編集」**を選択します。
4. VPN タイプとサブネット・アクセスの詳細を入力します。

|フィールド名  |オプション   |
| -----------| ------------ |
| VPN タイプ   | なし、SSL、PPTP、または両方 (SSL と PPTP) |
|サブネット・アクセス | 自動または手動 |           
{: caption="表 1. VPN とサブネットの詳細" caption-side="top"}   
5. **「保存」**をクリックして、変更内容を保存します。

   **注:** ユーザーが PPTP を使用して接続するには、PPTP アクセスをアクティブにする必要があります。
