---

copyright:
  years: 2014, 2024
lastupdated: "2024-05-17"

keywords: management of certificates, add certificate, managing certificates

subcollection: ssl-certificates

---

{{site.data.keyword.attribute-definition-list}}

# Managing SSL certificates
{: #managing-ssl-certificates}

SSL Certificate Order is deprecated. As of 15 April 2024, SSL Certificate Order is no longer available for purchase. As of 15 December 2024,  SSL Certificate Order is no longer supported for new orders or reorders. Only existing certificates that are not expired are still available for you to download, reissue, or revoke. For more information, see [Deprecation of SSL Certificates](/docs/ssl-certificates?topic=ssl-certificates-deprecation).
{: deprecated}

You can manage your SSL certificates in the {{site.data.keyword.cloud}} console. Not only can this serve as a repository for management of your certificates, it is also necessary when using services that can use or require certificates.

1. Navigate to your console's security menu. For more information, see [Navigating to devices](//docs/ssl-certificates?topic=ssl-certificates-navigating-devices).
2. From the **Security** menu, select **SSL > Certificates > Manage Certificates**.

You are presented with a list of your current certificates, along with information regarding their status.

You can search, download parts of a certificate or a PEM formatted version, or review the expiration of your certificates. You can also view how many services are currently using each certificate. This lets you know whether action must be taken when a certificate is nearing expiration.

## Adding an SSL certificate
{: #adding-ssl-certficate}

When you are ready to add a certificate, select **Add Certificate** in the sub-navigation menu or within the Certificate List title. You are only required to supply the certificate and its private key. However, not providing an intermediate certificate when your issuer provides one can result in a broken certificate chain and improper validation for users or associated services.

Private keys that require a passphrase cannot be stored.
{: note}

Once added, the following fields are derived from your certificates directly:

* Common name
* Organization name
* Validity period

## Editing an SSL certificate
{: #editing-ssl-certficate}

Activating the triangle to the left of a certificate reveals the certificate parts in their entirety. This also allows the certificate parts to be edited. A note can be added, and when necessary the certificate can be removed. Also listed is a list of services that are currently using the certificate.

Only certificates that are not associated with services can have their private key, certificate, or intermediate certificate parts updated. The certificate also cannot be removed. You can modify the note at any time.

## Removing an SSL certificate
{: #removing-ssl-certficate}

To remove a certificate, follow the steps to edit it and select **Confirm certificate removal** and save.

## Managing SSL certificates by using the API
{: #manage-ssl-certificate-api}

For an example of editing certificates using the API, see [SSL Management ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://sldn.softlayer.com/article/ssl-management){: external}.
