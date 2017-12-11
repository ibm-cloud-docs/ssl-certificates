---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-17"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Viewing and updating SSL certificates

After an SSL certificate has been imported to the SSL certificates screen, you can view and update them at any time. Updates work similar to the [import process](import-ssl-certificate.html), as all details that are updated must match the original certificate exactly, including spacing and line breaks.

To view and update an SSL certificate, complete the following steps.

1. Access the [{{site.data.keyword.slportal_full}} ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/){: new_window} by using your unique credentials.
2. From the **Security** menu, select **SSL > Certificates**.
2. Select **View/Update certificate** from the **Actions** drop down list.
3. Update the **SSL certificate details** in the applicable text boxes.

   **Note:** Details entered in the **Import SSL certificate** window must be entered exactly as provided by the certificate authority, including spacing and line breaks. If not, an error occurs.

| Text Box | Entry |
| -------- | ----- |
|Certificate |SSL certificate details, provided by the certificate authority. This is generally an alpha-numeric block of text.|
|Private Key | Private Key details for the certificate, provided by the certificate authority. This is generally an alpha-numeric block of text.|
|Intermediate Certificate | Intermediate certificate details, provided by the certificate authority. Intermediate certificates are not required, however, if the information is available for the SSL certificate, it should be entered.|
| Certificate Signing Request | Certificate Signing Request (CSR) details, provided by the certificate authority. CSR details are not required, but should be provided if they are part of the certificate. **Note:** Do not change the CSR in any way. A public key may be included with the CSR and should not be replaced by the Private Key.|
|Notes | Any notes regarding the SSL certificate that may be helpful to other users.
Click **Update** to update the SSL certificate or click **Cancel** to cancel the action.

## Next Steps

After updating the details for the SSL certificate, any products or services that use the certificate will not be negatively impacted by the change. The certificate may be updated again at any time by repeating the steps above.
