# Project 2: Small Business Network Design

## Project Overview

This project focuses on designing, configuring, and testing a simulated small business network using Cisco Packet Tracer.

The objective is to develop hands-on networking skills involving network topology, IP addressing, VLANs, routing, DHCP, and basic network security.

## Business Scenario

A fictional company with 30 employees requires a reliable, scalable, and secure network to support three departments:

- Human Resources
- Finance
- Information Technology

The network will provide departmental segmentation, connectivity to shared services, and controlled access between network segments.

## Tools and Technologies

- Cisco Packet Tracer
- Cisco Routers and Switches
- VLANs and IEEE 802.1Q Trunking
- IPv4 Addressing and Subnetting
- Inter-VLAN Routing
- DHCP
- Access Control Lists (ACLs)

## Network Design

| Department | VLAN | Subnet | Default Gateway |
|---|---|---|---|
| HR | 10 | 192.168.10.0/24 | 192.168.10.1 |
| Finance | 20 | 192.168.20.0/24 | 192.168.20.1 |
| IT | 30 | 192.168.30.0/24 | 192.168.30.1 |
| Servers | 40 | 192.168.40.0/24 | 192.168.40.1 |

## Project Objectives

- [ X] Design a network topology
- [ ] Configure switches and router interfaces
- [ ] Create VLANs for each department
- [ ] Configure trunk ports
- [ ] Implement inter-VLAN routing
- [ ] Configure DHCP for client devices
- [ ] Test network connectivity
- [ ] Implement basic ACL security policies
- [ ] Document configuration and troubleshooting
- [ ] Upload topology screenshots and Packet Tracer project file

## Implementation Phases

### Phase 1: Network Topology

Create the network layout in Cisco Packet Tracer and connect the required devices.

### Phase 2: VLAN Configuration

Segment the network by department and assign switch ports to their respective VLANs.

### Phase 3: Routing and DHCP

Enable communication between authorized VLANs and configure automatic IP address assignment.

### Phase 4: Network Security

Implement ACLs to restrict unauthorized access between departments while permitting required services.

### Phase 5: Testing and Documentation

Verify connectivity using ping, traceroute, and Cisco IOS show commands. Document the results and troubleshoot any issues.

## Project Files

- Packet Tracer topology (.pkt) — To be added
- Network topology screenshots — To be added
- Device configurations — To be added
- Testing results — To be added

## Skills Being Developed

- Network Design
- VLAN Configuration
- IPv4 Subnetting
- Routing and Switching
- DHCP
- Network Security
- Troubleshooting
- Technical Documentation

## Project Status

**Planning — Network design and implementation pending.**

## Lessons Learned

This section will be updated as the project progresses.
