---

copyright:
  years: 2014, 2018
lastupdated: "2018-05-17"

keywords:  renewing SSL certificates, renewal SSL, SSL certificate renewal process, renewing, renewal

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Renewing SSL certificates
{: #renewing-ssl-certificates}

After an SSL certificate is ordered through {{site.data.keyword.BluSoftlayer_full}}, it can be renewed at any time. During the renewal process, {{site.data.keyword.BluSoftlayer_notm}} acts as the facilitator between the customer (you) and the certificate authority, and does not see or control any part of the renewal process that involves the details of the SSL certificate. SSL certificates are renewed under the same terms in which they were ordered, so no changes to the Renewal Details (certificate Type and Authority, Validity Month, Server Platform, and so on) can be made. Certificates can be renewed before or after they expire; however, to maintain the validity of the SSL certificate, renew the certificate before its expiration date. Complete the following steps to renew an SSL certificate.

## Renewing an SSL certificate

1. Access the [{{site.data.keyword.slportal_full}} ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/){: new_window} by using your unique credentials.
2. From the **Security** menu, select **SSL > Orders**.
3. Click the **Renew** link in the **Renew** column for the desired SSL certificate.

   **Note:** A pop-up box will appear to complete the request.  
   * Determine if all Renewal and CSR details are correct:<br /><br /><table border="1"><caption>Table 1. Renewal and CSR details</caption><tr><th>If...</th><th>Then...</th></tr><tr><td>All Renewal and CSR details are correct</td><td>Proceed to the next step.</td></tr><tr><td>Renewal details are incorrect</td><td><ul><li>Click the <strong>Purchase a new SSL certificate</strong> link to be redirected to the purchasing screen.<br /><blockquote><strong>Note:</strong> Because Renewal details, including the certificate Type, Authority and Approve Email cannot be changed, the only way to update details for a website's SSL certificate is to order a new certificate.</blockquote></li><li>Complete the screens on the Order page with the desired information for the SSL certificate. No additional action is required using this procedure.</li></ul></td></tr><tr><td>CSR details are incorrect</td><td><ul><li>Click the **Change CSR** button.</li><li>Enter the **new CSR details** in the **CSR** text box.</li><li>Click the **Restore CSR** button.</li></ul></td></tr></table>
4. Click the **Renew** button to renew the SSL certificate or click **Cancel** to cancel the action.

## Next Steps

After requesting an SSL certificate's renewal, {{site.data.keyword.BluSoftlayer_notm}} forwards the request to the certificate authority in order to complete the website verification required for renewal. Upon renewal of the certificate, the new expiration date appears in the Expires field.
