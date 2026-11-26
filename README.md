
# Week 2 - IP Addressing (FLSM & VLSM) and VLAN Configuration

## Overview

This repository contains the practical work completed during Week 2 of my Networking Internship.

The focus of this week's activities was IP addressing, subnetting techniques, VLAN configuration, and network simulation using Cisco Packet Tracer and GNS3.

## Objectives

- Understand Fixed Length Subnet Masking (FLSM).
- Understand Variable Length Subnet Masking (VLSM).
- Practice efficient IPv4 address allocation.
- Learn VLAN configuration and network segmentation.
- Configure access and trunk ports.
- Design and simulate network topologies.
- Perform network connectivity testing and troubleshooting.

## Tasks Completed

### 1. IP Addressing and Subnetting

**FLSM (Fixed Length Subnet Masking)**
- Dividing networks into equal-sized subnets.
- Calculating subnet masks and network addresses.
- Identifying usable host ranges and broadcast addresses.

**VLSM (Variable Length Subnet Masking)**
- Allocating different subnet sizes based on host requirements.
- Applying efficient IP address utilization.
- Designing subnet allocations for different departments.

### 2. VLAN Configuration

Implemented a VLAN-based enterprise network with two departments:

| VLAN ID | Department | Network |
|---|---|---|
| VLAN 10 | HR | 192.168.10.0/24 |
| VLAN 20 | IT | 192.168.20.0/24 |

**Network Topology:**
- 2 Cisco 2960 switches
- 4 end devices (PCs)
- VLAN 10 for HR
- VLAN 20 for IT
- Trunk connection between switches
- Access port configuration for end devices

### 3. IP Address Assignment

| Device | VLAN | IP Address | Subnet Mask |
|---|---|---|---|
| PC1 | 10 | 192.168.10.10 | 255.255.255.0 |
| PC2 | 20 | 192.168.20.10 | 255.255.255.0 |
| PC3 | 10 | 192.168.10.11 | 255.255.255.0 |
| PC4 | 20 | 192.168.20.11 | 255.255.255.0 |

### 4. Switch Configuration

**Access Ports:**
- Fa0/1 - VLAN 10
- Fa0/2 - VLAN 20

**Trunk Port:**
- Fa0/24 - Switch-to-switch connection
- IEEE 802.1Q VLAN tagging

**Verification Commands:**

```bash
show vlan brief
show interfaces trunk
```

### 5. Network Simulation

**Cisco Packet Tracer**
- Designed a VLAN-based network topology.
- Configured VLANs on both switches.
- Assigned IP addresses to end devices.
- Configured access and trunk ports.
- Captured configuration and connectivity evidence.

**GNS3**
- Recreated the network topology.
- Used built-in Ethernet switches and VPCS devices.
- Assigned IP addresses and explored VLAN configuration.
- Practiced network connectivity troubleshooting.

## Tools and Technologies

- Cisco Packet Tracer
- GNS3
- IPv4 Addressing
- FLSM and VLSM
- Virtual LANs (VLANs)
- IEEE 802.1Q
- VPCS



## Key Learning Outcomes

- Improved understanding of IPv4 subnetting and address allocation.
- Practical exposure to FLSM and VLSM.
- Understanding of VLAN-based network segmentation.
- Experience configuring access and trunk ports.
- Hands-on experience with Cisco Packet Tracer and GNS3.
- Improved network troubleshooting skills.

## Conclusion

This week's activities provided practical exposure to IP addressing, subnetting, and VLAN-based network segmentation. Working with Cisco Packet Tracer and GNS3 helped strengthen my understanding of network design, switch configuration, and network simulation.

---


