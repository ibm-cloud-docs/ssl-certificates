---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 续订 SSL 证书

## 概述

通过 {{site.data.keyword.BluSoftlayer_full}} 订购 SSL 证书后，可随时续订该证书。在续订过程中，{{site.data.keyword.BluSoftlayer_notm}} 充当客户（您）和认证中心之间的协作者，并且不会查看或控制涉及 SSL 证书详细信息的任何续订过程部分。SSL 证书根据其订购的相同条款进行续订，因此不会更改续订详细信息（证书类型和认证中心、有效期、服务器平台等）。可以在到期之前或之后续订证书，但是，要维护 SSL 证书的有效性，请在到期日期之前续订证书。请遵循以下步骤以续订 SSL 证书。

## 续订 SSL 证书

1. 使用您的唯一凭证访问 [{{site.data.keyword.slportal_full}} ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://control.softlayer.com/){: new_window}。
2. 从**安全性**菜单中，选择 **SSL > 订单**。
3. 单击所需 SSL 证书的**续订**列中的**续订**链接。

   **注：**此时将显示一个弹出框，用于完成请求。  
   * 确定所有更新和 CSR 详细信息都正确：<br /><br /><table border="1"><tr><th>如果...</th><th>那么...</th></tr><tr><td>所有续订和 CSR 详细信息都正确</td><td>继续下一步。</td></tr><tr><td>续订详细信息不正确</td><td><ul><li>单击<strong>购买新 SSL 证书</strong>链接以重定向到采购屏幕。<br /><blockquote><strong>注：</strong>由于无法更改续订详细信息（包括证书类型、认证中心和核准电子邮件），因此更新 Web 站点 SSL 证书详细信息的唯一方法是订购一个新证书。</blockquote></li><li>使用 SSL 证书的所需信息完成“订单”页面上的屏幕。使用此过程无需执行其他操作。</li></ul></td></tr><tr><td>CSR 详细信息不正确</td><td><ul><li>单击**更改 CSR** 按钮。</li><li>在 **CSR** 文本框中输入**新 CSR 详细信息**。</li><li>单击**复原 CSR** 按钮。</li></ul></td></tr></table>
4. 单击**续订**按钮以续订 SSL 证书，或单击**取消**以取消操作。

## 后续步骤

在请求 SSL 证书续订后，{{site.data.keyword.BluSoftlayer_notm}} 会将请求转发给认证中心，以完成续订所需的 Web 站点验证。在续订证书时，新的到期日期将显示在“到期”字段中。
