---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-21"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Getting started with SSL certificates  


## Before you begin

Getting started with SSL requires a bit of planning. Complete the following prerequisites.

1. Decide where to get the certificate
2. Learn about the types of certificates, key length, and duration
3. Choose a common name
4. Learn about the socket rule
5. Generate the CSR

For more information, see [Planning for SSL certificates](planning-ahead-ssl.html).

## Ordering SSL certificates

1. Access the [{{site.data.keyword.slportal_full}} ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/){: new_window} by using your unique credentials.
2. Select **Security > SSL certificates >** to access the SSL certificates screen.
3. You must select the type and duration of certificate, submit the text of the CSR, enter some additional details, and then confirm payment.

## Installing and testing
After the ordering and validating process is complete, you receive an email from the certificate authority that includes your certificate, as well as any necessary intermediate certificates. The method for installation depends on the software you are using but the result should be the same. You should, when done, be able to go to <http://host.yourdomain.com> and see your content while also seeing the SSL padlock that browsers use to denote an encrypted session. If you get a warning, then there are steps that you must take.

## Next Steps

After testing successfully, you can access the SSL certificates screen, to [update](view-and-update-ssl-certificate.html), [download](download-ssl-certificate-details.html), [delete](delete-ssl-certificate.html), or [import](import-ssl-certificate.html) existing SSL certificates into the tool.
