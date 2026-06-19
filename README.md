# 🏦 Secure Financial Multi-Branch Banking Hub

A fully designed and simulated enterprise banking network built from scratch 
using Cisco Packet Tracer — connecting two bank branches, an HQ, and a 
Central Bank with real-world security and routing configurations.

---

## 🛠️ Tools & Technologies
`Cisco Packet Tracer` `VLSM` `DHCP` `DNS` `NAT` `VPN` `VLANs` `Static Routing`

---

## 🌐 Network Topology
- **Branch 1** — Tellers & ATMs subnets
- **Branch 2** — Tellers & ATMs subnets
- **HQ Router** — connects both branches
- **Central Router** — connects HQ to the server network
- **Server Network** — DNS Server & Web Server

---

## ✨ Features
- 📐 **VLSM Addressing** — efficient IP allocation for every subnet
- 🔀 **VLANs** — Tellers and ATMs separated for security & traffic control
- 🌍 **DHCP** — automatic IP assignment for all end devices
- 🔗 **DNS Server** — resolves `banking.bank` domain across the full network
- 🔒 **VPN Tunnels** — encrypted inter-branch communication
- 🔄 **NAT** — private-to-public IP translation for secure connectivity
- 🗺️ **Static Routing** — full connectivity between all routers
- 🌐 **Web Server** — accessible from any device on the network
- ✅ **Full ICMP Testing** — all devices ping successfully across all networks

---

## 📋 VLSM Addressing Table

| Subnet           | Network       | Subnet Mask       | First IP     | Last IP       | Broadcast     |
|------------------|---------------|-------------------|--------------|---------------|---------------|
| Branch1 Tellers  | 10.10.10.0    | 255.255.255.192   | 10.10.10.1   | 10.10.10.62   | 10.10.10.63   |
| Branch1 ATMs     | 10.10.20.0    | 255.255.255.240   | 10.10.20.1   | 10.10.20.14   | 10.10.20.15   |
| Branch2 Tellers  | 20.20.20.0    | 255.255.255.192   | 20.20.20.1   | 20.20.20.62   | 20.20.20.63   |
| Branch2 ATMs     | 20.20.30.0    | 255.255.255.240   | 20.20.30.1   | 20.20.30.14   | 20.20.30.15   |
| WAN B1 ↔ HQ     | 30.30.30.0    | 255.255.255.252   | 30.30.30.1   | 30.30.30.2    | 30.30.30.3    |
| WAN B2 ↔ HQ     | 40.40.40.0    | 255.255.255.252   | 40.40.40.1   | 40.40.40.2    | 40.40.40.3    |
| WAN HQ ↔ CB     | 50.50.50.0    | 255.255.255.0     | 50.50.50.1   | 50.50.50.254  | 50.50.50.255  |
| Server Network   | 60.60.60.0    | 255.255.255.0     | 60.60.60.1   | 60.60.60.254  | 60.60.60.255  |

---

## ✅ Testing & Verification
All devices were tested using ICMP ping across every network:
- ATMs0 → DNS Server ✅
- Tellers0 → Web Server (banking.bank) ✅
- ATMs1 → Central Router ✅
- Tellers1 → HQ Router ✅
- Simulation mode packet tracing verified end-to-end path ✅

---

## Pictures
<img width="975" height="1250" alt="image" src="https://github.com/user-attachments/assets/f776e682-c9b7-4929-8e57-04417f2d9257" />
<img width="975" height="481" alt="image" src="https://github.com/user-attachments/assets/1a1ae86a-852c-4371-9a5d-0afeac33f57c" />




