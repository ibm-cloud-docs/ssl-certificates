---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: importing SSL certificates,SSL import, SSL certificate details

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 导入 SSL 证书
{: #importing-ssl-certificates}

为 Web 站点签发 SSL 证书后，可以将其导入到 {{site.data.keyword.cloud}} 控制台。通过将 SSL 证书导入到 {{site.data.keyword.cloud_notm}} 控制台中，可以将证书应用于可能需要这些证书的产品和服务，例如，负载均衡器的 [SSL 卸载](/docs/infrastructure/local-load-balancer?topic=local-load-balancer-configuring-ssl-offloading-on-a-load-balancer)。缺省情况下，不会将 {{site.data.keyword.cloud_notm}} 所发出的 SSL 证书导入到列表中，因为这些证书仅供接收方处理。因此，任何与 {{site.data.keyword.cloud_notm}} 产品或服务配合使用的 SSL 证书都必须由帐户上的授权用户手动导入。
{:shortdesc}

## 导入 SSL 证书

请完成以下步骤以导入 SSL 证书。

1. 导航至控制台的安全性菜单。有关更多信息，请参阅[导航至设备](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)。
2. 从**安全性**菜单中，选择 **SSL > 证书**。
3. 单击**导入 SSL 证书**。
4. 在适用字段中输入 **SSL 证书详细信息**，然后单击**导入**。请参阅下表以了解更多信息。

   在**导入 SSL 证书**窗口中输入的详细信息必须严格按照认证中心提供的方式输入，包括间隔和换行情况。否则，将发生错误。
   {:note}

|SSL 证书详细信息      | 描述 |
| --------------------------- | ----------- |
|证书|SSL 证书详细信息，由认证中心提供。这通常是字母数字的文本块。|
|专用密钥|证书的专用密钥详细信息，由认证中心提供。这通常是字母数字的文本块。|
|中间证书|中间证书详细信息，由认证中心提供。中间证书不是必需的，但是如果该信息可用于 SSL 证书，那么应该输入中间证书。|
|证书签名请求|证书签名请求 (CSR) 详细信息，由认证中心提供。CSR 详细信息不是必需的，但如果是证书的一部分，那么应提供这些信息。**注：**请勿以任何方式更改 CSR。公用密钥可能随附于 CSR 中，不应由专用密钥替换。|
|注释|可能对其他用户有帮助的有关 SSL 证书的任何注释。|
{: caption="表 1. SSL 证书详细信息" caption-side="top"}

## 后续步骤

在将 SSL 证书导入到 {{site.data.keyword.cloud_notm}} 控制台之后，它将存储在“SSL 证书”屏幕上，直到
[手动删除](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates)为止。对于所有需要 SSL 证书详细信息的产品或服务，新的 SSL 证书将显示在可用证书列表中，以供在与所需产品或服务的 SSL 功能交互时使用。证书可能已[更新](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates)，并且有关证书的详细信息可以随时[安全下载](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details)。
