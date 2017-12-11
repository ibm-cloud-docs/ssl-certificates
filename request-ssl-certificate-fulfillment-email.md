---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Requesting an SSL certificate fulfillment email

## Overview

After ordering a new SSL certificate through {{site.data.keyword.BluSoftlayer_full}}, the certificate authority sends a fulfillment email to the domain administrator provided during the ordering process. This email contains all details associated with the SSL certificate. At any time, the fulfillment email may be requested again from the SSL Orders screen on the {{site.data.keyword.slportal_full}}. Follow the steps below to request the SSL fulfillment email from the certificate authority.

## Requesting a fulfillment email

1. Access the [{{site.data.keyword.slportal_full}} ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/){: new_window} by using your unique credentials.
2. From the **Security** menu, select **SSL > Orders**.
3. Click the **Send** link in the **Email** column for the desired SSL certificate.<br/>**Note:** A pop-up window appears to confirm the request. This window contains the email address for the Domain Administrator that was provided when the SSL certificate was requested.
4. Click the **Resend Email** button to confirm the selection and request an additional fulfillment email from the certificate authority.  Or, click **Cancel** to cancel the action.

## What Happens Next

After requesting an additional fulfillment email, the request will be forwarded to the applicable certificate authority for completion. Because SSL certificate details are confidential, {{site.data.keyword.BluSoftlayer_notm}} does not store the SSL certificate data on our system. After receiving the SSL certificate details via email, they may be manually [imported](import-ssl-certificate.html) to the {{site.data.keyword.slportal}}, if necessary.
