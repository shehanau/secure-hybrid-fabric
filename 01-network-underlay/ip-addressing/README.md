# Enterprise IP Addressing Framework

![Status](https://img.shields.io/badge/Status-In_Progress-yellow)
![IPAM](https://img.shields.io/badge/IP-Addressing-blue)
![Enterprise](https://img.shields.io/badge/Enterprise-Networking-blue)
![Scalability](https://img.shields.io/badge/Scalable-Design-green)

## Overview

A structured IP addressing framework is critical for scalability, operational simplicity, troubleshooting efficiency, and future network growth.

This section documents enterprise IP allocation standards, subnet planning methodologies, summarisation strategies, and addressing conventions used across multi-site environments.

---

## Business Objectives

- Standardised IP allocation
- Simplified troubleshooting
- Route summarisation
- Future growth planning
- Consistent site deployments
- Reduced operational complexity

---

## Design Principles

### Hierarchical Allocation

Address ranges are allocated logically by site, function, and service type.

### Summarisation

Networks should be summarised wherever possible to reduce routing table size.

### Scalability

Address allocations should support future growth without renumbering.

### Consistency

All sites follow a standard allocation model.

### Documentation

All subnets must be documented and tracked.

---

## Enterprise Addressing Model

| Site | Address Space |
|--------|--------|
| Melbourne Head Office | 10.10.0.0/16 |
| Sydney Branch | 10.20.0.0/16 |
| Brisbane Branch | 10.30.0.0/16 |
| Perth Branch | 10.40.0.0/16 |
| Data Centre | 10.50.0.0/16 |
| Azure Cloud | 10.100.0.0/16 |

---

## Melbourne Head Office Example

| VLAN | Purpose | Subnet |
|--------|--------|--------|
| 10 | Corporate | 10.10.10.0/24 |
| 20 | Voice | 10.10.20.0/24 |
| 30 | Guest WiFi | 10.10.30.0/24 |
| 40 | Servers | 10.10.40.0/24 |
| 50 | Management | 10.10.50.0/24 |
| 60 | CCTV / IoT | 10.10.60.0/24 |

---

## Azure Addressing Example

| Subnet | Purpose |
|----------|----------|
| 10.100.1.0/24 | Web Tier |
| 10.100.2.0/24 | Application Tier |
| 10.100.3.0/24 | Database Tier |
| 10.100.255.0/27 | Gateway Subnet |

---

## Route Summarisation Strategy

### Branch Offices

```text
Sydney      10.20.0.0/16
Brisbane    10.30.0.0/16
Perth       10.40.0.0/16
```

Advertised as:

```text
10.0.0.0/8
```

where appropriate.

### Benefits

- Smaller routing tables
- Faster convergence
- Easier troubleshooting
- Simplified WAN design

---

## Address Allocation Standards

### User Networks

```text
x.x.10.0/24
```

### Voice Networks

```text
x.x.20.0/24
```

### Guest Networks

```text
x.x.30.0/24
```

### Server Networks

```text
x.x.40.0/24
```

### Management Networks

```text
x.x.50.0/24
```

### CCTV / IoT

```text
x.x.60.0/24
```

---

## IPAM Considerations

Recommended documentation:

- Subnet allocations
- DHCP scopes
- VLAN mappings
- DNS zones
- Gateway assignments
- Reserved ranges

---

## Validation Checklist

- [ ] Address plan documented
- [ ] Subnets allocated
- [ ] DHCP scopes configured
- [ ] DNS records validated
- [ ] Route summarisation reviewed
- [ ] Documentation updated

---

## Future Enhancements

- IPAM Platform Integration
- Azure IP Planning
- IPv6 Strategy
- Multi-Region Addressing
- Cloud-Native Network Design

---

## Status

🚧 Active Development

This section is being expanded with enterprise addressing models, cloud network planning, IPAM standards, and operational guidance.
