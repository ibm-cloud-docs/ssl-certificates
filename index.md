---

copyright:
  years: 2014, 2024
lastupdated: "2024-07-17"

keywords: types of certificates,SSL certificates, Select Security

subcollection: ssl-certificates

---

{{site.data.keyword.attribute-definition-list}}

# Getting started tutorial
{: #getting-started-tutorial}

SSL Certificate Order is deprecated. As of 15 April 2024, SSL Certificate Order is no longer available for purchase. As of 15 December 2024, SSL Certificate Order is no longer supported for new orders or reorders. Only existing certificates that are not expired are still available for you to download, reissue, or revoke. For more information, see [Deprecation of SSL Certificates](/docs/ssl-certificates?topic=ssl-certificates-deprecation).
{: deprecated}

## Before you begin
{: #byb-getting-started-tutorial}

Getting started with SSL requires a bit of planning. Complete the following prerequisites.

1. Decide where to get the certificate
2. Learn about the types of certificates, key length, and duration
3. Choose a common name
4. Learn about the socket rule
5. Generate the CSR

For more information, see [Planning for SSL certificates](/docs/ssl-certificates?topic=ssl-certificates-planning-for-ssl).

If you are ordering a Microsoft certificate, by default the Federal Common Policy CA G2 root certificate is issued. If you need a Federal Common Policy CA G1 root certificate, you must create a support case. For more information, see [Using the Support Center](/docs/get-support?topic=get-support-using-avatar).
{: important}

## Ordering SSL certificates
{: #ordering-ssl-certificates}

1. Go to your console's security menu. For more information, see [Navigating to devices](/docs/ssl-certificates?topic=ssl-certificates-navigating-devices).
2. From the **Security** menu, select **Security > SSL > Certificates**.
3. Select **Order SSL Certificate**.
4. Select the type and duration of the certificate, submit the text of the CSR, and select your server platform.
5. You must verify that you own the domain by choosing an email that is connected to the domain. See [Why do I need to choose an email?](/docs/ssl-certificates?topic=ssl-certificates-faqs-ssl-certificates#faq-ssl-cert-4) for more details on verifying domain ownership.
6. Confirm payment.
7. Wait for a verification email. The email is delivered to the address that you entered in step 5. Click the link in the email to verify domain ownership.
8. After you confirm domain ownership, the SSL Certificate is delivered to the email address that is connected to your account.
9. If either the verification email or the SSL Certificate email takes longer than half an hour to arrive, contact support.

## Installing and testing
{: #installing-ssl-certs}

After the ordering and validating process is complete, you receive an email from the certificate authority that includes your certificate, and any necessary intermediate certificates. The method for installation depends on the software you are using. After you complete the installation, to go to `http://host.yourdomain.com` to confirm the presence of the SSL padlock in the browser address bar that signals an encrypted session. If you get a warning, take any indicated steps to resolve it.

## Next steps
{: #ns-getting-started-tutorial}

After a successful test, you can [manage your SSL certificates](/docs/ssl-certificates?topic=ssl-certificates-managing-ssl-certificates).
