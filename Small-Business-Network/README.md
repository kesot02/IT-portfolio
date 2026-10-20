# Project 2: Small Business Network Design & Implementation

## Project Overview

This project involves designing, configuring, and testing a simulated small business network using Cisco Packet Tracer.

The network is designed for a fictional company with **50 employees across six departments**. The goal is to create a secure, scalable, and organized network infrastructure that supports departmental connectivity, business applications, and future growth.

This project demonstrates my developing skills in network design, IPv4 subnetting, VLAN segmentation, routing, switching, and network troubleshooting.

**Project Status:** In Progress — Network Topology Created, Device Configuration Pending

## Business Scenario

A growing small business requires a reliable network infrastructure to support its daily operations.

The company consists of six departments:

| Department | Employees | VLAN |
|---|---:|---:|
| Human Resources | 5 | 10 |
| Finance | 6 | 20 |
| Sales | 18 | 30 |
| Information Technology | 5 | 40 |
| Operations | 10 | 50 |
| Management | 6 | 60 |
| **Total** | **50** | |

The network must support:

- Reliable connectivity for all 50 employees
- Logical separation of departments using VLANs
- Efficient IPv4 address allocation through subnetting
- Controlled communication between departments
- Internet access and cloud-based business applications
- Centralized network administration
- Scalability for future business growth

### Business Communications

The company uses software based phones for voice and video communications through employee computers.

Because employees use software-based calling rather than dedicated physical IP phones, a separate voice VLAN is not included in the initial design.

Quality of Service (QoS) may be evaluated later to improve voice and video traffic performance.

## Tools and Technologies

- Cisco Packet Tracer
- Cisco Routers and Switches
- IPv4 Addressing
- Variable Length Subnet Masks (VLSM)
- Virtual Local Area Networks (VLANs)
- Inter-VLAN Routing
- Dynamic Host Configuration Protocol (DHCP)
- Access Control Lists (ACLs)
- Network Troubleshooting

## Network Design

### VLAN and IP Addressing Plan

Each department is assigned a dedicated VLAN and IPv4 subnet.

Subnet sizes are selected based on the number of employees, anticipated devices, and available room for expansion.

| Department | VLAN | Network Address | Subnet Mask | Usable IPs |
|---|---:|---|---|---:|
| HR | 10 | 192.168.10.0/28 | 255.255.255.240 | 14 |
| Finance | 20 | 192.168.20.0/28 | 255.255.255.240 | 14 |
| Sales | 30 | 192.168.30.0/27 | 255.255.255.224 | 30 |
| IT | 40 | 192.168.40.0/28 | 255.255.255.240 | 14 |
| Operations | 50 | 192.168.50.0/27 | 255.255.255.224 | 30 |
| Management | 60 | 192.168.60.0/28 | 255.255.255.240 | 14 |

### Subnetting Strategy

Instead of assigning a /24 subnet to every department, smaller subnets were selected to better match departmental requirements.

**/28 Networks**
- Provide 14 usable IPv4 addresses.
- Assigned to HR, Finance, IT, and Management.
- Suitable for smaller departments while allowing additional devices.

**/27 Networks**
- Provide 30 usable IPv4 addresses.
- Assigned to Sales and Operations.
- Provide additional capacity for larger departments and potential expansion.

This design demonstrates subnet sizing based on organizational needs rather than allocating the same subnet size to every department.

### Proposed Default Gateways

| Department | VLAN | Default Gateway |
|---|---:|---|
| HR | 10 | 192.168.10.1 |
| Finance | 20 | 192.168.20.1 |
| Sales | 30 | 192.168.30.1 |
| IT | 40 | 192.168.40.1 |
| Operations | 50 | 192.168.50.1 |
| Management | 60 | 192.168.60.1 |

These gateway addresses will be configured during the routing implementation phase.

## Network Topology

The initial network topology has been created in Cisco Packet Tracer.

The topology will be used to implement departmental VLANs, configure network devices, and test connectivity between network segments.

**Topology Screenshot:** To be added.

**Packet Tracer Project File:** To be added.

## Implementation Plan

### Phase 1: Network Planning and Topology

- [x] Define the fictional business requirements
- [x] Establish six departments and employee counts
- [x] Assign VLAN IDs to departments
- [x] Develop an IPv4 subnetting plan
- [x] Select proposed default gateway addresses
- [x] Create the initial network topology in Cisco Packet Tracer

### Phase 2: Basic Device Configuration

- [ ] Configure router and switch hostnames
- [ ] Configure basic device management settings
- [ ] Verify physical and logical device connections
- [ ] Document network device configurations

### Phase 3: VLAN Configuration

- [ ] Create VLAN 10 — Human Resources
- [ ] Create VLAN 20 — Finance
- [ ] Create VLAN 30 — Sales
- [ ] Create VLAN 40 — IT
- [ ] Create VLAN 50 — Operations
- [ ] Create VLAN 60 — Management
- [ ] Assign switch access ports to their respective VLANs
- [ ] Configure trunk links where required

### Phase 4: Routing and IP Addressing

- [ ] Configure inter-VLAN routing
- [ ] Configure default gateways
- [ ] Configure DHCP scopes for departmental networks
- [ ] Verify client IP address assignments
- [ ] Test authorized communication between VLANs

### Phase 5: Network Security

- [ ] Implement Access Control Lists (ACLs)
- [ ] Restrict unauthorized access to sensitive departmental networks
- [ ] Configure appropriate network device access controls
- [ ] Test and document security restrictions

### Phase 6: Testing and Troubleshooting

- [ ] Verify connectivity within each VLAN
- [ ] Test inter-VLAN routing
- [ ] Verify DHCP functionality
- [ ] Perform ping and traceroute tests
- [ ] Troubleshoot network configuration issues
- [ ] Document test results

## Planned Security Considerations

The network will use VLAN segmentation to logically separate departments.

Additional security controls will be evaluated to protect sensitive business resources.

Examples include:

- Restricting unnecessary access to HR and Finance networks
- Limiting administrative access to authorized IT personnel
- Using ACLs to control interdepartmental traffic
- Separating guest devices from internal business systems in a future expansion

## Future Improvements

Potential enhancements include:

- Dedicated server VLAN
- Guest wireless network
- Centralized monitoring and logging
- Network redundancy
- Quality of Service for RingCentral communications
- Additional security policies

## Skills Demonstrated and Being Developed

- Network requirements analysis
- Network topology design
- IPv4 subnetting and address planning
- VLAN design and segmentation
- Cisco
