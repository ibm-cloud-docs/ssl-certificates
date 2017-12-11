---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Managing SSL certificates

{{site.data.keyword.BluSoftlayer_full}} now provides a means of storing certificates within its portal. Not only can this serve as a repository for management of your certificates, it is also necessary when using services that can use or require certificates.

1. Access the [{{site.data.keyword.slportal_full}} ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/){: new_window} by using your unique credentials.
2. From the **Security** menu, select **SSL > Certificates > Manage Certificates**.

You are presented with a list of your current certificates, along with information regarding their status.

You may search, download parts of a certificate or a PEM formatted version, or review the expiration of your certificates. You can also view how many services are currently utilizing each certificate. This lets you know if action must be taken when a certificate is nearing expiration.

## Adding a certificate

When you are ready to add a certificate, select "Add Certificate" in the sub-navigation menu or within the Certificate List title. You are only required to supply the certificate and its private key. However, not providing an intermediate certificate when your issuer provides one can result in a broken certificate chain and improper validation for end users or associated services.

Note: Private keys that require a passphrase cannot be stored.

Once added, the following fields are derived from your certificates directly:

* Common Name
* Organization Name
* Validity Period


That's it!

## Editing a certificate

Activating the triangle to the left of a certificate will reveal the certificate parts in their entirety. This also allows the certificate parts to be edited. A note may be added, and when necessary the certificate may be removed. Also listed is a list of services that are currently utilizing the certificate.



Important Note: Only certificates that are not associated with services may have their "private key," "certificate," or "intermediate certificate" parts updated.  The certificate can also not be removed.

You may modify the note at any time.

## Removing a certificate

In order to remove a certificate, simply follow the steps to edit it and select the "Confirm certificate removal" checkbox and save.

### API

The ability to add, remove, edit, and search your certificates is also available through the SLAPI sldn.softlayer.com. Some examples have been provided in the following SLDN article, sldn.softlayer.com/article/SSL-Management-my-SLAPI-Its-more-likely-you-think.
