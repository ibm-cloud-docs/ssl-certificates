---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: PPTP VPN access, PPTP VPN, PPTP access

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:external: target="_blank" .external}

# PPTP VPN アクセスのアクティブ化または非アクティブ化
{: #activating-or-deactivating-pptp-vpn-access}

PPTP VPN により、デスクトップまたは専用デバイスで実行される特殊なクライアント・ソフトウェアを使用して、{{site.data.keyword.cloud}} プライベート・ネットワークへのセキュア・トンネルを形成できます。PPTP アクセスは、オフィス全体を接続する必要がある場合、または SSL VPN ソリューションを使用できない場合に対応するよう設計されています。1 つの PPTP 接続が割り当てられますが、複数の接続を利用することが可能です。無制限の PPTP アクセス権限を有効にするようにサポートに要求することができます。これは追加料金なしで提供されます。ユーザーのために PPTP VPN アクセスをアクティブ化または非アクティブ化するには、以下の手順を実行します。{:shortdesc}

1. {{site.data.keyword.cloud_notm}} コンソールの[「アクセス (IAM)」](https://cloud.ibm.com/iam/overview){: external}ページにログインします。
2. アクセス権限を変更するユーザーを見つけて、**「VPN アクセス」**列を表示し、現在のアクセス・レベルを確認します。
3. **「アクション」**メニューで、**「VPN のアクセス権限の編集」**を選択します。
4. VPN タイプとサブネット・アクセスの詳細を入力し、**「保存」**をクリックして、変更内容を保存します。詳しくは、次の表を参照してください。

|フィールド名  |オプション   |
| -----------| ------------ |
| VPN タイプ   | なし、SSL、PPTP、または両方 (SSL と PPTP) |
|サブネット・アクセス | 自動または手動 |           
{: caption="表 1. VPN とサブネットの詳細" caption-side="top"}   

ユーザーが PPTP を使用して接続するには、PPTP アクセスをアクティブにする必要があります。{:note}
