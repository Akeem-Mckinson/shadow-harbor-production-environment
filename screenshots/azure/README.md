# Azure Infrastructure Deployment

## Overview

This section documents the Azure infrastructure deployed for the Shadow Harbor Production Environment project.

The goal of this deployment was to build a production-style Linux server environment in Microsoft Azure and prepare it for Linux administration, web hosting, monitoring, security hardening, and automation.

---

## Technologies Used

- Microsoft Azure
- Ubuntu Linux
- Azure Virtual Machines
- Azure Resource Groups
- Azure Virtual Network (VNet)
- Network Security Groups (NSG)
- SSH Authentication
- Azure Monitor
- Azure Alerts

---

## Infrastructure Components

### Resource Group

Created a dedicated production resource group:

- rg-shadowharbor-prod

This resource group contains all infrastructure resources associated with the project.

---

### Virtual Machine

Provisioned an Ubuntu Linux virtual machine:

- VM Name: vm-linux-prod-01
- Operating System: Ubuntu 24.04 LTS
- Size: Standard D2s v3
- Public IP Enabled
- SSH Access Configured

---

### Networking

Configured networking resources including:

- Virtual Network
- Production Subnet
- Public IP Address
- Network Security Group

SSH access was restricted through Azure networking controls.

---

### Monitoring

Configured Azure Monitor to track:

- CPU Utilization
- Available Memory
- VM Availability

Metrics were visualized through Azure Monitor dashboards.

---

### Alerting

Configured operational alerts including:

#### CPU Alert

- Trigger when CPU exceeds 80%
- Evaluation Period: 15 Minutes
- Severity: Warning

#### Memory Alert

- Trigger when available memory falls below 20%
- Severity: Warning

#### Availability Alert

- Trigger when VM availability drops below expected thresholds
- Severity: Critical

Email notification actions were configured for alert delivery.

---

## Screenshots

### Infrastructure Deployment

- azure-00-vm-creation.png
- azure-01-resource-group.png
- azure-02-vm-overview.png
- azure-03-ssh-configuration.png

### Monitoring and Operations

- azure-04-monitoring-metrics.png
- azure-05-alert-rules.png
- azure-06-cpu-alert-configuration.png

---

## Skills Demonstrated

- Azure Infrastructure Deployment
- Virtual Machine Administration
- Linux Server Provisioning
- Network Configuration
- SSH Connectivity
- Azure Monitoring
- Azure Alert Management
- Operational Visibility
- Infrastructure Documentation

---

## Project Outcome

Successfully deployed and configured a production-style Azure Linux environment with monitoring, alerting, networking, and operational visibility.

This environment serves as the foundation for Linux administration, NGINX deployment, security hardening, backup automation, and Infrastructure as Code workflows throughout the Shadow Harbor Production Environment project.
