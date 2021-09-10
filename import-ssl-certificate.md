---

copyright:
  years: 2014, 2019
lastupdated: "2019-08-26"

keywords: importing SSL certificates,SSL import, SSL certificate details

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Importing SSL certificates
{: #importing-ssl-certificates}

After an SSL certificate is issued for a website, it can be imported into the {{site.data.keyword.cloud}} console. By importing SSL certificates into the {{site.data.keyword.cloud_notm}} console, the certificates can be applied to products and services that might require them, such as Load Balancer's [SSL offloading](/docs/infrastructure/local-load-balancer?topic=local-load-balancer-configuring-ssl-offloading-on-a-load-balancer). By default, SSL certificates that are issued by {{site.data.keyword.cloud_notm}} are not imported into the list, as they are intended to be manipulated by the recipient only. Therefore, any SSL certificate used with an {{site.data.keyword.cloud_notm}} product or service must be manually imported by an authorized user on the account.
{: shortdesc}

## Importing SSL certificates
{: #importing-ssl-certificates-steps}

Complete the following steps to import an SSL certificate.

1. Navigate to your console's security menu. For more information, see [Navigating to devices](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. From the **Security** menu, select **SSL > Certificates**.
3. Click **Import SSL Certificate**.
4. Enter the **SSL certificate details** in the applicable fields and click **Import.** See the following table for more information.

   Details that are entered in the **Import SSL Certificate** window must be entered exactly as provided by the certificate authority, including spacing and line breaks. If not, an error occurs.
   {: note}

| SSL Certificate Details     | Description |
| --------------------------- | ----------- |
|Certificate                  | SSL certificate details, provided by the certificate authority. This is generally an alpha-numeric block of text.|
|Private key                  | Private key details for the certificate, provided by the certificate authority. This is generally an alpha-numeric block of text.|
|Intermediate certificate     | Intermediate certificate details, provided by the certificate authority. Intermediate certificates are not required; however, if the information is available for the SSL certificate, it should be entered.|
|Certificate signing request  | Certificate signing request (CSR) details provided by the certificate authority. CSR details are not required, but should be provided if they are part of the certificate. **Note:** Do not change the CSR in any way. A public key can be included with the CSR and should not be replaced by the Private Key.|
|Notes                        | Any notes regarding the SSL certificate that might be helpful to other users.|
{: caption="Table 1. SSL certificate details" caption-side="top"}

## Next steps
{: #ns-importing-ssl-certificates}

After the SSL certificate is imported to the {{site.data.keyword.cloud_notm}} console, it is stored on the SSL certificates screen until it is [manually deleted](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates). For all products or services requiring SSL certificate details, the new SSL certificate appears in the list of available certificates for use when interacting with the SSL feature for the wanted product or service. The certificate can be [updated](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates) and details about the certificate can be [securely downloaded](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details) at any time.
