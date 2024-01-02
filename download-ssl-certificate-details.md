---

copyright:
  years: 2014, 2024
lastupdated: "2024-01-02"

keywords: SSL certificate details, preferred Download Option, SSL certificate download details

subcollection: ssl-certificates

---

{{site.data.keyword.attribute-definition-list}}

# Downloading SSL certificate details
{: #downloading-ssl-certificate-details}

SSL Certificate Order is deprecated. As of 15 April 2024, SSL Certificate Order is no longer available for purchase. As of 15 December 2024,  SSL Certificate Order is no longer supported for new orders or reorders. Only existing certificates that are not expired are still available for you to download, reissue, or revoke. For more information, see [Deprecation of SSL Certificates](/docs/ssl-certificates?topic=ssl-certificates-deprecation).
{: deprecated}

After an SSL certificate is added to the {{site.data.keyword.cloud}} console, its details can be downloaded at any time. Downloads can include the certificate, key or PEM, which includes all available details that are associated with the SSL certificate. SSL certificate details are downloaded securely, so there is no risk that is associated with retrieving the details through this method.
{: shortdesc}

To download details for the SSL certificate, complete the following steps.

1. Navigate to your console's security menu. For more information, see [Navigating to devices](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. From the **Security** menu, select **SSL > Certificates**.
3. From the **Actions** menu, select the preferred **Download Option** for the certificate. Refer to the following table for more information:

| Download Option      | Download Information |
| -------------------- | -------------------- |
| Download certificate | Downloads only the certificate portion, and does not include the private key, intermediate certificate, certificate signing request, or notes details. |
| Download key         | Downloads only the private key, and does not include the certificate, intermediate certificate, certificate signing request, or notes details. |
| Download PEM         | Downloads all details that are associated with the SSL certificate, including the certificate, private key, intermediate certificate, certificate signing request, and notes details. |
{: caption="Table 1. Download options" caption-side="top"}

## Next steps
{: #ns-downloading-ssl-certificate-details}

After requesting the SSL certificate details for download, they are automatically downloaded in the web browser. Select the download to open the file. The file can also be saved to your workstation for future reference; however, data for any SSL certificate present on the SSL certificates screen can be downloaded automatically at any time by repeating the previous steps.

