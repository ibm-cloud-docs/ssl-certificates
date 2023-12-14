---

copyright:
  years: 2023
lastupdated: "2023-12-15"

keywords:

subcollection: ssl-certificates

---

{{site.data.keyword.attribute-definition-list}}

# Deprecation of SSL Certificates
{: #deprecation}

SSL Certificate Order is deprecated. As of 15 April 2024, SSL Certificate Order is no longer available for purchase. As of 15 December 2024, SSL Certificate Order is no longer supported for new orders or reorders. Only your existing certificates that are not expired are still available for you to download, reissue, or revoke.
{: shortdesc}

## Important dates
{: #deprecation-timeline}

The following table describes the details of the deprecation, timeline, and extra information.

| Date | Stage | Description |
| --- | --- | --- |
| 15 December 2023 | Deprecation announcement (SoftLayer notification) | Announcement of the SSL Certificate Order deprecation. All current SSL Certificate Order users receive an announcement email with information about the deprecation. |
| 17 January 2024 | Deprecation announcement ({{site.data.keyword.cloud}} Announcement) | Announcement of the SSL Certificate Order deprecation through {{site.data.keyword.cloud}} Announcement. Notification details are put into the console and related screens. |
| 15 April 2024 | End of Marketing (EOM) | SSL Certificate Order end of marketing. After this date, SSL Certificate Order is no longer available for purchase. For more information, see [Deprecation details](/docs/ssl-certificates?topic=ssl-certificates-deprecation#deprecation-details). |
| Ongoing | Reminders | Periodic reminders are sent to remaining SSL Certificate users that the end of support date is coming.|
| 15 December 2024 | End of Support (EOS) | SSL Certificate Order end of support. For more information, see [Deprecation details](/docs/ssl-certificates?topic=ssl-certificates-deprecation#deprecation-details). |
{: caption="Table 1. Deprecation timeline" caption-side="bottom"}

## Deprecation details
{: #deprecation-details}

Review the following details about the SSL Certificates Order deprecation:

* After EOM (15 April 2024), you can't create new orders through the SSL Certificate Order.
* After EOM (15 April 2024) and before EOS (15 December 2024), SSL Certificate Order is still available for you to view your past orders, certificate status, and the expiration date. You will continue to receive support before EOS (15 December 2024), but you cannot get support for expired certificates.
* After EOS (15 December 2024), SSL Certificate Order is no longer supported for orders or reorders. Only your existing certificates that are not expired are available for you to download, reissue, or revoke.

## Next steps for current users
{: #deprecation-next-steps}

If you have an existing SSL certificate that is not expired, do the following actions:

- Before the EOM date and before the SSL certificate expires, reorder the certificate from the SSL orders screen to extend the SSL certificate expiration date for another year. For more information about ordering a certificate, see the [Getting Started Tutorial](/docs/ssl-certificates?topic=ssl-certificates-getting-started-tutorial).
- Import your existing certificate to the SSL Certificates screen for management. For more information about importing certificates, see [Importing SSL Certificates](/docs/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates).
- Before the SSL certificate expires, you can still view or update your SSL certificates on the SSL Certificates screen. For more information, see [Viewing and updating SSL certificates](/docs/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates).

You can also migrate to {{site.data.keyword.cloud}}'s strategic offering, {{site.data.keyword.secrets-manager_full}} for enhanced security and advanced features. For more information, see [Migrating to Secrets Manager to create new certificates](/docs/ssl-certificates?topic=ssl-certificates-deprecation#deprecation-migrating-ssl-secrets-manager-new-cert) and [Migrating to Secrets Manager for certificate lifecycle management](/docs/ssl-certificates?topic=ssl-certificates-deprecation#deprecation-migrating-ssl-secret-manager-lifecycle).

## Migration options
{: #deprecation-migration-options}

See the following options to create and manage new SSL certificates

### Migrating to Secrets Manager to create new SSL certificates
{: #deprecation-migrating-ssl-secrets-manager-new-cert}

If you want a new public certificate after EOM, you can migrate to Secrets Manager.

1. Create a Secret Manager instance. For more information, see [Creating a Secrets Manager service instance](/docs/secrets-manager?topic=secrets-manager-create-instance).
2. Request public SSL/TLS certificates from another Certificate Authority LetsEncrypt. For more information, see [Ordering SSL/TLS public certificates](/docs/secrets-manager?topic=secrets-manager-public-certificates).

With Secrets Manager, you can also store, request, and generate private SSL/TLS certificates by using a private certificate authority for your apps or services. For more information about private certificates, see [Creating SSL/TLS private certificates](/docs/secrets-manager?topic=secrets-manager-private-certificates).

### Migrating to Secrets Manager for SSL certificate lifecycle management
{: #deprecation-migrating-ssl-secret-manager-lifecycle}

If you want to manage your SSL certificate lifecycle after EOM, Secrets Manager also offers certificate lifecycle management that is similar to the SSL Certificates screen. Your SSL certificates are stored securely in your dedicated Secrets Manager service instance where you can centrally manage the lifecycles.

For more information, see [Importing SSL/TLS certificates](/docs/secrets-manager?topic=secrets-manager-certificates).

### Migrating to DigiCert to order new DigiCert certificates
{: #deprecation-migrating-ssl-digi-cert-lifecycle}

If you have a preference on using DigiCert certificates or your certificates need renewed after the EOM date, you can migrate to DigiCert by creating a DigiCert account. You can contact DigiCert sales (sales@digicert.com) to set up a new account with an assigned account manager.

For more information about getting started with DigiCert, see [DigiCert CertCentral documentation](https://docs.digicert.com/en/certcentral.html){: external}.

## Customer Support
{: #deprecation-support}

If you need more help with your {{site.data.keyword.cloud}} SSL Certificates migration after you review these materials and resources, or if you have questions, contact [{{site.data.keyword.cloud}} Customer Support](https://cloud.ibm.com/unifiedsupport/supportcenter){: external}.
