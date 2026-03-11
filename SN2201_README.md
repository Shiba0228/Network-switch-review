NVIDIA SN2201 Ethernet Switch
a. Introduction

SN2201 是由 NVIDIA 推出的 1GbE 管理型 Ethernet Switch，屬於 Spectrum Ethernet Switch 系列的低速管理交換器。
通常用於 資料中心管理網路（Management Network），而不是高頻寬資料傳輸。

SN2201 屬於 Out-of-Band (OOB) 管理網路設備。

在 AI / HPC / Server Rack 架構中，它常被用來連接：

BMC (Baseboard Management Controller)

IPMI 管理埠

管理 PC / Management Network

Switch / Storage 管理 Port



Specification of SN2201
Item	Specification
Switch Type	Layer 2 Managed Switch
Ethernet Port	48 × 1GbE RJ45
Uplink Port	4 × 10GbE SFP+
Switching Capacity	176 Gbps
Management	CLI / Web / SNMP
Console	RJ45 Console
OS	NVIDIA Onyx / MLNX-OS
Mount	1U Rack Mount
Port Layout
Port	Function
1–48	1GbE RJ45
49–52	10GbE SFP+ uplink
Console	CLI Management
Mgmt	OOB Management

Port usage:

48 ports → Server / BMC / Device

4 uplink → 上層 Switch / Core Network

SN2201 在 Rack 架構中的角色
(I) Classic AI Server Rack

(II) SN2201 負責功能

SN2201 主要負責：

所有 Server BMC 管理網路

Firmware Update

Monitoring

IPMI / Redfish Management

SSH Remote Management

常見管理方式

SN2201 支援多種管理方式：

Console 連線

SSH Management

Web UI

常用基本指令

常見的 SN2201 CLI 指令：

show version
show interfaces status
show vlan
show mac-address-table




