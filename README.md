
# 🌐 Bonalbo Branch Network Design
### **Enterprise-Grade VLAN Segmentation & Inter-VLAN Routing**

[![Cisco Packet Tracer](https://img.shields.io/badge/Lab-Cisco%20Packet%20Tracer-blue?style=flat-square&logo=cisco)](https://www.netacad.com/)
[![Networking](https://img.shields.io/badge/Focus-Network%20Infrastructure-green?style=flat-square)](https://www.cisco.com)

## 🚀 Project Overview
This project presents a simulated branch network design for **XYZ Company’s expansion in Bonalbo**, developed using **Cisco Packet Tracer**. The architecture transitions the branch from a flat network to a modern, segmented infrastructure to improve security, manageability, and performance.

The design focuses on **VLAN isolation**, **Router-on-a-Stick (RoaS) routing**, and **automated IP management** to ensure a professional, scalable environment.

---

## 🏢 Scenario & Objectives
XYZ Company requires an independent network for its new Bonalbo location. The infrastructure must support three distinct departments while maintaining centralized management.

**Key Objectives:**
* **Segmentation:** Group users logically to minimize broadcast domains.
* **Automation:** Implement DHCP to eliminate manual IP configuration.
* **Connectivity:** Enable Inter-VLAN routing for cross-departmental resource sharing.
* **Mobility:** Provide integrated Wireless LAN (WLAN) access.

---

## 🛠️ Technical Architecture

### 🖧 Logical Topology
The network utilizes a **Router-on-a-Stick** configuration. A single physical link between the Switch and Router is partitioned into logical sub-interfaces to act as the default gateway for each VLAN.

### 🔹 Network Segmentation Table
| Department | VLAN ID | Subnet | Gateway |
| :--- | :---: | :--- | :--- |
| **Admin / IT** | 10 | `192.168.1.0/26` | `192.168.1.1` |
| **Finance / HR** | 20 | `192.168.1.64/26` | `192.168.1.65` |
| **CS / Reception** | 30 | `192.168.1.128/26` | `192.168.1.129` |
| **Management (Native)** | 99 | `192.168.1.192/26` | `192.168.1.193` |

---

### 1. Inter-VLAN Routing (Sub-Interfaces)

📶 Key Features Implemented

✅ VLAN Segmentation: Enhanced security by isolating department traffic.

✅ Router-on-a-Stick: Efficient routing using minimal physical hardware.

✅ Dynamic Addressing: DHCP pools configured for all subnets.

✅ Wireless Integration: Seamless Wi-Fi connectivity for mobile end-devices.

✅ ICMP Verification: Validated end-to-end connectivity across the entire branch.

✅ Outcome
The Bonalbo Branch network is fully operational. All departments receive automated IP configurations, and cross-VLAN communication is successful. The design is highly scalable, allowing the company to add more users or departments with minimal configuration changes.

👨‍💻 Author
Hiru Ranasinghe Undergraduate – Computer Networks NSBM Green University
