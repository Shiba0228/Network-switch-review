NVEDIA SN2201 Ethernet Switch
a. Introduction:
SN2201是由NVIDIA推出的1GbE管理型Ethernet Switch，屬於 Spectrum Ethernet switch 系列的低速管理交換器，通常用於資料中心管理網路（Management Network），而不是高頻寬資料傳輸。是 Out-of-Band (OOB) 管理網路。
    在 AI / HPC / Server Rack 架構中，它常被用來連接：
    BMC (Baseboard Management Controller)
    IPMI 管理埠
    管理 PC / 管理網路
    Switch / Storage 管理 port

![alt text](<sn2201 switch-1.jpg>)


Specification of SN2201:
    Switch Type	Layer:      2 Managed Switch
    Ethernet Port:	        48 × 1GbE RJ45
    Uplink Port:            4 × 10GbE SFP+
    Switching Capacity:  	176 Gbps
    Management:	            CLI / Web / SNMP
    Console:	            RJ45 Console
    OS:                 	NVIDIA Onyx or MLNX-OS
    Mount:	                1U Rack Mount

Port Layout:
    1–48:	                1GbE RJ45
    49–52:	                10GbE SFP+ uplink
    Console:	            CLI management
    Mgmt:	                OOB management
    48 ports → server / BMC / device
    4 uplink → 上層 switch / core network

SN2201在Rack架構中的角色:
(I) Classic AI Server Rack：
    Management Network
         │
    Core Switch
         │
    ┌───────────┐
    │  SN2201   │
    └───────────┘
    │ │ │ │ │ │
    │ │ │ │ │ │
    BMC BMC BMC BMC
    GPU GPU GPU GPU
    Server Server Server
(II)SN2201 負責：
    所有 server BMC 管理網路
    FW update
    Monitoring
    IPMI / Redfish
    SSH management

常見管理方式:
    (I)Console 連線
    (II)SSH manement
    (III)Web UI

常用基本指令:



