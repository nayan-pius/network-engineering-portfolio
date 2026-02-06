# Day 3: Inter-Network Routing

**Date:** Feb 5, 2026
**Focus:** Layer 3 Routing & Default Gateways

### 🎯 Objective
To connect two separate networks (192.168.1.0/24 and 192.168.2.0/24) using a Router so they can communicate.

### 🛠️ Topology
![Router Lab](../../diagrams/day03-router-lab.png)

### ⚙️ Configuration
* **Router Interface G0/0/0:** 192.168.1.1 (Gateway for LAN A)
* **Router Interface G0/0/1:** 192.168.2.1 (Gateway for LAN B)

### 🧠 Key Learnings
* **Default Gateway:** The IP address of the router interface that allows a device to leave its local network.
* **"no shutdown":** Router ports are off by default; you must manually turn them on.
* **Routing Table:** The router automatically knows about networks directly connected to it.