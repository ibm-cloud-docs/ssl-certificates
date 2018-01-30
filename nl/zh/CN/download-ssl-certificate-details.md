---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-17"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 下载 SSL 证书详细信息

## 概述

将 SSL 证书添加到 {{site.data.keyword.slportal_full}} 后，可随时下载其详细信息。下载可能包含证书、密钥或 PEM，其中包括与 SSL 证书相关联的所有可用详细信息。SSL 证书详细信息可安全下载，因此通过此方法不存在与检索详细信息相关联的风险。

要下载 SSL 证书的详细信息，请完成以下步骤。

## 下载 SSL 证书详细信息

1. 使用您的唯一凭证访问 [{{site.data.keyword.slportal_full}} ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://control.softlayer.com/){: new_window}。
2. 从**安全性**菜单中，选择 **SSL > 证书**。
3. 从**操作**菜单中，为证书选择所需的**下载选项**。请参阅下表以了解更多信息：<br /> <br /><table border="1"><tr><th>下载选项</th><th>已下载的信息</th></tr><tr><td>下载证书</td><td>仅下载证书部分，并且不包含专用密钥、中间证书、证书签名请求或注释详细信息。</td></tr><tr><td>下载密钥</td><td>仅下载专用密钥，并且不包含证书、中间证书、证书签名请求或注释详细信息。</td></tr><tr><td>下载 PEM</td><td>下载与 SSL 证书相关联的所有详细信息，包括证书、专用密钥、中间证书、证书签名请求和注释。</td></tr></table>

## 后续步骤

在请求下载 SSL 证书详细信息之后，会在 Web 浏览器中自动下载这些详细信息。单击下载以打开文件。还可以将该文件保存到工作站以供将来参考；但是，通过重复上述步骤，可以随时自动下载 SSL 证书屏幕上存在的任何 SSL 证书的数据。
