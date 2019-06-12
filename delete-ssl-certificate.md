---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificates delete, SSL delete

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Deleting SSL certificates
{: #deleting-ssl-certificates}

After an SSL certificate's details are imported into the {{site.data.keyword.cloud}} console, it can be deleted at any time to remove all data from being saved to the {{site.data.keyword.cloud_notm}} console.

To delete an SSL certificate, complete the following steps.

1. Navigate to your console's security menu. For more information, see [Navigating to devices](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. From the **Security** menu, select **SSL > Certificates**.
3. From the **Actions** menu, select **Delete** for the desired SSL certificate.
4. Click **Yes** to delete the SSL certificate..

## Next steps

After deleting an SSL certificate, all services that are linked to the certificate no longer use its information. The certificate no longer appears on the SSL certificates screen within the {{site.data.keyword.cloud_notm}} console.

Update all services that previously used the deleted certificate to be associated with a valid SSL certificate that is associated with the account.

At any time, the SSL certificate can be added back to the {{site.data.keyword.cloud_notm}} console by using the [import](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates) process.
{:note}
