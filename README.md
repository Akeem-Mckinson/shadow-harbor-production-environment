Shadow Harbor Capital Infrastructure

Project Overview

Shadow Harbor Capital Infrastructure is a production-style cloud infrastructure project designed to simulate the technology environment of a modern financial services organization.

The project demonstrates infrastructure deployment, security hardening, monitoring, automation, and Infrastructure as Code (IaC) using Microsoft Azure, Terraform, Linux, and NGINX.

The objective was to build and manage a secure cloud environment while applying industry-standard operational practices used by cloud and infrastructure engineers.

⸻

Technologies Used

* Microsoft Azure
* Terraform
* Ubuntu Linux
* NGINX
* Azure Monitor
* Azure Alert Rules
* Azure Action Groups
* UFW Firewall
* Fail2Ban
* Bash Scripting
* Cron Jobs
* SSH

⸻

Business Scenario

Shadow Harbor Capital is a fictional investment firm requiring a secure and reliable cloud environment to support business operations.

The infrastructure must provide:

* Secure remote administration
* Web service availability
* Monitoring and alerting
* Backup and recovery capabilities
* Infrastructure automation
* Operational visibility

Architecture

Internet
    ↓


Azure Public IP
    ↓


Network Security Group
    ↓


Ubuntu Linux VM
    ↓


NGINX Web Server
    ↓


Monitoring & Alerting
    ↓


Backup Automation

__________

Terraform Infrastructure as Code

Terraform was used to automate Azure resource provisioning through Infrastructure as Code (IaC).

Terraform Workflow

Initialize Terraform: 
terraform init
Review planned infrastructure: 
terraform plan
Deploy resources: 
terraform apply

Terraform Skills Demonstrated
* Infrastructure as Code
* Azure Provider Configuration
* Terraform State Management
* Resource Automation
* Cloud Provisioning
* Deployment Validation

Terraform Deployment Validation
Terraform successfully deployed Azure resources and validated infrastructure creation.

Example: Apply complete!
Resources: 1 added, 0 changed, 0 destroyed.

Azure Infrastructure

Resources deployed:

* Resource Group
* Virtual Network (VNet)
* Production Subnet
* Ubuntu Virtual Machine
* Public IP Address
* Network Security Group (NSG)
* Network Interface

Skills demonstrated:

* Azure Resource Management
* Virtual Networking
* Compute Services
* Security Configuration

⸻

Linux Administration

Connected securely using SSH and performed administrative operations.
Commands used:hostname,whoami,ip a,lsb_release -a

Tasks completed:

* Host validation
* User verification
* Network inspection
* Operating system verification
* System administration

Web Server Deployment

Installed and configured NGINX.

Commands:sudo apt update,sudo apt install nginx -y,sudo systemctl status nginx

Validation:

* Service running successfully
* Accessible through public IP address
* NGINX default webpage displayed

⸻

Security Hardening

UFW Firewall

Configured firewall rules for controlled access.
sudo ufw allow 22/tcp,sudo ufw allow 80/tcp,sudo ufw enable

Fail2Ban
Implemented intrusion prevention to protect SSH services.
sudo fail2ban-client status,sudo fail2ban-client status sshd

Security controls implemented:

* Firewall Management
* Intrusion Prevention
* SSH Protection
* Access Control

⸻

Monitoring and Alerting

Azure Monitor was configured to track infrastructure health.

Metrics Monitored

* CPU Utilization
* Available Memory Percentage
* Virtual Machine Availability

Alert Rules Created
CPU Alert:CPU > 80%
Memory Alert:Available Memory < 20%
Availability Alert:VM Availability < 100%

Notification System

Azure Action Groups were configured to send email notifications when alert thresholds are triggered.

Backup Automation
Created an automated backup solution using Bash scripting and Cron.
Backup script:/usr/local/bin/shadow-backup.sh
Backup destination:/var/backups/shadowharbor
Cron schedule:0 2 * * * /usr/local/bin/shadow-backup.sh

Capabilities:

* Automated backups
* Scheduled execution
* Reduced manual administration
* Improved recovery readiness

Skills Demonstrated
* Microsoft Azure
* Terraform
* Linux Administration
* Infrastructure as Code
* NGINX
* SSH
* Cloud Security
* Monitoring & Alerting
* Backup Automation
* Bash Scripting
* Cron Scheduling
* Infrastructure Operations

Project Outcomes

✅ Provisioned Azure Infrastructure

✅ Automated Deployment with Terraform

✅ Configured Secure SSH Access

✅ Deployed NGINX Web Server

✅ Implemented UFW Firewall

✅ Configured Fail2Ban

✅ Automated Backup Operations

✅ Implemented Azure Monitoring

✅ Created Alert Rules

✅ Configured Email Notifications

✅ Validated End-to-End Functionality


Key Takeaways

This project demonstrates the core responsibilities of a Cloud Infrastructure Engineer:

* Deploying cloud resources
* Managing Linux systems
* Implementing security controls
* Monitoring system health
* Automating operational tasks
* Managing infrastructure through code

The environment was built to simulate real-world operational requirements while applying cloud engineering, Linux administration, security, monitoring, and automation practices.