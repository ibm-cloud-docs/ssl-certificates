---

copyright:
  years: 2014, 2019
lastupdated: "2022-06-06"

keywords: types of certificates,SSL certificates, Select Security

subcollection: ssl-certificates

---

{{site.data.keyword.attribute-definition-list}}

# Getting started tutorial
{: #getting-started-tutorial}

## Before you begin
{: #byb-getting-started-tutorial}

Getting started with SSL requires a bit of planning. Complete the following prerequisites.

1. Decide where to get the certificate
2. Learn about the types of certificates, key length, and duration
3. Choose a common name
4. Learn about the socket rule
5. Generate the CSR

For more information, see [Planning for SSL certificates](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-planning-for-ssl#planning-for-ssl).

## Ordering SSL certificates
{: #ordering-ssl-certificates}

1. Navigate to your console's security menu. For more information, see [Navigating to devices](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. From the **Security** menu, select **Security > SSL > Certificates**.
3. Select **Order SSL Certificate**.
4. Select the type and duration of certificate, submit the text of the CSR, and select your server platform. 
5. You must verify that you own the domain by choosing an email that is connected to the domain. See [Why do I need to choose an email?](/docs/ssl-certificates?topic=ssl-certificates-faqs-ssl-certificates#why-do-i-need-to-choose-an-email) for more details on verifying domain ownership. 
6. Confirm payment. 
7. Wait for a verification email. The email is delivered to the address that you entered in step 5. Click the link in the email to verify domain ownership. 
8. After confirming domain ownership, the SSL Certificate is delivered to the email address that is connected to your account. 
9. If either the verification email or the SSL Certificate email take longer than half an hour to arrive, please contact the Support Team. 

## Installing and testing
{: #installing-ssl-certs}

After the ordering and validating process is complete, you receive an email from the certificate authority that includes your certificate, as well as any necessary intermediate certificates. The method for installation depends on the software you are using. After you complete the installation, to go to `http://host.yourdomain.com` to confirm the presence of the SSL padlock in the browser address bar that signals an encrypted session. If you get a warning, take any indicated steps to resolve it.

## Next steps
{: #ns-getting-started-tutorial}

After testing successfully, you can access your SSL certificates in the {{site.data.keyword.cloud_notm}} console to [update](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates#viewing-and-updating-ssl-certificates), [download](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details#downloading-ssl-certificate-details), [delete](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates), or [import](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates) existing SSL certificates into the tool.
