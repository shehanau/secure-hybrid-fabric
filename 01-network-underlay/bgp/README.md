# Enterprise BGP Design

![Status](https://img.shields.io/badge/Status-In_Progress-yellow)
![BGP](https://img.shields.io/badge/BGP-Routing-blue)
![Cisco](https://img.shields.io/badge/Cisco-Networking-blue)
![SD-WAN](https://img.shields.io/badge/SD--WAN-Connectivity-green)
![Azure](https://img.shields.io/badge/Azure-ExpressRoute-0078D4)

## Overview

Border Gateway Protocol (BGP) is the industry-standard routing protocol used to exchange routing information between autonomous systems and large-scale enterprise networks.

BGP enables resilient WAN connectivity, cloud integration, ISP redundancy, traffic engineering, and scalable multi-site network design.

This section provides enterprise design patterns, operational guidance, routing policies, and reference architectures commonly used in modern infrastructure environments.

---

## Business Objectives

Provide highly available and scalable connectivity between:

- Head Office
- Branch Offices
- Data Centres
- Cloud Providers
- Internet Service Providers
- SD-WAN Platforms

Key outcomes include:

- Increased resilience
- Reduced downtime
- Optimised traffic flow
- Improved cloud connectivity
- Simplified route management

---

## Architecture

![Enterprise BGP Architecture](diagrams/bgp-dual-isp.png)

### Example Architecture Components

| Component | Purpose |
|------------|------------|
| ISP 1 | Primary Internet Connectivity |
| ISP 2 | Secondary Internet Connectivity |
| Edge Routers | BGP Peering |
| Firewall Cluster | Security Enforcement |
| Core Network | Internal Routing |
| Azure ExpressRoute | Cloud Connectivity |
| SD-WAN Fabric | Branch Connectivity |

---

## Design Principles

### Redundancy

Multiple internet providers eliminate single points of failure.

### Fast Convergence

Traffic automatically reroutes during service interruptions.

### Route Summarisation

Reduce routing complexity and improve scalability.

### Policy Based Routing

Control preferred traffic paths.

### Scalability

Support future growth without redesigning the network.

---

## Common Enterprise Use Cases

### ISP Redundancy

Maintain internet connectivity during provider outages.

Benefits:

- Increased uptime
- Improved resilience
- Automatic failover

---

### SD-WAN Integration

Exchange dynamic routing information between branch locations.

Benefits:

- Dynamic path selection
- Centralised management
- Improved WAN performance

---

### Azure ExpressRoute

Establish private connectivity to Microsoft Azure services.

Benefits:

- Reduced latency
- Improved reliability
- Enhanced security

---

### Multi-Site Enterprise WAN

Provide routing exchange between regional offices and data centres.

Benefits:

- Centralised routing control
- Route optimisation
- Simplified management

---

## Routing Policies

### Local Preference

Used to determine the preferred outbound path.

### AS Path Prepending

Influences inbound traffic routing.

### Route Filtering

Prevents route leaks and unauthorised advertisements.

### Prefix Lists

Controls advertised and accepted prefixes.

---

## Operational Considerations

### Monitoring

Recommended monitoring methods:

- SNMP
- Syslog
- NetFlow
- Telemetry
- BGP Session Monitoring

### Documentation

Maintain records of:

- ASN assignments
- BGP neighbours
- Advertised prefixes
- Routing policies
- Failover procedures

---

## Validation Checklist

- [ ] BGP neighbour relationships established
- [ ] Route advertisements verified
- [ ] Prefix filtering validated
- [ ] Failover testing completed
- [ ] Traffic paths confirmed
- [ ] Monitoring enabled
- [ ] Documentation updated

---

## Lessons Learned

- Keep route advertisements simple.
- Use route summarisation where possible.
- Minimise route redistribution.
- Apply route filtering consistently.
- Regularly test failover scenarios.
- Maintain accurate documentation.

---

## Future Enhancements

- Azure ExpressRoute Design
- SD-WAN Routing Integration
- Route Reflector Architectures
- BGP Security Controls
- Enterprise Routing Runbooks

---

## Status

🚧 Active Development

This section is being expanded with enterprise routing architectures, implementation examples, operational procedures, and troubleshooting guidance.
