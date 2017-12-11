---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-17"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Deleting SSL certificates

## Overview

After an SSL certificate's details are imported into the {{site.data.keyword.slportal_full}}, it may be deleted at any time to remove all data from being saved to the {{site.data.keyword.slportal}}.

To delete an SSL certificate, complete the following steps.

## Deleting an SSL certificate

1. Access the [{{site.data.keyword.slportal}} ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/){: new_window} by using your unique credentials.
2. From the **Security** menu, select **SSL > Certificates**.
3. From the **Actions** menu, select **Delete** for the desired SSL certificate.

  **Note:** A window appears to confirm the deletion.
4. Click **Yes** to delete the SSL certificate or click **No** to cancel the action.

## Next Steps

After deleting an SSL certificate, all services linked to the certificate will no longer utilize its information. The certificate no longer appears on the SSL certificates screen within the {{site.data.keyword.slportal}}.

It is recommended that you update all services that previously used the deleted certificate to be associated with a valid SSL certificate that is associated with the account.

**Note:** At any time, the SSL certificate may be added back to the {{site.data.keyword.slportal}} using the [import](import-ssl-certificate.html) process.
