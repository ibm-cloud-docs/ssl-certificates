---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

<a name="top"></a>
# 常见问题：SSL 证书

## 为什么我所订购的 SSL 证书不会自动显示在 SSL 证书屏幕上？

SSL 证书由第三方认证中心颁发，该认证中心会将所有证书详细信息直接在保密电子邮件中发送给您。接收到该电子邮件后，您可以选择[将 SSL 证书导入](import-ssl-certificate.html)到 {{site.data.keyword.slportal_full}}（如果您选择将证书用于 {{site.data.keyword.BluSoftlayer_full}} 产品和服务的话）。由于我们从不接收 SSL 证书的详细信息，因此无法自动导入此数据。

## 什么是 SSL 证书？

SSL 证书是 Web 站点启用的一种安全措施，用来保护最终用户。通常，当您需要将保密信息（例如，姓名、地址、信用卡号码和其他个人数据）传输到 Web 站点或在管理需要认证的数据（例如，{{site.data.keyword.slportal}} 中的数据）时，可利用 SSL 证书。SSL 证书由运行 Web 站点的公司请求，但由确保 Web 站点的有效性的授信第三方公司颁发。安全 Web 站点的 URL 前面将有 HTTPS 而不是标准的 HTTP。

## 可以如何订购 SHA2 SSL？

如果您已经订购了 SSL，并且显示的错误表明 SSL 证书正在使用 SHA-1 而不是 SHA-2，那么您需要请求重新发出 SSL。您可以通过提交凭单来完成此操作。

如果您尚未向我们订购 SSL，但需要订购一个使用 SHA-2 的 SSL，请提交凭单以针对所讨论的域手动订购 SSL。我们的门户网站仍会自动创建使用 SHA-1 的 SSL 证书，因此您需要重新发出 SSL 证书。
