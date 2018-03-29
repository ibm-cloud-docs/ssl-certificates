---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 删除 SSL 证书

在将 SSL 证书的详细信息导入到 {{site.data.keyword.slportal_full}} 中之后，可以随时将其删除，以防止将所有数据保存到 {{site.data.keyword.slportal}}中。

要删除 SSL 证书，请完成以下步骤。

1. 使用您的唯一凭证访问 [{{site.data.keyword.slportal}} ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://control.softlayer.com/){: new_window}。
2. 从**安全性**菜单中，选择 **SSL > 证书**。
3. 从**操作**菜单中，针对所需的 SSL 证书，选择**删除**。

  **注：**此时将显示一个窗口以确认删除。
4. 单击**是**以删除 SSL 证书，或者单击**否**以取消操作。

## 后续步骤

删除 SSL 证书后，链接到该证书的所有服务将不再使用其信息。该证书将不会再显示在 {{site.data.keyword.slportal}} 的 SSL 证书屏幕上。

建议您将先前使用已删除证书的所有服务更新为与帐户关联的有效 SSL 证书相关联。

**注：**您可以随时使用[导入](import-ssl-certificate.html)过程将 SSL 证书添加回 {{site.data.keyword.slportal}}。
