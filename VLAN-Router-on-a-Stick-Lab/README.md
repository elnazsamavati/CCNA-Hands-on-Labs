# CCNA VLAN & Router-on-a-Stick Lab

This project demonstrates a small enterprise Layer 2 and Layer 3 network implemented in Cisco Packet Tracer.


## Technologies Used
- VLAN
- Router-on-a-Stick
- IEEE 802.1Q Trunking
- EtherChannel (LACP)
- Rapid Spanning Tree Protocol
- SSH Remote Management
- DHCP
- PortFast
- BPDU Guard

---

## VLAN Design
| VLAN | Name | Network |
|------|------|---------------|
| 10 | IT | 192.168.10.0/24 |
| 20 | HR | 192.168.20.0/24 |
| 30 | Management | 192.168.30.0/24 |

---

## Network Design
- R1 performs inter-VLAN routing using Router-on-a-Stick.
- SW-01 acts as the distribution switch.
- SW-02 and SW-03 are access switches.
- EtherChannel is configured using LACP.
- SW-01 is configured as the Root Bridge for all VLANs.
- Management IP addresses are assigned through VLAN 30.
- DHCP services are provided by R1.
- SSH is enabled on all devices.
- PortFast and BPDU Guard are enabled on access ports.

---

## Device Management IPs
| Device | Management IP |
|---------|---------------|
| SW-01 | 192.168.30.1 |
| SW-02 | 192.168.30.2 |
| SW-03 | 192.168.30.3 |
| R1 | 192.168.30.254 |

---

## Files
- `VLAN-Router-on-a-Stick-Lab.pkt` → Packet Tracer project
- `configs/` → Device configurations

---

## Skills Demonstrated
- VLAN segmentation
- Inter-VLAN Routing
- Layer 2 Redundancy
- EtherChannel
- SSH Configuration
- DHCP Configuration
- Cisco IOS CLI