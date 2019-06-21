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

# 删除 SSL 证书
{: #deleting-ssl-certificates}

在将 SSL 证书的详细信息导入到 {{site.data.keyword.cloud}} 控制台中之后，可以随时将其删除，以阻止所有数据保存到 {{site.data.keyword.cloud_notm}} 控制台中。

要删除 SSL 证书，请完成以下步骤。

1. 导航至控制台的安全性菜单。有关更多信息，请参阅[导航至设备](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)。
2. 从**安全性**菜单中，选择 **SSL > 证书**。
3. 从**操作**菜单中，针对所需的 SSL 证书，选择**删除**。
4. 单击**是**以删除 SSL 证书。

## 后续步骤

删除 SSL 证书后，链接到该证书的所有服务将不再使用其信息。该证书将不会再显示在 {{site.data.keyword.cloud_notm}} 控制台中的“SSL 证书”屏幕上。

将先前使用已删除证书的所有服务更新为与关联到帐户的有效 SSL 证书相关联。

您可以随时使用[导入](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates)过程将 SSL 证书添加回 {{site.data.keyword.cloud_notm}} 控制台。
{:note}
