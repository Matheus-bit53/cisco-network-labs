# 🌐 Lab: Corporate VLAN Configuration

Practical project focused on network segmentation, logical security, and performance using Cisco switches and routers.

### 🗺️ Network Scenario
The network was divided into 3 departments using a single Managed Switch, isolating broadcast traffic and increasing security:

| Department / VLAN | VLAN ID | IP Network |
| :--- | :--- | :--- |
| **Admin (Management)** | VLAN 10 | `192.168.10.0/24` |
| **Sales (Commercial)** | VLAN 20 | `192.168.20.0/24` |
| **IT (Support)** | VLAN 30 | `192.168.30.0/24` |

---

### 🛠️ Main Commands

**1. Creating the VLANs:**
```cisconet
Switch(config)# vlan 10
Switch(config-vlan)# name Admin
Switch(config-vlan)# vlan 20
Switch(config-vlan)# name Sales
Switch(config-vlan)# vlan 30
Switch(config-vlan)# name IT

