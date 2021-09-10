---

copyright:
  years: 2014, 2019
lastupdated: "2019-08-26"

keywords: view SSL certificates, update SSL certificates, original certificates

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Viewing and updating SSL certificates
{: #viewing-and-updating-ssl-certificates}

After an SSL certificate is imported to the SSL certificates screen, you can view and update it at any time. Updates work similar to the [import process](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates), as all details that are updated must match the original certificate exactly, including spacing and line breaks.
{: shortdesc}

To view and update an SSL certificate, complete the following steps.

1. Navigate to your console's security menu. For more information, see [Navigating to devices](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. From the **Security** menu, select **SSL > Certificates**.
3. Select **View/Update certificate** from the **Actions** drop down list.
4. Update the **SSL certificate details** in the applicable text boxes, and click **Update** to apply your changes. See the following table for more information.

   Details that are entered in the **Import SSL certificate** window must be entered exactly as provided by the certificate authority, including spacing and line breaks. If not, an error occurs.
   {: note}

| SSL Certificate Details     | Description |
| --------------------------- | ----------- |
|Certificate                  | SSL certificate details that are provided by the certificate authority. This is generally an alpha-numeric block of text.|
|Private key                  | Private key details for the certificate that are provided by the certificate authority. This is generally an alpha-numeric block of text.|
|Intermediate certificate     | Intermediate certificate details that are provided by the certificate authority. Intermediate certificates are not required; however, if the information is available for the SSL certificate, it should be entered.|
|Certificate signing request  | Certificate signing request (CSR) details that are provided by the certificate authority. CSR details are not required, but should be provided if they are part of the certificate. **Note:** Do not change the CSR in any way. A public key can be included with the CSR and should not be replaced by the private key.|
|Notes                        | Any notes regarding the SSL certificate that might be helpful to other users.|
{: caption="Table 1. SSL certificate details" caption-side="top"}

## Next steps
{: #ns-viewing-and-updating-ssl-certificates}

After updating the details for the SSL certificate, any products or services that use the certificate will not be negatively impacted by the change. The certificate can be updated again at any time by repeating the previous steps.
