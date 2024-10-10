---

copyright:
  years: 2014, 2024
lastupdated: "2024-07-17"
keywords: importing SSL certificates,SSL import, SSL certificate details

subcollection: ssl-certificates

---

{{site.data.keyword.attribute-definition-list}}

# Importing SSL certificates
{: #importing-ssl-certificates}

SSL Certificate Order is deprecated. As of 15 April 2024, SSL Certificate Order is no longer available for purchase. As of 15 December 2024, SSL Certificate Order is no longer supported for new orders or reorders. Only existing certificates that are not expired are still available for you to download, reissue, or revoke. For more information, see [Deprecation of SSL Certificates](/docs/ssl-certificates?topic=ssl-certificates-deprecation).
{: deprecated}

After an SSL certificate is issued for a website, it can be imported into the {{site.data.keyword.cloud}} console. By importing SSL certificates into the {{site.data.keyword.cloud_notm}} console, the certificates can be applied to products and services that might require them, such as Load Balancer's SSL offloading. By default, SSL certificates that are issued by {{site.data.keyword.cloud_notm}} are not imported into the list, as they are intended to be manipulated by the recipient only. Therefore, any SSL certificate that is used with an {{site.data.keyword.cloud_notm}} product or service must be manually imported by an authorized user on the account.
{: shortdesc}

## Importing SSL certificates
{: #importing-ssl-certificates-steps}

Complete the following steps to import an SSL certificate.

1. Go to your console's security menu. For more information, see [Navigating to devices](/docs/ssl-certificates?topic=ssl-certificates-navigating-devices).
2. From the **Security** menu, select **SSL > Certificates**.
3. Click **Import SSL Certificate**.
4. Enter the **SSL certificate details** in the applicable fields and click **Import.** See the following table for more information.

   Details that are entered in the **Import SSL Certificate** window must be entered exactly as provided by the certificate authority, including spacing and line breaks. If not, an error occurs.
   {: note}

| SSL Certificate Details     | Description |
| --------------------------- | ----------- |
|Certificate                  | SSL certificate details are provided by the certificate authority and are generally an alpha-numeric block of text.|
|Private key                  | Private key details for the certificate are provided by the certificate authority and are generally an alpha-numeric block of text.|
|Intermediate certificate     | Intermediate certificate details are provided by the certificate authority. Intermediate certificates are not required; however, if the information is available for the SSL certificate, it must be entered.|
|Certificate signing request  | Certificate signing request (CSR) details provided by the certificate authority. CSR details are not required, but must be provided if they are part of the certificate. **Note:** Do not change the CSR in any way. A public key can be included with the CSR and must not be replaced by the Private Key.|
|Notes                        | Any notes about the SSL certificate that might be helpful to other users.|
{: caption="SSL certificate details" caption-side="top"}

## Next steps
{: #ns-importing-ssl-certificates}

After the SSL certificate is imported to the {{site.data.keyword.cloud_notm}} console, it is stored on the SSL certificates screen until it is [manually deleted](/docs/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates). For all products or services that require SSL certificate details, the new SSL certificate appears in the list of available certificates for use when you interact with the SSL feature for the wanted product or service. The certificate can be [updated](/docs/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates) and details about the certificate can be [securely downloaded](/docs/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details) at any time.
