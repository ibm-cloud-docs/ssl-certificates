---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Installing SSL certificates in Plesk 9

To add SSL certificates in Plesk 9, complete the following steps.

1. Log in to Plesk and go to the domain on which you want to install the certificate.
2. Enter into the configuration of the target domain.
3. Click **SSL certificates**.
4. Click **Add SSL certificate**.

   **Note:** If you already have an SSL certificate, skip this step and go to step 8.
5.  Name the certificate.  You can name it anything, but it can be helpful to use a descriptive name, including a time stamp.

   In this case, use the *YYYYMMDDRR* format where *RR* is the revision number (00 in this case as there are no revisions for the same day).
6. Make any necessary adjustments to the SSL Request. This information is embedded in the SSL certificate and should be similar to the domain registration information.

  The email address should match one of the email addresses in the domain whose information was provided by your domain registrar.

  **Important:** False information might be rejected by your SSL certificate authority.
7. Go back into the certificate configuration.
8. Review the CSR and private key and save the private key in a safe location.  

  **Note:** If anything occurs with your server that the certificate must be reentered, you must have at least the certificate and private key.
9. Take the CSR and submit it to the certificate authority of your choice. {{site.data.keyword.cloud_notm}} infrastructure does not provide SSL certificates.
10. After you receive the certificate from your certificate authority, you can paste it into the certificate text area.

   **Notes:**
   * If your certificate authority requires, you might need to paste their own certificate into the CA certificate text area (often called a CA Bundle).
   * You must have a matching private key and certificate to use a certificate.
11. Go back to the *<span style="text-decoration: underline">Web Hosting Settings</span>* from the Domains configuration.
12. Select the corresponding certificate and click **OK**.

The new certificate is now being used for the domain.  If you update the certificate, then you might need to completely close out of your browser before the new certificate is used.
