# CCNA Enterprise Network Topology Simulator

## Overview

This project demonstrates:

- VLANs (10, 20, 30)
- Inter-VLAN Routing (Router-on-a-Stick)
- OSPF Area 0
- EIGRP AS 100
- OSPF ↔ EIGRP Route Redistribution
- PVST+ Root Bridge
- End-to-End Connectivity Testing

## Topology

PC1 (VLAN10)
PC2 (VLAN20)
PC3 (VLAN30)
        |
       SW1
        |
       R1
        |
      OSPF
        |
       R2
        |
      EIGRP
        |
       R3

## Verification

### OSPF Neighbor

show ip ospf neighbor

State: FULL

### EIGRP Neighbor

show ip eigrp neighbors

Neighbor: 10.1.23.1

### Route Redistribution

R1 learned:

O E2 3.3.3.3/32

### Connectivity

R1 successfully pinged 3.3.3.3