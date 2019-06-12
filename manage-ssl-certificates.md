---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: management of certificates, add certificate, managing certificates

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Managing SSL certificates
{: #managing-ssl-certificates}

You can manage your SSL certificates in the {{site.data.keyword.cloud}} console. Not only can this serve as a repository for management of your certificates, it is also necessary when using services that can use or require certificates.

1. Navigate to your console's security menu. For more information, see [Navigating to devices](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. From the **Security** menu, select **SSL > Certificates > Manage Certificates**.


You are presented with a list of your current certificates, along with information regarding their status.

You can search, download parts of a certificate or a PEM formatted version, or review the expiration of your certificates. You can also view how many services are currently using each certificate. This lets you know whether action must be taken when a certificate is nearing expiration.

## Adding a certificate

When you are ready to add a certificate, select **Add Certificate** in the sub-navigation menu or within the Certificate List title. You are only required to supply the certificate and its private key. However, not providing an intermediate certificate when your issuer provides one can result in a broken certificate chain and improper validation for users or associated services.

Private keys that require a passphrase cannot be stored.
{:note}

Once added, the following fields are derived from your certificates directly:

* Common name
* Organization name
* Validity period

## Editing a certificate

Activating the triangle to the left of a certificate reveals the certificate parts in their entirety. This also allows the certificate parts to be edited. A note can be added, and when necessary the certificate can be removed. Also listed is a list of services that are currently using the certificate.

Only certificates that are not associated with services can have their private key, certificate, or intermediate certificate parts updated. The certificate also cannot be removed. You can modify the note at any time.

## Removing a certificate

To remove a certificate, follow the steps to edit it and select "Confirm certificate removal" and save.

## Using the API

For an example of editing certificates using the API, see [SSL Management ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://sldn.softlayer.com/article/ssl-management){: new_window}.
