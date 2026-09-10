\# Cisco Networking \& Security Labs 🛡️



Hands-on Cisco networking and network security labs developed using

Cisco Packet Tracer.



This repository documents my progression from foundational enterprise

networking to network security hardening and secure enterprise topology

design.



\---



\## 📚 Lab Portfolio



\### 01 — Basic Enterprise Network



Foundational enterprise networking implementation covering:



\- Cisco switching and routing

\- VLAN configuration

\- IP addressing

\- Inter-VLAN connectivity

\- Basic network troubleshooting

\- Cisco Packet Tracer topology design



\---



\### 02 — Enterprise Network Security



Enterprise networking with security-focused configuration and

segmentation.



Key areas:



\- VLAN segmentation

\- 802.1Q trunking

\- Inter-VLAN routing

\- DHCP

\- Access control

\- SSH

\- Network security fundamentals

\- Connectivity verification



\---



\### 03 — Enterprise Network Security Hardening



Network hardening lab focused on Layer 2 security and switch

protection.



Key security controls include:



\- VLAN segmentation

\- Secure trunking

\- Native VLAN hardening

\- STP security

\- Port Security

\- Sticky MAC addresses

\- BPDU Guard

\- DHCP Snooping

\- Dynamic ARP Inspection

\- Unused-port hardening

\- Management VLAN

\- Security verification and troubleshooting



\---



\### 04 — Enterprise Network Topology \& Security



Advanced enterprise topology integrating networking and security

controls into a larger simulated environment.



\### VLAN Architecture



| VLAN | Department | Network |

|------|------------|---------|

| 10 | HR | 192.168.10.0/24 |

| 20 | IT | 192.168.20.0/24 |

| 30 | Finance | 192.168.30.0/24 |

| 40 | Sales | 192.168.40.0/24 |

| 50 | Servers | 192.168.50.0/24 |

| 99 | Management | 192.168.99.0/24 |

| 999 | Native / Unused | Lab security VLAN |



\### Inter-VLAN Gateways



\- VLAN 10 → 192.168.10.1

\- VLAN 20 → 192.168.20.1

\- VLAN 30 → 192.168.30.1

\- VLAN 40 → 192.168.40.1

\- VLAN 50 → 192.168.50.1

\- VLAN 99 → 192.168.99.1



\### Security Focus



\- Network segmentation

\- Secure trunking

\- STP security

\- Port Security

\- DHCP Snooping

\- Dynamic ARP Inspection

\- Management VLAN

\- Unused-port isolation

\- Network hardening

\- Security verification



\---



\## 🧰 Technologies \& Tools



\- Cisco Packet Tracer

\- Cisco IOS

\- VLANs

\- 802.1Q Trunking

\- Inter-VLAN Routing

\- DHCP

\- STP

\- Port Security

\- DHCP Snooping

\- Dynamic ARP Inspection

\- SSH

\- ACL fundamentals

\- NAT fundamentals

\- TCP/IP

\- Network troubleshooting



\---



\## 🔍 Verification \& Evidence



Each lab contains configuration files, Packet Tracer projects,

screenshots, and verification evidence where applicable.



Examples of verification commands:



```text

show vlan brief

show interfaces trunk

show ip interface brief

show ip route

show ip dhcp binding

show spanning-tree

show port-security

show ip dhcp snooping

show ip arp inspection

