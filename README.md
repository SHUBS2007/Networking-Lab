# Cybercrime Network Simulation using Cisco Packet Tracer

## Project Overview

This project demonstrates the design and implementation of a small secure Local Area Network (LAN) using Cisco Packet Tracer. The network simulates the infrastructure of a cybercrime investigation office where investigator workstations communicate with a centralized evidence server through a router and switch.

The primary objective of this project was to understand network topology design, IP addressing, router configuration, switching concepts, and network connectivity testing using Cisco devices.

---

## Project Scenario

A small cybercrime investigation office requires a secure internal network where investigators can communicate with a central evidence server.

The network should:

- Connect multiple investigator systems
- Provide communication through a router and switch
- Use static IP addressing
- Allow connectivity verification between all devices
- Simulate a basic organizational network

---

## Project Objectives

- Design a basic enterprise LAN
- Configure Cisco router using CLI
- Configure static IP addressing
- Understand routing and switching fundamentals
- Verify network communication using Ping
- Practice Cisco IOS commands
- Document the complete network setup

---

## Software Used

- Cisco Packet Tracer 8.x
- Cisco IOS CLI

---

## Network Topology

```
                 Router (1841)

                      |

                 Switch (2960)

       |       |       |       |        |

 Investigator-PC1

 Investigator-PC2

 Investigator-PC3

 Investigator-PC4

 Evidence-Server
```

---

## Devices Used

| Device | Quantity |
|----------|---------:|
| Cisco 1841 Router | 1 |
| Cisco 2960 Switch | 1 |
| PC | 4 |
| Server | 1 |

---

## IP Addressing Scheme

| Device | IP Address |
|----------|----------------|
| Router | 192.168.10.1 |
| Investigator-PC1 | 192.168.10.10 |
| Investigator-PC2 | 192.168.10.11 |
| Investigator-PC3 | 192.168.10.12 |
| Investigator-PC4 | 192.168.10.13 |
| Evidence Server | 192.168.10.100 |

Subnet Mask

```
255.255.255.0
```

Default Gateway

```
192.168.10.1
```

---

## Router Configuration

The router interface was configured using Cisco IOS CLI.

Commands used:

```bash
enable

configure terminal

interface FastEthernet0/0

ip address 192.168.10.1 255.255.255.0

no shutdown

exit

copy running-config startup-config
```

The **no shutdown** command was used to activate the router interface.

---

## Project Workflow

### Phase 1 – Network Design

- Created network topology
- Added router
- Added switch
- Added investigator PCs
- Added evidence server

---

### Phase 2 – Device Configuration

Configured:

- Static IP Address
- Subnet Mask
- Default Gateway

Router interface configured using Cisco CLI.

---

### Phase 3 – Connectivity Testing

Performed network verification using:

```bash
ping
```

Verified communication between:

- PC to Router
- PC to PC
- PC to Evidence Server

Successfully established network connectivity.

---

## Cisco Commands Used

| Command | Purpose |
|----------|---------|
| enable | Enter privileged mode |
| configure terminal | Enter configuration mode |
| interface FastEthernet0/0 | Select interface |
| ip address | Assign IP address |
| no shutdown | Enable interface |
| show ip interface brief | View interface status |
| ping | Test connectivity |

---

## Skills Learned

- Cisco Router Configuration
- Cisco Switch Connectivity
- Static IP Addressing
- Network Topology Design
- Cisco IOS CLI
- Routing Fundamentals
- Switching Fundamentals
- LAN Communication
- Network Troubleshooting
- Connectivity Testing

---

## Project Structure

```
Cybercrime-Network-Simulation/

│

├── README.md

├── Report.docx

├── Report.pdf

├── topology.pkt

├── screenshots/

│     ├── topology.png

│     ├── router-configuration.png

│     ├── successful-ping.png

│

└── LICENSE
```

---

## Screenshots

### Network Topology

*(Insert topology screenshot here)*

---

### Router Configuration

*(Insert CLI screenshot here)*

---

### Successful Ping Test

*(Insert successful ping screenshot here)*

---

## Challenges Faced

During the initial configuration, the router interface remained in a down state because Cisco router interfaces are administratively disabled by default.

This issue was resolved using:

```bash
no shutdown
```

Another challenge involved unsuccessful ping requests before assigning static IP addresses and default gateways to all end devices. After proper configuration, all devices communicated successfully.

---

## Future Improvements

This project can be extended by implementing:

- VLAN Segmentation
- Access Control Lists (ACL)
- DHCP Server
- DNS Server
- SSH Remote Management
- Firewall Configuration
- Inter-VLAN Routing
- Dynamic Routing Protocols (RIP, OSPF)

---

## Learning Outcome

Through this project, I gained practical experience in:

- Designing a LAN
- Configuring Cisco routers and switches
- Assigning IP addresses
- Understanding packet forwarding
- Testing network communication
- Troubleshooting basic networking issues

This project strengthened my understanding of networking fundamentals, which are essential for cybersecurity and cloud security.

---

## Author

**Shubham Bhatti**

B.Tech Cybersecurity Student
Marwadi University

LinkedIn:
https://linkedin.com/in/shubham-bhatti2007

---

> **Disclaimer:** This project was created for educational purposes to demonstrate networking fundamentals using Cisco Packet Tracer.
