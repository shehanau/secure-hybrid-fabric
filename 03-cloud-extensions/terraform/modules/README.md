# Terraform Modules

![Status](https://img.shields.io/badge/Status-In_Progress-yellow)
![Terraform](https://img.shields.io/badge/Terraform-Reusable_Modules-844FBA)
![Azure](https://img.shields.io/badge/Azure-Cloud_Platform-0078D4)
![Automation](https://img.shields.io/badge/Automation-IaC-green)

### Reusable Infrastructure Components • Standardisation • Automation

---

## Overview

Terraform modules provide reusable building blocks that simplify infrastructure deployments and promote consistency across environments.

Modules enable organisations to standardise deployments, reduce configuration drift, improve governance, and accelerate cloud adoption.

This section contains reusable Azure infrastructure modules designed to support enterprise-scale deployments.

---

## Module Structure

```text
modules
│
├── network
├── virtual-machine
├── storage-account
├── log-analytics
├── key-vault
├── nsg
├── route-table
└── resource-group
```

---

## Available Modules

### Network Module

Deploys:

* Virtual Networks
* Subnets
* Address Spaces
* DNS Configuration

### Network Security Group Module

Deploys:

* NSGs
* Security Rules
* Traffic Controls

### Route Table Module

Deploys:

* Route Tables
* Custom Routes
* Traffic Management Policies

### Virtual Machine Module

Deploys:

* Windows Virtual Machines
* Linux Virtual Machines
* Network Interfaces
* Managed Disks

### Storage Account Module

Deploys:

* Storage Accounts
* Blob Containers
* File Shares

### Log Analytics Module

Deploys:

* Log Analytics Workspaces
* Monitoring Configuration
* Diagnostic Settings

### Key Vault Module

Deploys:

* Azure Key Vault
* Secrets Management
* Certificate Storage

### Resource Group Module

Deploys:

* Resource Groups
* Tags
* Governance Standards

---

## Design Principles

### Reusability

Create once and deploy multiple times.

### Standardisation

Ensure consistent deployments across environments.

### Security

Apply security controls by default.

### Scalability

Support enterprise growth and cloud expansion.

### Governance

Enforce organisational policies and standards.

---

## Example Usage

```terraform
module "network" {
  source              = "../modules/network"

  resource_group_name = "rg-production"
  vnet_name           = "vnet-production"
  address_space       = ["10.10.0.0/16"]
}
```

---

## Benefits

* Reduced Deployment Time
* Consistent Infrastructure
* Improved Governance
* Simplified Maintenance
* Easier Troubleshooting
* Infrastructure Standardisation

---

## Future Enhancements

* Azure Firewall Module
* VPN Gateway Module
* ExpressRoute Module
* Azure Backup Module
* Azure Monitor Module
* Azure Landing Zone Module

---

## Status

🚧 Active Development

This section is being expanded with reusable Azure infrastructure modules, governance controls, monitoring integrations, and enterprise deployment standards.
