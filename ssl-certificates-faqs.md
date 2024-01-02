---

copyright:
  years: 2014, 2024
lastupdated: "2024-01-02"

keywords: SSL certificates FAQ, SSL FAQ

subcollection: ssl-certificates

content-type: faq

---

{{site.data.keyword.attribute-definition-list}}

# FAQs: SSL certificates
{: #faqs-ssl-certificates}

SSL Certificate Order is deprecated. As of 15 April 2024, SSL Certificate Order is no longer available for purchase. As of 15 December 2024,  SSL Certificate Order is no longer supported for new orders or reorders. Only existing certificates that are not expired are still available for you to download, reissue, or revoke. For more information, see [Deprecation of SSL Certificates](/docs/ssl-certificates?topic=ssl-certificates-deprecation-ssl-certificates).
{: deprecated}

## Why doesn't the SSL certificate that I ordered automatically show up on the SSL certificates screen?
{: #faq-ssl-cert-1}
{: support}

SSL certificates are issued by a third-party certificate authority, which sends all of the certificate details directly to you in a confidential email. After receiving that email, you have the option to [import the SSL certificate](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates) to the {{site.data.keyword.cloud}} console should you choose to use the certificate with {{site.data.keyword.cloud_notm}} products and services. Because {{site.data.keyword.cloud_notm}} never receives the details for SSL certificate, data cannot be imported automatically.

## What is an SSL certificate?
{: #faq-ssl-cert-2}
{: support}

SSL certificates are enabled by websites as a security measure to protect the user. They are generally used when you are required to transmit confidential information to a website, such as name, address, credit card numbers, and other personal data or are managing data that requires authentication (such as in the {{site.data.keyword.cloud_notm}} console). SSL certificates are requested by the company that runs the website but are issued by a trusted, third-party company that ensures the validity of the website. Secure websites are preceded by HTTPS in the URL, as opposed to the standard HTTP.

## How can I order an SHA2 SSL?
{: #faq-ssl-cert-3}
{: support}

If you already ordered an SSL and it is showing errors that the SSL certificate is using SHA-1 instead of SHA-2, you need to request that the SSL is re-issued. You can do this by submitting a ticket.

If you have not yet ordered an SSL from {{site.data.keyword.cloud_notm}} and need to order one with SHA-2, submit a ticket to manually order an SSL for the domain in question. {{site.data.keyword.cloud_notm}} console still automatically creates SSL certificates using SHA-1, so if you do this, you will then need to have it re-issued.

## Why do I need to choose an email? 
{: #faq-ssl-cert-4}
{: support}

To create an SSL certificate, you need to verify that you own the domain where you are requesting the SSL certificate. You can verify that you own the domain in one of two ways: 

1. If you have an email connected to the domain, such as *admin@your_domain*, you can verify using that email address. Just choose the email address that you use from the list provided, and you receive a verification email at the chosen address. 

2. If you do not have an email connected to the domain, you must contact support to use DNS TXT verification. Just open a case, and the Support team will walk you through what to do. Using email verification is generally preferred. 

Either way, you verify that the domain is yours to use, and then receive an SSL certificate. 

## Why can't I order a wildcard SSL certificate? 
{:  #faq-ssl-cert-6}
{: support}

Wildcard SSL certificates are not available in {{site.data.keyword.cloud_notm}}. 

## How do I request SSL-VPN logs?
{: #faq-ssl-cert-5}
{: support}

For information about requesting SSL-VPN audit logs, see [How do I request SSL-VPN logs](/docs/iaas-vpn?topic=iaas-vpn-vpn-ssl-faq) in the [SSL VPN FAQs](/docs/iaas-vpn?topic=iaas-vpn-vpn-ssl-faq).

## What happens to my SSL certificates after SSL Certificate Order is no longer available for purchase?
{: #faq-ssl-cert-7}
{: support}

**End of Marketing (EOM): 15 April 2024** After this date, SSL Certificate Order is no longer available for purchase. 

After the EOM date, you can't order any new SSL certificates by using the SSL Certificate Order portal. 

If your SSL certificate is close to expiration and you don’t reorder a new SSL certificate by the EOM date, you must migrate to either {{site.data.keyword.secrets-manager_full}} or DigiCert to order new certificates. 

For more information regarding the options for your SSL certificates, see [Deprecation of SSL Certificates](/docs/ssl-certificates?topic=ssl-certificates-deprecation-ssl-certificates).

