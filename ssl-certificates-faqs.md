---

copyright:
  years: 2014, 2019, 2020
lastupdated: "2020-03-23"

keywords: SSL certificates FAQ, SSL FAQ

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:support: data-reuse='support'}
{:new_window: target="_blank"}
{:faq: data-hd-content-type='faq'}

# FAQs: SSL certificates
{: #faqs-ssl-certificates}

## Why doesn't the SSL certificate that I ordered automatically show up on the SSL certificates screen?
{: faq}
{: support}

SSL certificates are issued by a third-party certificate authority, which sends all of the certificate details directly to you in a confidential email. After receiving that email, you have the option to [import the SSL certificate](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates) to the {{site.data.keyword.cloud}} console should you choose to use the certificate with {{site.data.keyword.cloud_notm}} products and services. Because {{site.data.keyword.cloud_notm}} never receives the details for SSL certificate, data cannot be imported automatically.

## What is an SSL certificate?
{: faq}
{: support}

SSL certificates are enabled by websites as a security measure to protect the user. They are generally used when you are required to transmit confidential information to a website, such as name, address, credit card numbers, and other personal data or are managing data that requires authentication (such as in the {{site.data.keyword.cloud_notm}} console). SSL certificates are requested by the company that runs the website but are issued by a trusted, third-party company that ensures the validity of the website. Secure websites are preceded by HTTPS in the URL, as opposed to the standard HTTP.

## How can I order an SHA2 SSL?
{: faq}
{: support}

If you already ordered an SSL and it is showing errors that the SSL certificate is using SHA-1 instead of SHA-2, you need to request that the SSL is re-issued. You can do this by submitting a ticket.

If you have not yet ordered an SSL from {{site.data.keyword.cloud_notm}} and need to order one with SHA-2, submit a ticket to manually order an SSL for the domain in question. {{site.data.keyword.cloud_notm}} console still automatically creates SSL certificates using SHA-1, so if you do this, you will then need to have it re-issued.
