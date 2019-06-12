---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: PPTP VPN access, PPTP VPN, PPTP access

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:external: target="_blank" .external}

# Activating or deactivating PPTP VPN access
{: #activating-or-deactivating-pptp-vpn-access}

PPTP VPN allows you to form a secure tunnel to the {{site.data.keyword.cloud}} private network by using specialized client software that runs on your desktop or dedicated device. PPTP access is designed if you need to connect an entire office or cannot use the SSL VPN solution. You are allotted one PPTP connection with more connections available, and you can request support to enable unlimited PPTP access, which is available at no additional charge. To activate or deactivate PPTP VPN access for a user, complete the following steps.
{:shortdesc}

1. Log in to the [Access (IAM)](https://cloud.ibm.com/iam/overview){: external} page in the {{site.data.keyword.cloud_notm}} console.
2. Locate the user whose access you'd like to modify and view the **VPN access** column to view their current access level.
3. From the **Actions** menu, select **Edit VPN access**.
4. Enter the VPN type and subnet access details, and click **Save** to save your changes. See the following table for more information.

|Field Name  |Options   |
| -----------| ------------ |
| VPN Type   | None, SSL, PPTP, or both (SSL and PPTP) |
| Subnet Access | Auto or manual |           
{: caption="Table 1. VPN and subnet details" caption-side="top"}   

PPTP access must be activated in order for a user to connect by using PPTP.
{:note}
