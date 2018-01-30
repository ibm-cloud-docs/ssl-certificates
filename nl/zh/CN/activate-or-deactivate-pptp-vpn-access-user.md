---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-16"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 激活或取消激活 PPTP VPN 访问权

## 概述

PPTP VPN 允许用户通过使用在其桌面或专用设备上运行的专用客户机软件，构成 {{site.data.keyword.BluSoftlayer_full}} 专用网络的安全通道。PPTP 访问权专为需要连接整个办公室或无法使用 SSL VPN 解决方案的客户而设计。每个客户都将分配一个 PPTP 连接，其中包含其他可用连接，但会请求支持，以启用不受限的 PPTP 访问权，而无需额外收费。要激活或取消激活用户的 PPTP VPN 访问权，请完成以下步骤。

## 激活或取消激活 PPTP VPN 访问权

1. 通过以管理员身份使用唯一凭证来访问 [{{site.data.keyword.slportal_full}} ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://control.softlayer.com/){: new_window}。
2. 找到要修改其访问权的用户，并查看 **VPN 访问权**列以查看其当前访问级别。
3. 从**操作**菜单中，选择**编辑 VPN 访问权**。
4. 输入 VPN 类型和子网访问权详细信息。

|字段名称|选项   |
| -----------| ------------ |
| VPN 类型 | 无、SSL、PPTP 或两者（SSL 和 PPTP）|
|子网访问权| 自动或手动|           
{: caption="表 1. 编辑 VPN 访问权选项" caption-side="top"}   
5. 单击**保存**以保存更改。

   **注：**必须激活 PPTP 访问权，用户才能使用 PPTP 进行连接。
