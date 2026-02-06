## 📅 Day 02: The Switch "Brain" (Switching)
**Date:** February 3, 2026
**Focus:** Layer 2 Switching & MAC Addresses

### 📝 Summary
I built a Small Office LAN using a Cisco 2960 Switch. The goal was to understand how a central device manages traffic between multiple computers without causing collisions.

### 💡 Key Learnings
* **MAC Address Table:** I used the command `show mac address-table`. It was fascinating to see the switch "learn" dynamically. Initially, the table was empty, but as soon as I sent a ping, the switch recorded the Source MAC and the Port it came from.
* **Layer 2 Logic:** Switches don't care about IP addresses; they deliver mail based on the physical MAC address (Hardware ID).

### 🔧 Troubleshooting
* **Scenario:** I tried connecting a PC to the Switch with a Crossover cable just to see what happened.
* **Result:** In the simulation, it worked (due to Auto-MDIX), but I noted that in a strict physical environment, a **Straight-Through** cable is the correct choice for different device types (PC to Switch).