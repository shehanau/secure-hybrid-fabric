# Enterprise BGP Design

## Overview

Border Gateway Protocol (BGP) provides scalable routing between autonomous systems and enables resilient WAN and cloud connectivity.

## Business Objective

Provide highly available connectivity between:

- Head Office
- Branch Offices
- Data Centres
- Cloud Providers

## Design Principles

- Redundancy
- Fast Convergence
- Route Summarisation
- Policy Based Routing
- Scalability

## Architecture

(insert diagram)

## Example Use Cases

### ISP Redundancy

Primary ISP
Secondary ISP

### SD-WAN Integration

Dynamic route advertisement.

### Cloud Connectivity

Azure ExpressRoute

## Validation

- Route failover testing
- Path selection verification
- Route filtering validation

## Lessons Learned

- Keep route advertisements simple.
- Use summarisation whenever possible.
- Avoid unnecessary route redistribution.
