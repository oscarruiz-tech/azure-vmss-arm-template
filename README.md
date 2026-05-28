# azure-vmss-arm-template
# High Availability and Auto-Scaling Architecture on Azure using VMSS and ARM Templates

## 📌 Project Overview
This project demonstrates the design and implementation of a highly available and fault-tolerant cloud network infrastructure on Microsoft Azure. It utilizes a **Virtual Machine Scale Set (VMSS)** deployed in uniform mode behind an **Azure Load Balancer**, ensuring automated scaling, traffic distribution, and standardized resource management.

## 🏗️ Architecture & Core Components
- **Compute:** Scalable Ubuntu Server instances orchestrated symmetrically via Virtual Machine Scale Sets (Uniform Orchestration Mode).
- **Networking:** A private Virtual Network (VNet) coupled with a Network Security Group (NSG) configured to safely handle inbound HTTP (Port 80) and SSH (Port 22) traffic.
- **Monitoring & Health Checks:** Infrastructure health telemetry applied via Azure Linux extensions (`ApplicationHealthLinux`) targeting the `/health.html` endpoint.
- **Infrastructure as Code (IaC):** Full declarative definition of the cloud ecosystem using native Azure Resource Manager (ARM) templates.

## 📄 Repository Files
- `template.json`: The complete Azure Resource Manager (ARM) blueprint declaring all cloud infrastructure, network topology, and compute profiles.
