---

copyright:
  years: 2014, 2019
lastupdated: "2019-08-26"

keywords: SSL certificate fulfillment email, fulfillment email

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Requesting an SSL certificate fulfillment email
{: #requesting-an-ssl-certificate-fulfillment-email}

After ordering a new SSL certificate through {{site.data.keyword.cloud}}, the certificate authority sends a fulfillment email to the domain administrator provided during the ordering process. This email contains all details that are associated with the SSL certificate. At any time, the fulfillment email can be requested again from the SSL Orders screen on the {{site.data.keyword.cloud_notm}} console.
{:shortdesc}

## Requesting a fulfillment email
Complete the following steps to request the SSL fulfillment email from the certificate authority.

1. Navigate to your console's security menu. For more information, see [Navigating to devices](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. From the **Security** menu, select **SSL > Orders**.
3. Click **Send** in the **Email** column for the SSL certificate that you want.

  A pop-up window appears to confirm the request. This window contains the email address for the domain administrator that was provided when the SSL certificate was requested.
  {:note}

4. Click **Resend Email** to confirm the selection and request an additional fulfillment email from the certificate authority.

## Next steps
{: #ns-requesting-an-ssl-certificate-fulfillment-email}

After requesting an additional fulfillment email, the request will be forwarded to the applicable certificate authority for completion. Because SSL certificate details are confidential, {{site.data.keyword.cloud_notm}} does not store the SSL certificate data on its system. After receiving the SSL certificate details by email, they can be manually [imported](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates) to the {{site.data.keyword.cloud_notm}} console, if necessary.
