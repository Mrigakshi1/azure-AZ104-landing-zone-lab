# Azure Landing Zone Lab

## Project Overview

This project demonstrates the implementation of a secure and scalable Azure Landing Zone based on Microsoft Azure best practices. The environment was designed to establish governance, identity management, networking, security, monitoring, and cost control foundations required for cloud adoption.

The solution simulates an enterprise environment using a Hub-and-Spoke network architecture, Azure Policy, Role-Based Access Control (RBAC), Microsoft Entra ID, Azure Monitor, and Azure Storage.

---

## Objectives

- Implement Azure governance and compliance controls
- Configure identity and access management using Microsoft Entra ID
- Demonstrate Role-Based Access Control (RBAC)
- Deploy Hub-and-Spoke networking architecture
- Implement Azure Policy for standardization and compliance
- Configure monitoring and cost management
- Demonstrate secure storage access using Shared Access Signatures (SAS)

---

## Architecture Components

### Identity

- Microsoft Entra ID Users
- Microsoft Entra ID Groups
- Role Assignments

### Governance

- Azure Policy
- Resource Tagging Standards
- Naming Conventions

### Networking

- Hub Virtual Network
- Development Spoke VNet
- Production Spoke VNet
- VNet Peering

### Compute

- Development Virtual Machine
- Production Virtual Machine

### Monitoring

- Azure Monitor
- Metrics Collection
- Budget Alerts

### Storage

- Azure Storage Account
- Blob Container
- Shared Access Signature (SAS)

---

# Project Implementation

---

## Step 1 – Resource Group Design

Created dedicated resource groups for networking, identity, management, and workloads to support logical resource organization.

### Key Learning

- Resource organization
- Governance structure
- Environment separation

### Screenshot

![Resource Groups](screenshots/01-resource-groups.png)

---

## Step 2 – Microsoft Entra ID Configuration

Created users and security groups to simulate enterprise identity management and access control.

### Key Learning

- Identity management
- Group-based access control
- Azure authentication

### Screenshot

![Entra ID Users and Groups](screenshots/02-entra-users-groups.png)

---

## Step 3 – Azure RBAC Configuration

Configured Azure RBAC roles following the principle of least privilege.

### Roles Assigned

| Group | Role |
|---------|---------|
| Azure-Admins | Owner |
| Developers | Contributor |

### Key Learning

- Authorization
- Least privilege principle
- Role assignment management

### Screenshot

![RBAC Role Assignments](screenshots/03-rbac-role-assignments.png)

---

## Step 4 – Hub Virtual Network Deployment

Created the central Hub VNet to serve as the connectivity foundation for spoke networks.

### Configuration

```text
VNet Name: vnet-hub
Address Space: 10.0.0.0/16
```

### Key Learning

- Azure networking
- Hub-and-Spoke architecture

### Screenshot

![Hub VNet](screenshots/04-hub-vnet.png)

---

## Step 5 – Spoke Virtual Networks

Created separate VNets for Development and Production workloads.

### Configuration

```text
vnet-dev
10.1.0.0/16

vnet-prod
10.2.0.0/16
```

### Key Learning

- Network segmentation
- Environment isolation

### Screenshot

![Spoke VNets](screenshots/05-spoke-vnets.png)

---

## Step 6 – VNet Peering

Established bidirectional VNet peering between Hub and Spoke networks.

### Key Learning

- Private network connectivity
- Azure backbone networking
- Inter-VNet communication

### Screenshot

![VNet Peering](screenshots/06-vnet-peering.png)

---

## Step 7 – Virtual Machine Deployment

Deployed virtual machines in Development and Production environments.

### Resources

```text
vm-dev-01
vm-prod-01
```

### Key Learning

- Compute deployment
- VM administration

### Screenshot

![Virtual Machines](screenshots/07-virtual-machines.png)

---

## Step 8 – Azure Policy Implementation

Configured Azure Policy to enforce organizational standards and regional compliance.

### Policy Example

```text
Allowed Locations
```

### Key Learning

- Governance
- Compliance enforcement
- Standardization

### Screenshot

![Azure Policy](screenshots/08-azure-policy.png)

---

## Step 9 – Resource Tagging Policy

Implemented mandatory tagging requirements for resource governance.

### Required Tags

```text
Environment
Owner
CostCenter
```

### Key Learning

- Resource management
- Cost allocation
- Governance

### Screenshot

![Tagging Policy](screenshots/09-tagging-policy.png)

---

## Step 10 – Azure Storage Configuration

Configured a secure Azure Storage Account and Blob Container.

### Features Enabled

- HTTPS Only
- Secure Transfer Required
- Soft Delete

### Key Learning

- Storage security
- Blob storage management

### Screenshot

![Storage Account](screenshots/10-storage-account.png)

---

## Step 11 – Shared Access Signature (SAS)

Generated SAS Tokens to provide secure, time-limited access to Blob Storage resources.

### Key Learning

- Secure file sharing
- Temporary delegated access

### Screenshot

![SAS Token Access](screenshots/11-sas-token-access.png)

---

## Step 12 – Azure Monitor

Configured Azure Monitor to collect performance and operational metrics.

### Metrics Monitored

- CPU Utilization
- Network Activity
- VM Health

### Key Learning

- Monitoring
- Observability
- Operational visibility

### Screenshot

![Azure Monitor](screenshots/12-azure-monitor.png)

---

## Step 13 – Cost Management and Budget Alerts

Implemented budget monitoring and spending alerts.

### Budget

```text
50 USD
Alert Threshold: 80%
```

### Key Learning

- Cost optimization
- Budget management
- Financial governance

### Screenshot

![Budget Alert](screenshots/13-budget-alert.png)

---

## Skills Demonstrated

- Microsoft Azure
- Azure Administration
- Azure Governance
- Azure Policy
- Azure RBAC
- Microsoft Entra ID
- Azure Virtual Networks
- VNet Peering
- Azure Virtual Machines
- Azure Storage
- Azure Blob Storage
- Shared Access Signatures (SAS)
- Azure Monitor
- Azure Cost Management
- Cloud Security
- Infrastructure as a Service (IaaS)
- Hub-and-Spoke Architecture

---

## LinkedIn Project Description

Designed and implemented an Azure Landing Zone based on Microsoft best practices, incorporating governance, identity, networking, security, monitoring, and cost management. Configured Microsoft Entra ID, Azure RBAC, Azure Policy, Hub-and-Spoke networking, Azure Monitor, Azure Storage, and budget controls to simulate an enterprise cloud environment. Demonstrated cloud governance, operational management, and secure Azure infrastructure deployment aligned with Azure Cloud Adoption Framework principles.
