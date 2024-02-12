---

copyright:
  years: 2014, 2024
lastupdated: "2024-02-12"

keywords: SSL certificate fulfillment email, fulfillment email

subcollection: ssl-certificates

---

{{site.data.keyword.attribute-definition-list}}

# Requesting an SSL certificate fulfillment email
{: #requesting-an-ssl-certificate-fulfillment-email}

SSL Certificate Order is deprecated. As of 15 April 2024, SSL Certificate Order is no longer available for purchase. As of 15 December 2024,  SSL Certificate Order is no longer supported for new orders or reorders. Only existing certificates that are not expired are still available for you to download, reissue, or revoke. For more information, see [Deprecation of SSL Certificates](/docs/ssl-certificates?topic=ssl-certificates-deprecation).
{: deprecated}

After ordering a new SSL certificate through {{site.data.keyword.cloud}}, the certificate authority sends a fulfillment email to the domain administrator provided during the ordering process. This email contains all details that are associated with the SSL certificate. At any time, the fulfillment email can be requested again from the SSL Orders screen on the {{site.data.keyword.cloud_notm}} console.
{: shortdesc}

## Requesting a fulfillment email
Complete the following steps to request the SSL fulfillment email from the certificate authority.

1. Go to your console's security menu. For more information, see [Navigating to devices](/docs/ssl-certificates?topic=ssl-certificates-navigating-devices).
2. From the **Security** menu, select **SSL > Orders**.
3. Click **Send** in the **Email** column for the SSL certificate that you want.

    A pop-up window appears to confirm the request. This window contains the email address for the domain administrator that was provided when the SSL certificate was requested.
    {: note}

4. Click **Resend Email** to confirm the selection and request an additional fulfillment email from the certificate authority.

## Next steps
{: #ns-requesting-an-ssl-certificate-fulfillment-email}

After you request an additional fulfillment email, the request is forwarded to the applicable certificate authority for completion. Because SSL certificate details are confidential, {{site.data.keyword.cloud_notm}} does not store the SSL certificate data on its system. After you receive the SSL certificate details by email, they can be manually [imported](/docs/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates) to the {{site.data.keyword.cloud_notm}} console, if necessary.
