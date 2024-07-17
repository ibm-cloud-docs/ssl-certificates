---

copyright:
  years: 2014, 2024
lastupdated: "2024-07-17"

keywords: migrating ssl certificates, secrets manager

subcollection: ssl-certificates

---

{{site.data.keyword.attribute-definition-list}}

# Migrating SSL certificates
{: #migrating-ssl-certificates}

SSL Certificate Order is deprecated. As of 15 April 2024, SSL Certificate Order is no longer available for purchase. As of 15 December 2024, SSL Certificate Order is no longer supported for new orders or reorders. Only existing certificates that are not expired are still available for you to download, reissue, or revoke. For more information, see [Deprecation of SSL Certificates](/docs/ssl-certificates?topic=ssl-certificates-deprecation).
{: deprecated}

- You can't create new orders through the SSL Certificate Order.
- Between the EOM date and the End of Service (EOS), the SSL Certificate Order is still available for you to view your past orders, certificate status, and the expiration date.
- Before the EOS date, you can continue to receive support on certificates that aren't expired. You can't get support for expired certificates.

 Depending on various migration scenarios and the expiration dates of your certificates, you might have one of the following options to migrate your SSL certificates.

## Ordering certificates before EOM
{: #order-new-ssl-certificates-before-eom}

Before the EOM date, you can still order a certificate or reorder your existing certificate. For more information, see [Ordering SSL certificates](/docs/ssl-certificates?topic=ssl-certificates-getting-started-tutorial#ordering-ssl-certificates).

## Managing your existing certificates
{: #migratng-existing-ssl-certificates}

If you have an existing SSL certificate that is not expired, do the following actions:

- Before the EOM date and before the SSL certificate expires, reorder the certificate from the [SSL Certificate Order](/classic-gen1/sslorders) page to get the SSL certificate expiration date extended for another year.
- Import your existing certificate to the [SSL Certificates](/classic-gen1/sslcerts) page for management. For more information about importing certificates, see [Importing SSL Certificates](/docs/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates).
- Before the SSL certificate expires, you can still view or update your SSL certificates on the [SSL Certificates](/classic-gen1/sslcerts) page. For more information, see [Viewing and updating SSL certificates](/docs/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates).

You can also migrate to {{site.data.keyword.cloud}}'s strategic offering, {{site.data.keyword.secrets-manager_full}} for enhanced security and advanced features. See [Migrating to Secrets Manager to create certificates](#migrating-ssl-secrets-manager-new-cert) and [Migrating to Secrets Manager for certificate lifecycle management](#migrating-ssl-secret-manager-lifecycle) for more details.

## Migrating to Secrets Manager to create certificates
{: #migrating-ssl-secrets-manager-new-cert}

If you want a new public certificate after EOM, you can migrate to Secrets Manager.

1. Create a Secret Manager instance. See [Creating a Secrets Manager service instance](/docs/secrets-manager?topic=secrets-manager-create-instance) for more details.
2. Request public SSL/TLS certificates from another certificate authority LetsEncrypt. See [Ordering SSL/TLS public certificates](/docs/secrets-manager?topic=secrets-manager-public-certificates) for more details.

With Secrets Manager, you can also store, request, and generate private SSL/TLS certificates by using a private certificate authority for your apps or services. For more information about private certificates, see [Creating SSL/TLS private certificates](/docs/secrets-manager?topic=secrets-manager-private-certificates).

## Migrating to Secrets Manager for SSL certificate lifecycle management
{: #migrating-ssl-secret-manager-lifecycle}

If you want to manage your SSL certificate lifecycle after EOM, Secrets Manager also offers certificate lifecycle management similar to the [SSL Certificates](/classic-gen1/sslcerts) page. Your SSL certificates are stored securely in your dedicated Secrets Manager service instance where you can centrally manage the lifecycles.

For more information, see [Importing SSL/TLS certificates](/docs/secrets-manager?topic=secrets-manager-certificates).

## Migrating to DigiCert to order DigiCert certificates
{: #migrating-ssl-digi-cert-lifecycle}

If you have a preference on using DigiCert certificates or your certificates need renewed after the EOM date, you can migrate to DigiCert by creating a DigiCert account. You can contact DigiCert sales (sales@digicert.com) to set up an account with an assigned account manager.

For more information about getting started with DigiCert, see [DigiCert CertCentral documentation](https://docs.digicert.com/en/certcentral.html){:external}.
