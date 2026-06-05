# Azure Traffic Manager Deployment

This repository contains an Azure Resource Manager (ARM) template to deploy a global, high-performance **Azure Traffic Manager Profile**. 

Traffic Manager acts as a DNS-based traffic load balancer, intelligently routing incoming user requests to the best-performing destination endpoint based on geographic network latency.

## Architecture Overview

[ User Request ]
                           │
                           ▼
           [ <uniqueDnsName>.trafficmanager.net ]
                           │
           ┌───────────────┴───────────────┐
           ▼ (Low Latency / East US)        ▼ (Low Latency / West US)
  [ endpoint1: www.shehan.cloud ]    [ endpoint2: [www.google.com](https://www.google.com) ]


* **Routing Method:** `Performance` (Routes users to the closest available endpoint).
* **Health Monitoring:** Proactively probes endpoints via **HTTPS (Port 443)** on the root path (`/`).
* **Failover Engine:** Automatically shifts traffic away from unhealthy endpoints within 30 seconds if a target returns an error or times out.

---

## File Structure

* `template.json`: The fully commented, valid ARM deployment file specifying the Traffic Manager resource, monitoring configuration, and targets.

---

## Prerequisites

Before deploying, ensure you have:
1. An active Azure account and subscription.
2. The [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli) installed locally.
3. An existing Resource Group in your Azure subscription.

---

## Deployment Steps

Follow these steps to deploy the infrastructure using the Azure CLI[cite: 2]:

### 1. Authenticate to Azure
Open your terminal and log into your Azure account[cite: 2]:
```bash
az login

az deployment group show \
  --resource-group "rg-production-global" \
  --name "deploy-traffic-manager-v1" \
  --query "properties.provisioningState"
