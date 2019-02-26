---

copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Requesting an SSL certificate fulfillment email

After ordering a new SSL certificate through {{site.data.keyword.BluSoftlayer_full}}, the certificate authority sends a fulfillment email to the domain administrator provided during the ordering process. This email contains all details that are associated with the SSL certificate. At any time, the fulfillment email can be requested again from the SSL Orders screen on the {{site.data.keyword.slportal_full}}. Complete the following steps to request the SSL fulfillment email from the certificate authority.

## Requesting a fulfillment email

1. Access the [{{site.data.keyword.slportal_full}} ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/){: new_window} by using your unique credentials.
2. From the **Security** menu, select **SSL > Orders**.
3. Click the **Send** link in the **Email** column for the SSL certificate that you want.<br/>**Note:** A pop-up window appears to confirm the request. This window contains the email address for the Domain Administrator that was provided when the SSL certificate was requested.
4. Click **Resend Email** to confirm the selection and request an additional fulfillment email from the certificate authority.  Or, click **Cancel** to cancel the action.

## Next Steps

After requesting an additional fulfillment email, the request will be forwarded to the applicable certificate authority for completion. Because SSL certificate details are confidential, {{site.data.keyword.BluSoftlayer_notm}} does not store the SSL certificate data on its system. After receiving the SSL certificate details by email, they can be manually [imported](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates) to the {{site.data.keyword.slportal}}, if necessary.
