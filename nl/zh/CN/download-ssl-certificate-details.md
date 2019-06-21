---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificate details, preferred Download Option, SSL certificate download details

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 下载 SSL 证书详细信息
{: #downloading-ssl-certificate-details}

将 SSL 证书添加到 {{site.data.keyword.cloud}} 控制台后，可随时下载其详细信息。下载可能包含证书、密钥或 PEM，其中包括与 SSL 证书相关联的所有可用详细信息。SSL 证书详细信息将安全下载，因此通过此方法检索详细信息不会带来风险。
{:shortdesc}

要下载 SSL 证书的详细信息，请完成以下步骤。

1. 导航至控制台的安全性菜单。有关更多信息，请参阅[导航至设备](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)。
2. 从**安全性**菜单中，选择 **SSL > 证书**。
3. 从**操作**菜单中，为证书选择首选的**下载选项**。请参阅下表以了解更多信息：

|下载选项|下载信息|
| -------------------- | -------------------- |
|下载证书|仅下载证书部分，并且不包含专用密钥、中间证书、证书签名请求或注释详细信息。|
|下载密钥|仅下载专用密钥，并且不包含证书、中间证书、证书签名请求或注释详细信息。|
|下载 PEM|下载与 SSL 证书相关联的所有详细信息，包括证书、专用密钥、中间证书、证书签名请求和注释详细信息。|
{: caption="表 1. 下载选项" caption-side="top"}

## 后续步骤

在请求下载 SSL 证书详细信息之后，会在 Web 浏览器中自动下载这些详细信息。选择“下载”以打开文件。还可以将该文件保存到工作站以供将来参考；但是，通过重复上述步骤，可以随时自动下载“SSL 证书”屏幕上存在的任何 SSL 证书的数据。

