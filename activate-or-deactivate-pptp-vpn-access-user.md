---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-16"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Activating or deactivating PPTP VPN access

## Overview

PPTP VPN allows users to form a secure tunnel to the {{site.data.keyword.BluSoftlayer_full}} private network using specialized client software running on their desktop or dedicated device.  PPTP access is designed for customers who need to connect an entire office or cannot use the SSL VPN solution. Each customer is allotted one PPTP connection with additional connections available but requesting support to enable unlimited PPTP access, which is available at no additional charge. To activate or deactivate PPTP VPN access for a user, complete the following steps.

## Activating or Deactivating PPTP VPN access

1. Access the [{{site.data.keyword.slportal_full}} ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/){: new_window} by using your unique credentials as an administrator.
2. Locate the user whose access you'd like to modify and view the **VPN access** column to view their current access level.
3. From the **Actions** menu, select **Edit VPN access**.
4. Enter the VPN type and subnet access details.

|Field Name  |Options   |
| -----------| ------------ |
| VPN Type   | None, SSL, PPTP, or both (SSL and PPTP) |
|Subnet Access | Auto or Manual |           
{: caption="Table 1. Edit VPN access options" caption-side="top"}   
5. Click **Save** to save your changes.

   **Note:** PPTP access must be activated in order for a user to connect using PPTP.
