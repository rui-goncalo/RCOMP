# RCOMP 2021-2022 Project - Sprint 2 planning
<hr>
## Sprint master: Hugo Carvalho - 1210813
<hr>
# Data
* VTP domain name: **rc22dkg3**
* VLANID range: **400-430**
* IPv4 address space: **172.17.224.0/21**
* ISP router IPv4 node address: **15.203.48.93/30**

<hr>

# Sprint Backlog

| Task Number | Assignee | Task Description |
| -|-|-|
| 2.1 |  1210813 | Development of a layer two and layer three Packet Tracer simulation for building one, encompassing the campus backbone.<br>Integration of every member's Packet Tracer simulation into a single simulation. |
| 2.2 |  1191831 | Development of a layer two and layer three Packet Tracer simulation for building two, encompassing the campus backbone. |
| 2.3 |  1201694 | Development of a layer two and layer three Packet Tracer simulation for building three, encompassing the campus backbone. |

# Technical decisions and coordination
* Packet Tracer Version: **8.1.1.0022**

<hr>

* VLANSs Distribuition:
    * Building 1: **400-405**
    * Building 2: **406-410**
    * Building 3: **411-415**

<hr>

* Device naming conventions
    * Main Cross-connect: **"MC"**
    * Intermidiate Cross-connect: **"IC - Building X"**
    * Horizontal Cross-connect: **"HC - Building X Floor X"**
    * Consolidation Points: **"CPX - Building X Floor X"**
    <br><br>
    * PC: **"PC - Building X Floor X"**
    * IP Phone: **"Phone - Building X Floor X"**
    * Server: **"Server - Building X Floor X"**
    * Routers:
        * ISP: **"Router - ISP"**
        * Main: **"Router - Main"**
        * Building Specific: **"Router - Building X"**

<hr>

* VLAN naming conventions:
    * Backbone: **"V_Backbone"**
    * Wi-Fi network: **"V_WiFi_BuildingX"**
    * End user outlets on the ground floor: **"V_Floor0_BuildingX"**
    * End user outlets on the first floor: **"V_Floor1_BuildingX"**
    * VoIP: **"V_VoIP_BuildingX"**
    * DMZ: **"V_DMZ_BuildingX"**

<hr>
# IPv4 Networks
## Backbone
| Network Adress | Network Mask | Router Name | IP Address |
| -|-|-|-|
| 15.203.48.92/30 | 255.255.255.252 | Router - ISP | 15.203.48.93 |
| | | Router - Main | 15.203.48.94 |

| Router Name | IP Address |
| -|-|
| Router - Main | 172.17.224.1 |
| Router - Building 1 | 172.17.224.2 |
| Router - Building 2 | 172.17.224.3 |
| Router - Building 3 | 172.17.224.4 |

## Building 1

| Network Address | Network Mask | First IP Adress | Last IP Adress | Broadcast | VLAN IDs | VLAN Name |
| -|-|-|-|-|-|-|
| 172.17.224.0/25 | 255.255.255.128 | 172.17.224.1 | 172.17.224.126 | 172.17.224.127 | 400 | V_Backbone
| 172.17.224.128/25 | 255.255.255.128 | 172.17.224.129 | 172.17.224.254 | 172.17.224.255 | 401 | V_WiFi_Building1
| 172.17.225.0/25 | 255.255.255.128 | 172.17.225.1 | 172.17.225.126 | 172.17.225.127 | 402 | V_Floor0_Building1
| 172.17.225.128/25 | 255.255.255.128 | 172.17.225.129 | 172.17.225.254 | 172.17.225.255 | 403 | V_Floor1_Building1
| 172.17.226.0/26 | 255.255.255.192 | 172.17.226.1 | 172.17.226.62 | 172.17.226.63 | 404 | V_VoIP_Building1
| 172.17.226.64/26 | 255.255.255.192 | 172.17.226.65 | 172.17.226.126 | 172.17.226.127 | 405 | V_DMZ_Building1

## Building 2

| Network Address | Network Mask | First IP Adress | Last IP Adress | Broadcast | VLAN IDs | VLAN Name |
| -|-|-|-|-|-|-|
| 172.17.226.128/25 | 255.255.255.128 | 172.17.226.129 | 172.17.226.254 | 172.17.226.255 | 406 | V_WiFi_Building2
| 172.17.227.0/26 | 255.255.255.192 | 172.17.227.1 | 172.17.227.62 | 172.17.227.63 | 407 | V_Floor1_Building2
| 172.17.227.64/27 | 255.255.255.224 | 172.17.227.65 | 172.17.227.94 | 172.17.227.95 | 408 | V_Floor0_Building2
| 172.17.227.96/28 | 255.255.255.240 | 172.17.227.97 | 172.17.227.110 | 172.17.227.111 | 409 | V_VoIP_Building2
| 172.17.227.112/28 | 255.255.255.240 | 172.17.227.113 | 172.17.227.126 | 172.17.227.127 | 410 | V_DMZ_Building2

## Building 3

| Network Address | Network Mask | First IP Adress | Last IP Adress | Broadcast | VLAN IDs | VLAN Name |
| -|-|-|-|-|-|-|
| 172.17.227.128/26 | 255.255.255.192 | 172.17.227.129 | 172.17.227.190 | 172.17.227.191 | 411 | V_WiFi_Building3
| 172.17.227.192/26 | 255.255.255.192 | 172.17.227.193 | 172.17.227.254 | 172.17.227.255 | 412 | V_Floor1_Building3
| 172.17.228.0/26 | 255.255.255.192 | 172.17.228.1 | 172.17.228.62 | 172.17.228.63 | 413 | V_Floor0_Building3
| 172.17.228.64/27 | 255.255.255.224 | 172.17.228.65 | 172.17.228.94 | 172.17.228.95 | 414 | V_VoIP_Building3
| 172.17.228.96/27 | 255.255.255.224 | 172.17.228.97 | 172.17.228.126 | 172.17.228.127 | 415 | V_DMZ_Building3