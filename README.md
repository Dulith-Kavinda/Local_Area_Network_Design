# University of Moratuwa Campus LAN Design (EN2150)

This repository contains the design, technical specifications, and simulation files for a campus-wide Local Area Network (LAN) for the University of Moratuwa. The project was developed as part of the **EN2150 Communication Network Engineering** course, focusing on a high-availability backbone and a detailed internal network for the Department of Electronic and Telecommunication Engineering (ENTC).

## 📌 Project Overview

The network is engineered to support a 20-25 year operational lifespan with a focus on scalability, redundancy, and performance.

### 1. University Backbone Network
* **Topology**: Distributed ring architecture with redundant shortcut links to ensure low latency and high resilience.
* **Capacity**: 10 Gbps Single-Mode Fiber (OS2) backbone.
* **Protocols**: OSPF dynamic routing for rapid failover (reconvergence under 40 seconds) and dual-stack IPv4/IPv6 addressing.
* **Scope**: Interconnects 12 major building nodes across the campus.

### 2. ENTC Building Internal LAN
* **Architecture**: Two-tier hierarchical design (Core and Access layers).
* **VLAN Configuration**: Segmented traffic for Staff, Students, and Laboratories.
* **Wireless Infrastructure**: High-density Wi-Fi coverage managed by a centralized Wireless LAN Controller (WLC).
* **Cabling**: TIA-568-C compliant cabling with Cat6A for horizontal distribution and OM4 Multi-Mode Fiber for vertical risers.

## 🛠️ Technology Stack

### Network Hardware
* **Core/Distribution**: Cisco Catalyst 3650-24PS (Layer 3 switches with PoE+).
* **Access Layer**: Cisco Catalyst 2960-24TT (Layer 2 switches).
* **Security**: Cisco Firepower 2110 Next-Generation Firewall (NGFW) and Cisco 2911 ISR routers.
* **Wireless**: Cisco 3702i Lightweight Access Points and Cisco WLC-2504.

### Design & Simulation
* **Simulation Tool**: Cisco Packet Tracer.
* **Addressing**: 
    * IPv4: 172.16.0.0/16
    * IPv6: 2400:ee00:1000::/48

## 📂 Repository Structure

* `/Report.pdf`: Comprehensive design document including link budget analysis and addressing schemes.
* `/Simulations`: `.pkt` files containing the logical and physical topologies.
* `/Schematics`: Detailed diagrams of the backbone ring and building-level hierarchy.

## 👥 Team Synex

* Amarasinghe A.A.D.K.
* Bandara W.D.A.C.
* Dissanayake R.K.T.
* Tennakoon U.G.R.B.

---
*Submitted to the Department of Electronic & Telecommunication Engineering, University of Moratuwa.*
