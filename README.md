# network-infrastructure-lab
CCNA-style VLANs + Inter-VLAN routing + subnetting + DHCP + basic ACL
# Network Infrastructure Lab (CCNA)

## Overview
This lab demonstrates a small enterprise-style network with segmentation using VLANs, inter-VLAN routing (router-on-a-stick), DHCP, and basic access control. Built to reinforce CCNA networking fundamentals.

## Goals
- Create multiple VLANs for network segmentation
- Implement trunking between switch and router
- Configure inter-VLAN routing (802.1Q)
- Provide IP addresses via DHCP
- Validate connectivity with ping and troubleshooting steps
- Add a basic ACL to restrict inter-VLAN access (optional)

## Topology
- 1x Router (R1)
- 1x Switch (S1)
- 3x VLANs (example: Users, Admin, Guest)

## VLAN Plan (Example)
| VLAN | Name  | Subnet           | Gateway          |
|------|-------|------------------|------------------|
| 10   | USERS | 192.168.10.0/24  | 192.168.10.1     |
| 20   | ADMIN | 192.168.20.0/24  | 192.168.20.1     |
| 30   | GUEST | 192.168.30.0/24  | 192.168.30.1     |

## What’s Included
- Subnetting plan
- Cisco IOS-style configs (switch + router)
- Validation steps and expected results

## Validation Checklist
- [ ] VLANs created and ports assigned correctly
- [ ] Trunk configured between S1 and R1
- [ ] Router subinterfaces configured with dot1q encapsulation
- [ ] DHCP pools created and working
- [ ] End devices receive correct IP configuration
- [ ] Successful ping tests within and across VLANs
- [ ] (Optional) ACL blocks GUEST → ADMIN

## Author
Yordanos Mekonnen  
CCNA Certified | OSCP Candidate  
GitHub: https://github.com/YOTOMAN1012
