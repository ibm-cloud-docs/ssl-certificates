---

copyright:
  years: 2014, 2019
lastupdated: "2020-01-17"

keywords:  renewing SSL certificates, renewal SSL, SSL certificate renewal process, renewing, renewal

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Renewing SSL certificates
{: #renewing-ssl-certificates}

After an SSL certificate is ordered through {{site.data.keyword.cloud}}, it can be renewed at any time. During the renewal process, {{site.data.keyword.cloud_notm}} acts as the facilitator between you and the certificate authority, and does not see or control any part of the renewal process that involves the details of the SSL certificate. SSL certificates are renewed under the same terms under which they were ordered, so you can't change any renewal details (certificate type and authority, validity month, server platform, and so on). Certificates can be renewed before or after they expire; however, to maintain the validity of the SSL certificate, renew the certificate before its expiration date.
{: shortdesc}

## Renewing an SSL certificate
Complete the following steps to renew an SSL certificate.

1. Navigate to your console's security menu. For more information, see [Navigating to devices](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. From the **Security** menu, select **SSL > Orders**.
3. Click **Renew** in the **Renew** column for the desired SSL certificate.
4. Determine whether all renewal and CSR details are correct before you renew the SSL certificate. See the following table for more information.  

| Details                         | Action  |
| ------------------------------- | ------- |
| Correct renewal and CSR details | Select **Renew** to renew the SSL certificate. |
| Incorrect renewal details       | Select **Purchase a new SSL certificate** to order a new certificate. Because renewal        details, including certificate type, authority, and approve email can't be changed, the only way to update details for a website's SSL certificate is to order a new certificate. |
| Incorrect CSR details           | Select **Change CSR**, enter the new CSR details in the **CSR text box**, and select **Restore CSR**. |
{: caption="Table 1. Renewal and CSR details" caption-side="top"}

## Next steps
{: #ns-renewing-ssl-certificates}

After requesting an SSL certificate's renewal, {{site.data.keyword.cloud_notm}} forwards the request to the certificate authority in order to complete the website verification required for renewal. Upon renewal of the certificate, the new expiration date appears in the **Expires** field. Notice that after the ordering and validating process is complete, you receive an fulfillment email from the certificate authority that includes all the details that are associated with the SSL certificate. The certificate authority sends a fulfillment email to the domain administrator provided during the ordering process. The fulfillment email can be requested again from the SSL Orders screen, as described [here](https://cloud.ibm.com/docs/infrastructure/ssl-certificates?topic=ssl-certificates-requesting-an-ssl-certificate-fulfillment-email).
