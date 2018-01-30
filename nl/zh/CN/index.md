---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-30"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL 证书入门  


## 开始之前

开始使用 SSL 时需要进行一些规划。请完成以下先决条件。

1. 决定在何处获取证书
2. 了解证书类型、密钥长度和持续时间
3. 选择通用名称
4. 了解套接字规则
5. 生成 CSR

有关更多信息，请参阅[规划 SSL 证书](planning-ahead-ssl.html)。

## 订购 SSL 证书

1. 使用唯一凭证访问 [{{site.data.keyword.slportal}} ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://control.softlayer.com/){: new_window}。
2. 选择**安全性 > SSL 证书 >**以访问 SSL 证书屏幕。
3. 必须选择证书的类型和持续时间、提交 CSR 的文本、填写一些其他详细信息，然后确认付款。

## 安装和测试
完成订购和验证过程后，您会收到来自认证中心的电子邮件，其中包含您的证书以及任何必要的中间证书。安装这些证书方法将取决于您使用的软件，但最终结果应该是相同的。完成后，您应该能够访问 <http://host.yourdomain.com> 并可查看您的内容，同时还可以查看浏览器用于表示加密会话的 SSL 挂锁。如果收到警告，那么必须执行一些其他步骤。

## 后续步骤

测试成功后，您可以访问 SSL 证书屏幕，以[更新](view-and-update-ssl-certificate.html)、[下载](download-ssl-certificate-details.html)、[删除](delete-ssl-certificate.html)现有 SSL 证书，或者将这些证书[导入](import-ssl-certificate.html)到工具中。
