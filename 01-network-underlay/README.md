# Network Underlay

![Status](https://img.shields.io/badge/Status-In_Progress-yellow)
![Routing](https://img.shields.io/badge/Routing-BGP_|_OSPF-blue)
![Connectivity](https://img.shields.io/badge/Connectivity-SD--WAN_|_WAN-blue)
![Wireless](https://img.shields.io/badge/Wireless-Enterprise-blue)
![Core Services](https://img.shields.io/badge/Core_Services-DNS_|_DHCP_|_NTP-green)
![Identity](https://img.shields.io/badge/Identity-RADIUS_|_Entra_ID-0078D4)
![Operations](https://img.shields.io/badge/Operations-SNMP_|_NetFlow-orange)
![Governance](https://img.shields.io/badge/Governance-Standards-purple)

### Enterprise Network Architecture • Routing • Connectivity • Core Infrastructure Services

---

## Overview

The Network Underlay provides the foundational connectivity layer supporting enterprise infrastructure, cloud integration, security services, identity platforms, endpoint communications, and operational services.

This section contains enterprise reference architectures, design standards, implementation guidance, operational frameworks, and infrastructure best practices used to build scalable, resilient, secure, and highly available network environments.

The objective is to establish a standardised networking framework that supports business growth, operational reliability, cloud adoption, security integration, and future technology modernisation.

---

## Quick Navigation

| Domain                              | Description                                                                          |
| ----------------------------------- | ------------------------------------------------------------------------------------ |
| [BGP Routing](./bgp)                | Enterprise routing architectures, ISP redundancy, Azure ExpressRoute, route policies |
| [VLAN Design](./vlan-design)        | Enterprise segmentation, security zoning, switching standards                        |
| [Wireless](./wireless)              | Enterprise wireless architecture, Entra ID authentication, NAC integration           |
| [IP Addressing](./ip-addressing)    | Enterprise IP planning, subnet allocation, route summarisation                       |
| [Network Standards](./standards)    | Governance, ITIL, operational standards, change management                           |
| [Architecture Diagrams](./diagrams) | Enterprise architecture patterns and reference designs                               |

---

## Enterprise Reference Architecture

![Enterprise Network Architecture](images/enterprise-network-reference-architecture.png)

---

## Architecture Scope

The Network Underlay focuses on the core services required to support enterprise technology environments.

### Network Infrastructure

* Routing Architecture
* Switching Infrastructure
* VLAN Segmentation
* Enterprise Wireless
* WAN Connectivity
* SD-WAN Integration
* High Availability Design
* Network Segmentation

### Core Infrastructure Services

* DNS
* DHCP
* NTP
* RADIUS
* SNMP
* Syslog
* NetFlow
* Telemetry

### Identity & Access Integration

* Microsoft Entra ID
* Conditional Access
* Multi-Factor Authentication (MFA)
* Network Access Control (NAC)
* Device Compliance
* Role-Based Access Control (RBAC)

### Operations & Governance

* Monitoring & Observability
* ITIL Service Management
* Change Management
* Configuration Standards
* Documentation Standards
* Business Continuity

---

## Technology Domains

### BGP & Enterprise Routing

Enterprise routing architectures supporting WAN connectivity, cloud integration, route optimisation, and ISP redundancy.

#### Technologies

* BGP
* OSPF
* Route Summarisation
* Policy-Based Routing
* Azure ExpressRoute
* SD-WAN

#### Deliverables

* Routing Standards
* BGP Design Templates
* Route Filtering Policies
* ISP Integration Models
* Routing Validation Procedures

---

### VLAN Architecture & Segmentation

Logical network segmentation supporting security, performance, and operational consistency.

#### Technologies

* VLANs
* Layer 2 Switching
* Inter-VLAN Routing
* ACLs
* Security Zones

#### Deliverables

* VLAN Standards
* Naming Conventions
* Segmentation Models
* Security Zoning Frameworks
* Enterprise Switching Standards

---

### Enterprise Wireless

Modern wireless architectures supporting secure mobility, identity-driven access control, and enterprise-scale deployments.

#### Technologies

* Wi-Fi 6
* Wi-Fi 6E
* Wi-Fi 7
* WPA3 Enterprise
* 802.1X
* RADIUS
* NAC
* Microsoft Entra ID

#### Deliverables

* Wireless Reference Architectures
* Authentication Frameworks
* SSID Standards
* RF Planning Guidance
* Capacity Planning Models

---

### IP Address Management (IPAM)

Structured IP allocation and addressing frameworks supporting scalable enterprise deployments.

#### Technologies

* IPv4
* DHCP
* DNS
* Route Summarisation
* IP Planning

#### Deliverables

* Addressing Frameworks
* Subnet Standards
* Branch Site Models
* Cloud Addressing Standards
* IP Governance Procedures

---

### Core Infrastructure Services

Foundational services supporting enterprise operations and network functionality.

#### Services

* DNS
* DHCP
* NTP
* RADIUS
* SNMP
* Syslog
* NetFlow
* Telemetry

#### Deliverables

* Service Standards
* Availability Models
* Monitoring Standards
* Operational Procedures
* Validation Frameworks

---

### Network Topology & Architecture

Enterprise reference architectures and infrastructure design patterns.

#### Deliverables

* Campus Network Designs
* Branch Office Architectures
* WAN Topologies
* Hybrid Cloud Architectures
* Azure Connectivity Models
* SD-WAN Reference Designs

---

### Standards & Governance

Enterprise standards supporting operational consistency, security, compliance, and lifecycle management.

#### Areas Covered

* Infrastructure Standards
* Security Baselines
* Cloud Governance
* ITIL Service Management
* Change Management
* Monitoring & Observability
* Business Continuity
* Automation Standards

---

## Design Principles

### Scalability

Support future growth without requiring major architectural redesign.

### Resilience

Minimise service disruption through redundancy, failover mechanisms, and high-availability design.

### Security

Apply Zero Trust principles, segmentation, authentication controls, and least-privilege access.

### Standardisation

Maintain consistent deployment standards and operational practices.

### Observability

Provide complete visibility through monitoring, telemetry, logging, and reporting.

### Automation

Reduce operational complexity through Infrastructure as Code and automation frameworks.

### Cloud Integration

Enable seamless integration with cloud services and hybrid environments.

---

## Current Roadmap

* [ ] Enterprise Network Reference Architecture
* [ ] BGP & OSPF Design Framework
* [ ] VLAN Segmentation Standards
* [ ] Wireless Architecture Guide
* [ ] DNS & DHCP Standards
* [ ] Core Services Framework
* [ ] SD-WAN Architecture
* [ ] Network Operations Runbooks
* [ ] Validation & Testing Procedures
* [ ] Monitoring & Observability Framework

---

## Repository Structure

```text
01-network-underlay
│
├── bgp
├── vlan-design
├── wireless
├── ip-addressing
├── standards
├── diagrams
│
└── README.md
```

---

## Key Outcomes

✔ Enterprise Routing Architecture

✔ WAN & SD-WAN Connectivity

✔ Network Segmentation

✔ Enterprise Wireless Design

✔ Core Infrastructure Services

✔ Identity Integration

✔ Monitoring & Observability

✔ Operational Governance

✔ ITIL Service Management Alignment

✔ Infrastructure Standardisation

---

## Status

🚧 Active Development

This section is continuously expanded with enterprise architecture patterns, implementation guidance, operational frameworks, governance standards, cloud connectivity models, and modern networking reference designs.
