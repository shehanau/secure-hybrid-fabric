# VLAN Design

![Status](https://img.shields.io/badge/Status-In_Progress-yellow)
![VLAN](https://img.shields.io/badge/VLAN-Segmentation-blue)
![Cisco](https://img.shields.io/badge/Cisco-Switching-blue)
![Security](https://img.shields.io/badge/Security-Zoning-red)
![Enterprise](https://img.shields.io/badge/Enterprise-Networking-green)

## Overview

VLANs (Virtual Local Area Networks) provide logical segmentation within enterprise networks, improving security, performance, scalability, and operational management.

This section contains reference architectures, segmentation strategies, naming conventions, IP allocation models, and operational standards used within enterprise environments.

---

## Business Objectives

The VLAN architecture is designed to:

* Separate business-critical services
* Reduce broadcast domains
* Improve network performance
* Support security segmentation
* Simplify troubleshooting
* Enable scalable growth
* Support Zero Trust initiatives

---

## Enterprise Reference Model

| VLAN | Name                    | Purpose                      |
| ---- | ----------------------- | ---------------------------- |
| 10   | Corporate               | User Workstations            |
| 20   | Voice                   | IP Telephony                 |
| 30   | Guest WiFi              | Internet Access Only         |
| 40   | Servers                 | Internal Applications        |
| 50   | Management              | Network Devices              |
| 60   | CCTV / IoT              | Cameras and Building Systems |
| 70   | Wireless Infrastructure | Access Points                |
| 80   | Printers                | Shared Printing Services     |
| 90   | DMZ                     | Public Facing Services       |
| 99   | Native / Infrastructure | Switch Infrastructure        |

---

## Example IP Allocation

| VLAN       | Subnet        |
| ---------- | ------------- |
| Corporate  | 10.10.10.0/24 |
| Voice      | 10.10.20.0/24 |
| Guest      | 10.10.30.0/24 |
| Servers    | 10.10.40.0/24 |
| Management | 10.10.50.0/24 |
| CCTV       | 10.10.60.0/24 |
| Wireless   | 10.10.70.0/24 |
| Printers   | 10.10.80.0/24 |
| DMZ        | 10.10.90.0/24 |

---

## Design Principles

### Security

Sensitive systems should be isolated from user networks using dedicated VLANs and firewall policies.

### Scalability

VLAN numbering and subnet allocation should support future growth without requiring major redesign.

### Consistency

Naming conventions and VLAN assignments should remain consistent across all sites.

### Simplicity

Avoid unnecessary VLAN sprawl and maintain clear documentation.

### Resilience

Critical infrastructure should support redundancy and high availability.

---

## Sample Branch Office Architecture

```text
Internet
    │
FortiGate Firewall
    │
Core Switch
    │
├── VLAN 10 Corporate
├── VLAN 20 Voice
├── VLAN 30 Guest
├── VLAN 40 Servers
├── VLAN 50 Management
├── VLAN 60 CCTV
└── VLAN 70 Wireless
```

---

## Security Considerations

### Corporate VLAN

* Domain joined devices
* Access to internal resources
* Controlled internet access

### Voice VLAN

* Dedicated QoS policies
* IP telephony services
* Separate broadcast domain

### Guest VLAN

* Internet only
* No internal network access
* Captive portal optional

### Management VLAN

* Restricted administrator access
* Network device management
* Infrastructure monitoring

### CCTV / IoT VLAN

* Isolated security systems
* Limited outbound access
* Firewall-controlled communications

---

## Operational Standards

### VLAN Naming Convention

```text
VLAN10-CORPORATE
VLAN20-VOICE
VLAN30-GUEST
VLAN40-SERVERS
VLAN50-MANAGEMENT
VLAN60-CCTV
```

### Documentation Requirements

Each VLAN should document:

* VLAN ID
* Name
* Purpose
* Subnet
* Gateway
* DHCP Scope
* Firewall Policies
* Associated Services

---

## Validation Checklist

* [ ] VLANs created
* [ ] Trunks configured
* [ ] DHCP scopes assigned
* [ ] Inter-VLAN routing tested
* [ ] Firewall policies validated
* [ ] QoS policies applied
* [ ] Monitoring enabled
* [ ] Documentation completed

---

## Future Enhancements

* Micro-segmentation
* Software Defined Access (SDA)
* Dynamic VLAN assignment
* NAC integration
* Zero Trust network controls

---

## Status

🚧 Active Development

This section is being expanded with enterprise design examples, implementation guides, diagrams, and operational standards.
