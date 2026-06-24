# Cisco Zone-Based Firewall (ZPF) with DMZ Implementation

## Project Overview

This project demonstrates the implementation of a secure enterprise network using Cisco Packet Tracer and Cisco Zone-Based Firewall (ZPF).

The network is segmented into multiple security zones to control traffic flow and improve security:

* Internal Users Zone
* Internal Servers Zone
* DMZ (Demilitarized Zone)
* Internet Zone

The objective was to configure firewall policies that allow legitimate traffic while preventing unauthorized access to internal resources.

---

## Network Architecture

```text
                Internet
                    |
               [Router/ISP]
                    |
              [ZPF Firewall]
                    |
    --------------------------------
    |              |              |
 Internal      Internal         DMZ
  Users         Servers       Servers
```

---

## Key Features

* Cisco Zone-Based Firewall (ZPF) configuration
* Network segmentation using security zones
* DMZ deployment for public-facing services
* Stateful packet inspection
* Traffic filtering and access control
* Firewall policy validation and testing

---

## Security Policies

### Allowed Traffic

| Source         | Destination          |
| -------------- | -------------------- |
| Internal Users | Internal Servers     |
| Internal Users | DMZ Servers          |
| Internal Users | Internet             |
| Internet       | DMZ Servers          |
| Return Traffic | Established Sessions |

### Blocked Traffic

| Source      | Destination      |
| ----------- | ---------------- |
| Internet    | Internal Users   |
| Internet    | Internal Servers |
| DMZ Servers | Internal Servers |

---

## Testing Results

### Successful Tests

* Internal User → DMZ Server communication
* Internal User → Internal Server communication
* Internal User → Internet communication
* Internet → DMZ Server communication

### Blocked Tests

* Internet → Internal User access
* Internet → Internal Server access
* DMZ → Internal Server access

These tests confirm that the firewall correctly enforces the configured security policies.

---

## Technologies Used

* Cisco Packet Tracer
* Cisco IOS
* Zone-Based Firewall (ZPF)
* Network Security Concepts
* Routing and Switching
* Access Control Policies

---

## Skills Demonstrated

* Network Design
* Firewall Configuration
* Security Policy Implementation
* DMZ Architecture
* Traffic Inspection
* Network Troubleshooting
* Cisco Networking

---

## Project Files

```text
.
├── README.md
├── project-report.pdf
└── zpf-firewall-project.pkt
```

---

## Learning Outcomes

Through this project, I gained practical experience in:

* Designing segmented networks
* Implementing Cisco Zone-Based Firewalls
* Configuring secure communication between zones
* Protecting internal resources from external threats
* Testing and validating network security policies

---

## Author

**Rijan Poudel**

Networking | Cybersecurity | Cisco Technologies
