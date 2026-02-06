## 📅 Day 03: Crossing Boundaries (Routing)
**Date:** February 5, 2026
**Focus:** Layer 3 Routing & Default Gateways

### 📝 Summary
Today I moved up the OSI stack to **Layer 3**. I connected two separate networks (`192.168.1.0` and `192.168.2.0`) using a Cisco Router. This required understanding that a Switch cannot forward traffic between different IP subnets.

### 💡 Key Learnings
* **The Default Gateway:** This is the specific IP address of the router interface connected to the local network. It acts as the "door" out of the room. Without it, a PC is trapped in its own LAN.
* **Router Interfaces:** Unlike switch ports, router interfaces are `shutdown` (off) by default. I must manually run `no shutdown`.
* **The "ARP Delay":** I noticed the first ping to a new network often times out. This is because the router is busy using ARP to find the destination MAC address.

### 🔧 Troubleshooting
* **Issue:** PC-A could not ping PC-B initially.
* **Fix:** I realized I hadn't set the Default Gateway on the PCs. Once I added the Router's IP (`192.168.1.1`) to the PC settings, the traffic flowed.