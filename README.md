# 🛡️ Cisco Networking & Security Labs

> A hands-on cybersecurity and enterprise networking portfolio built with **Cisco Packet Tracer**, focused on network architecture, VLAN segmentation, routing, switching, security hardening, and SOC-relevant security controls.

![Cisco](https://img.shields.io/badge/Cisco-Packet%20Tracer-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white)
![Networking](https://img.shields.io/badge/Networking-TCP%2FIP-blue?style=for-the-badge)
![Security](https://img.shields.io/badge/Cybersecurity-Network%20Security-red?style=for-the-badge)
![GitHub](https://img.shields.io/badge/GitHub-Portfolio-black?style=for-the-badge&logo=github)

---

## 📌 About This Repository

This repository contains a collection of hands-on **Cisco networking and network security labs** developed as part of my cybersecurity learning journey toward becoming a **SOC Analyst**.

The labs progress from fundamental enterprise networking concepts to security-focused network architecture and hardening.

The primary objective is to understand how enterprise networks are:

- Designed
- Segmented
- Configured
- Secured
- Monitored
- Troubleshot
- Verified

The projects also provide practical exposure to concepts that are highly relevant to **SOC operations**, including network traffic, segmentation, access control, authentication, DHCP, STP security, endpoint protection, and security verification.

---

# 🎯 Learning Objectives

Through these labs, I worked on:

- Enterprise network topology design
- VLAN segmentation
- Access and trunk port configuration
- Inter-VLAN routing
- Router-on-a-stick
- DHCP configuration
- Static and dynamic addressing
- Network device configuration
- Switch security
- Port security
- MAC address security
- STP security
- Root Guard
- BPDU Guard
- PortFast
- DHCP Snooping concepts
- Dynamic ARP Inspection concepts
- Unused-port hardening
- Management VLAN design
- Native VLAN security
- WAN/ISP simulation
- Network troubleshooting
- Configuration verification
- Security evidence collection

---

# 🏗️ Repository Projects

## 01 — Basic Enterprise Network

**Location:** `01-Basic-Enterprise-Network/`

A foundational enterprise networking environment designed to build practical understanding of Cisco switching, VLANs, addressing, and connectivity.

### Key Concepts

- Cisco switching
- VLAN configuration
- Access ports
- Trunking
- IP addressing
- Basic routing
- Host connectivity
- Network troubleshooting

### Objective

Build a functional enterprise network and establish reliable communication between network segments.

---

# 🔐 02 — Enterprise Network Security

**Location:** `02-Enterprise-Network-Security/`

This project introduces security-focused configurations into an enterprise network environment.

### Key Concepts

- Network segmentation
- Secure switch configuration
- Access control
- Device hardening
- Secure management concepts
- Network security fundamentals
- Configuration verification

### Objective

Understand how basic enterprise networks can be strengthened against common network-level security risks.

---

# 🛡️ 03 — Enterprise Network Security Hardening

**Location:** `03-Enterprise-Network-Security-Hardening/`

This project focuses on practical switch-level security hardening.

### Security Controls

- Port Security
- Sticky MAC addresses
- MAC address limits
- Violation modes
- PortFast
- BPDU Guard
- STP security
- Root Guard
- DHCP security concepts
- Unused-port shutdown
- VLAN isolation
- Native VLAN security
- Management VLAN
- Endpoint protection

### Objective

Reduce the attack surface of an enterprise switching environment by applying layered security controls.

---

# 🏢 04 — Enterprise Network Topology & Security

**Location:** `04-Enterprise-Network-Topology-Security/`

This is the most comprehensive project in the repository.

It combines enterprise topology design, VLAN segmentation, routing, DHCP, switching, security hardening, and verification into a single simulated environment.

### Enterprise VLAN Architecture

| VLAN | Department / Purpose | Network |
|---|---|---|
| 10 | HR | `192.168.10.0/24` |
| 20 | IT | `192.168.20.0/24` |
| 30 | Finance | `192.168.30.0/24` |
| 40 | Sales | `192.168.40.0/24` |
| 50 | Servers | `192.168.50.0/24` |
| 99 | Management | `192.168.99.0/24` |
| 999 | Unused / Blackhole / Native | Security VLAN |

### Default Gateways

| VLAN | Gateway |
|---|---|
| HR | `192.168.10.1` |
| IT | `192.168.20.1` |
| Finance | `192.168.30.1` |
| Sales | `192.168.40.1` |
| Servers | `192.168.50.1` |
| Management | `192.168.99.1` |

---

# 🌐 Network Architecture

The topology consists of:

```text
                         ┌──────────────┐
                         │     ISP      │
                         └──────┬───────┘
                                │
                           Simulated WAN
                                │
                         ┌──────┴───────┐
                         │    EDGE-R1   │
                         │ Router/Layer │
                         │   3 Gateway   │
                         └──────┬───────┘
                                │
                             Trunk
                                │
                         ┌──────┴───────┐
                         │   CORE-SW    │
                         │ Cisco 3650   │
                         └──────┬───────┘
                                │
       ┌────────────┬───────────┼───────────┬────────────┐
       │            │           │           │            │
   ┌───┴───┐    ┌───┴───┐   ┌──┴───┐   ┌──┴────┐   ┌───┴────┐
   │ HR-SW │    │ IT-SW │   │FIN-SW│   │SALES-SW│  │SERVER-SW│
   └───────┘    └───────┘   └──────┘   └────────┘  └─────────┘
