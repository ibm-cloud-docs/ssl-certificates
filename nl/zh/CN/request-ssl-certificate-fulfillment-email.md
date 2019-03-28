---

copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"

keywords: SSL certificate fulfillment email, fulfillment email

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 请求 SSL 证书订单履行电子邮件
{: #requesting-an-ssl-certificate-fulfillment-email}

通过 {{site.data.keyword.BluSoftlayer_full}} 订购新 SSL 证书后，认证中心将向订购过程中提供的域管理员发送一封订单履行电子邮件。此电子邮件包含与 SSL 证书相关联的所有详细信息。您可以随时从 {{site.data.keyword.slportal_full}} 上的“SSL 订单”屏幕再次请求订单履行电子邮件。请完成以下步骤，以从认证中心请求 SSL 订单履行电子邮件。

## 请求订单履行电子邮件

1. 使用您的唯一凭证访问 [{{site.data.keyword.slportal_full}} ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://control.softlayer.com/){: new_window}。
2. 从**安全性**菜单中，选择 **SSL > 订单**。
3. 单击所需 SSL 证书的**电子邮件**列中的**发送**链接。<br/>**注：**此时将显示一个弹出窗口，用于确认请求。此窗口包含请求 SSL 证书时提供的域管理员的电子邮件地址。
4. 单击**重新发送电子邮件**以确认选择，并从认证中心请求额外的订单履行电子邮件。或者，单击**取消**以取消操作。

## 后续步骤

请求额外的订单履行电子邮件后，该请求将转发到适用的认证中心以完成。因为 SSL 证书详细信息是保密的，所以 {{site.data.keyword.BluSoftlayer_notm}} 不会在其系统上存储 SSL 证书数据。通过电子邮件接收 SSL 证书详细信息后，如果需要，可以将其手动[导入](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates)到 {{site.data.keyword.slportal}}。
