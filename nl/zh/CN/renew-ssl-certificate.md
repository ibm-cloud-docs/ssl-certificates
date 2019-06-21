---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords:  renewing SSL certificates, renewal SSL, SSL certificate renewal process, renewing, renewal

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 续订 SSL 证书
{: #renewing-ssl-certificates}

通过 {{site.data.keyword.cloud}} 订购 SSL 证书后，可随时续订该证书。在续订过程中，{{site.data.keyword.cloud_notm}} 充当您和认证中心之间的协作者，并且不会查看或控制续订过程中涉及 SSL 证书详细信息的任何部分。SSL 证书根据其订购的相同条款进行续订，因此不能更改续订详细信息（证书类型和认证中心、有效月份、服务器平台等）。可以在到期之前或之后续订证书；但是，要维护 SSL 证书的有效性，请在到期日期之前续订证书。
{:shortdesc}

## 续订 SSL 证书
请完成以下步骤以续订 SSL 证书。

1. 导航至控制台的安全性菜单。有关更多信息，请参阅[导航至设备](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)。
2. 从**安全性**菜单中，选择 **SSL > 订单**。
3. 单击所需 SSL 证书的**续订**列中的**续订**。
4. 在续订 SSL 证书之前，请确定所有续订和 CSR 详细信息是否都正确。请参阅下表以了解更多信息。  

| 详细信息                        | 操作    |
| ------------------------------- | ------- |
| 续订和 CSR 详细信息正确| 选择**续订**以续订 SSL 证书。|
| 续订详细信息不正确     | 选择**购买新 SSL 证书**以订购一个新证书。由于无法更改续订详细信息（包括证书类型、认证中心和核准电子邮件），因此更新 Web 站点 SSL 证书详细信息的唯一方法是订购一个新证书。|
| CSR 详细信息不正确     | 选择**更改 CSR**，在 **CSR 文本框**中输入新 CSR 详细信息，然后选择**复原 CSR**。|
{: caption="表 1. 续订和 CSR 详细信息" caption-side="top"}

## 后续步骤

在请求 SSL 证书续订后，{{site.data.keyword.cloud_notm}} 会将请求转发给认证中心，以便完成续订所需的 Web 站点验证。在续订证书时，新的到期日期将显示在**到期**字段中。
