---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-11"

keywords: types of certificates,SSL certificates, Select Security

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 入门教程
{: #getting-started-tutorial}

## 开始之前

开始使用 SSL 时需要进行一些规划。请完成以下先决条件。

1. 决定在何处获取证书
2. 了解证书类型、密钥长度和持续时间
3. 选择通用名称
4. 了解套接字规则
5. 生成 CSR

有关更多信息，请参阅[规划 SSL 证书](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-planning-for-ssl#planning-for-ssl)。

## 订购 SSL 证书

1. 导航至控制台的安全性菜单。有关更多信息，请参阅[导航至设备](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)。
2. 从**安全性**菜单中，选择**安全性 > SSL > 证书**。
3. 选择**订购 SSL 证书**。
3. 选择证书的类型和持续时间，提交 CSR 的文本，选择服务器平台，然后确认付款。

## 安装和测试
完成订购和验证过程后，您会收到来自认证中心的电子邮件，其中包含您的证书以及任何必要的中间证书。安装方法取决于您使用的软件，但结果应该是相同的。完成后，您应该能够转至 `http://host.yourdomain.com` 并看到您的内容，同时还会看到浏览器用于表示加密会话的 SSL 挂锁。如果收到警告，那么必须执行一些其他步骤。

## 后续步骤

测试成功后，您可以在 {{site.data.keyword.cloud_notm}} 控制台中访问 SSL 证书，以[更新](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates#viewing-and-updating-ssl-certificates)、[下载](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details#downloading-ssl-certificate-details)、[删除](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates)现有 SSL 证书，或者将这些证书[导入](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates)到工具中。
