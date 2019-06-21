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

# 激活或取消激活 PPTP VPN 访问权
{: #activating-or-deactivating-pptp-vpn-access}

PPTP VPN 允许您通过使用在您桌面或专用设备上运行的专用客户机软件，构成 {{site.data.keyword.cloud}} 专用网络的安全通道。如果您需要连接整个办公室或无法使用 SSL VPN 解决方案，PPTP 访问权是专为您的需求而设计的。同时将分配给您一个 PPTP 连接，其中包含更多可用连接，您也可以请求支持，以启用不受限的 PPTP 访问权，而无需额外费用。要激活或取消激活用户的 PPTP VPN 访问权，请完成以下步骤。
{:shortdesc}

1. 登录到 {{site.data.keyword.cloud_notm}} 控制台中的[访问权 (IAM)](https://cloud.ibm.com/iam/overview){: external} 页面。
2. 找到要修改其访问权的用户，并查看 **VPN 访问权**列以查看其当前访问级别。
3. 从**操作**菜单中，选择**编辑 VPN 访问权**。
4. 输入 VPN 类型和子网访问权详细信息，然后单击**保存**以保存更改。请参阅下表以了解更多信息。

|字段名称|选项   |
| -----------| ------------ |
|VPN 类型 |无、SSL、PPTP 或两者（SSL 和 PPTP）|
|子网访问权|自动或手动|           
{: caption="表 1. VPN 和子网详细信息" caption-side="top"}   

必须激活 PPTP 访问权，用户才能使用 PPTP 进行连接。
{:note}
