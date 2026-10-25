<img width="1362" height="726" alt="image" src="https://github.com/user-attachments/assets/a78ad40a-b7ad-4a25-b193-2962c62f4aab" /># CSE421 Final Project — Multi-Site Network Design (Cisco Packet Tracer)

Final project for **CSE421: Computer Networks**, BRAC University.

![Network Topology](topology.png)

## Overview
A multi-site enterprise network connecting **six branch sites**, each with its own
router, switch, end devices and local servers. Four sites (DC, RHC, PH, MH) are
interconnected through a central backbone switch, while MH, ERU and RI are linked
by a triangle of **serial WAN links** for redundancy. The network provides
centralized DNS and web services along with per-site email and DHCP servers.

## Network Sites
| Site | Router | Switch | End Devices | Servers |
|------|--------|--------|-------------|---------|
| DC   | DC   | DC-SW   | PC1-DC, PC2-DC   | Email-DC |
| RHC  | RHC  | RHC-SW  | PC1-RHC, PC2-RHC | Email-RHC, DHCP-RHC |
| PH   | PH   | PH-SW   | PC1-PH, PC2-PH   | Email-PH, DHCP-PH |
| MH   | MH   | MH-SW   | PC1-MH, PC2-MH   | DNS, WEB, Email-MH |
| ERU  | ERU  | ERU-SW  | PC1-ERU, PC2-ERU | Email-ERU |
| RI   | RI   | RI-SW   | PC1-RI, PC2-RI   | Email-RI |

## Features
- **Backbone:** DC, RHC, PH and MH routers connected through `CENTRAL-SW`
- **WAN:** Serial links forming a redundant triangle between MH, ERU and RI
- **DHCP:** Dynamic IP assignment from DHCP servers at RHC and PH
- **DNS & Web:** Centralized DNS and web server at the MH site
- **Email:** Dedicated email server at every site
- **Routing:** [Routing protocol, e.g. OSPF / RIP / EIGRP / static]

## Devices Used
- **Routers:** 6 × Cisco 2911
- **Switches:** 7 × Cisco Catalyst 2960-24TT (6 site switches + 1 central switch)
- **PCs:** 12 (2 per site)
- **Servers:** 10 (1 DNS, 1 Web, 6 Email, 2 DHCP)

## How to Open
1. Install [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer)
2. Download `CSE421_Final_Project.pkt`
3. Open it in Packet Tracer

## Author
- Group project
