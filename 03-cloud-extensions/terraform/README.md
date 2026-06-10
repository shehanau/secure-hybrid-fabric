# Terraform

![Status](https://img.shields.io/badge/Status-In_Progress-yellow)
![Terraform](https://img.shields.io/badge/Terraform-Infrastructure_as_Code-844FBA)
![Azure](https://img.shields.io/badge/Azure-Cloud_Platform-0078D4)
![Automation](https://img.shields.io/badge/Automation-IaC-green)
![DevOps](https://img.shields.io/badge/DevOps-Platform-orange)
![GitHub](https://img.shields.io/badge/GitHub-Version_Control-black)

### Infrastructure as Code • Automation • Cloud Provisioning • Governance

---

## Overview

Terraform is an Infrastructure as Code (IaC) platform used to automate the deployment, configuration, and lifecycle management of cloud and infrastructure resources.

This section contains reference architectures, deployment examples, reusable modules, governance standards, and operational practices used to provision enterprise infrastructure consistently and securely.

The objective is to reduce manual deployment effort, improve standardisation, increase reliability, and support scalable cloud adoption.

---
## Quick Navigation

| Module                                     | Description                                                                               |
| ------------------------------------------ | ----------------------------------------------------------------------------------------- |
| [Azure Virtual Network](./azure-vnet)      | Terraform deployment of Azure VNets, subnets, NSGs, route tables, and hybrid connectivity |
| [Azure Virtual Machine](./azure-vm)        | Terraform deployment of Windows and Linux virtual machines                                |
| [Azure Landing Zone](./azure-landing-zone) | Enterprise governance, subscriptions, policies, and Azure foundations                     |
| [Reusable Modules](./modules)              | Standardised Terraform modules for enterprise deployments                                 |

---

## Reference Architectures

| Architecture                      | Description                                        |
| --------------------------------- | -------------------------------------------------- |
| Terraform Reference Architecture  | End-to-end Infrastructure as Code deployment model |
| Azure VNet Reference Architecture | Enterprise Azure networking deployment             |
| Azure VM Reference Architecture   | Azure compute deployment pattern                   |
| Azure Landing Zone Architecture   | Governance and cloud foundation design             |

---

## Technology Coverage

### Infrastructure as Code

* Terraform
* HCL
* State Management
* Remote Backend

### Azure Services

* Resource Groups
* Virtual Networks
* Virtual Machines
* Storage Accounts
* Azure Monitor
* Key Vault

### Governance

* Azure Policy
* Resource Tagging
* RBAC
* Management Groups

### Automation

* GitHub Actions
* Azure DevOps
* PowerShell
* CI/CD Pipelines


## Reference Architecture

![Terraform Architecture](images/terraform-reference-architecture.png)

---

## Core Capabilities

### Infrastructure as Code

Provision infrastructure through version-controlled code.

### Automation

Automate repeatable deployments and operational tasks.

### Standardisation

Ensure environments are deployed consistently.

### Governance

Apply security, compliance, and organisational standards.

### Scalability

Support rapid growth through reusable deployment models.

---

## Technology Stack

### Terraform

Core Infrastructure as Code platform.

### GitHub

Source control and collaboration.

### Azure

Cloud platform hosting deployed infrastructure.

### PowerShell

Automation and operational scripting.

### Azure DevOps / GitHub Actions

CI/CD integration and deployment automation.

---

## Deployment Workflow

```text
Developer
    │
    ▼
Git Repository
    │
    ▼
Terraform Plan
    │
    ▼
Terraform Apply
    │
    ▼
Azure Resources
```

---

## Example Deployments

### Azure Networking

* Virtual Networks
* Subnets
* Route Tables
* NSGs
* DNS

### Azure Compute

* Virtual Machines
* Availability Sets
* Managed Disks

### Identity

* Resource RBAC
* Managed Identities

### Monitoring

* Log Analytics
* Azure Monitor
* Alerts

---

## Repository Structure

```text
terraform
│
├── azure-vnet
├── azure-vm
├── azure-landing-zone
├── modules
│
├── images
└── README.md
```

---

## Reusable Modules

### Network Module

Deploy:

* VNets
* Subnets
* NSGs
* Route Tables

### Compute Module

Deploy:

* Azure VMs
* Availability Sets
* Managed Disks

### Monitoring Module

Deploy:

* Log Analytics
* Azure Monitor
* Alerts

---

## Azure Landing Zone

Terraform can be used to deploy:

* Management Groups
* Subscriptions
* Policies
* Resource Groups
* Networking
* Security Controls

### Benefits

* Governance
* Standardisation
* Security
* Automation

---

## Security Considerations

### State Management

* Secure Storage Accounts
* Remote State
* RBAC Controls

### Secrets Management

* Azure Key Vault
* Managed Identities
* Secure Variables

### Access Control

* Least Privilege
* Role-Based Access Control
* Change Approval Processes

---

## Design Principles

### Automation First

Automate wherever possible.

### Reusability

Create modular deployments.

### Security

Protect state files and secrets.

### Governance

Enforce organisational standards.

### Consistency

Reduce configuration drift.

---

## Validation Checklist

* [ ] Code reviewed
* [ ] Terraform validated
* [ ] Plan reviewed
* [ ] Security controls applied
* [ ] State storage configured
* [ ] Documentation completed
* [ ] Deployment tested

---

## Future Enhancements

* Azure Landing Zones
* GitHub Actions
* Azure DevOps Pipelines
* Terraform Cloud
* Policy as Code
* FinOps Automation

---

## Status

🚧 Active Development

This section is being expanded with reusable Terraform modules, Azure deployment examples, governance frameworks, CI/CD integrations, and Infrastructure as Code best practices.
