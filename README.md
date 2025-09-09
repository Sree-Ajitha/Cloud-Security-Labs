# ☁️ Cloud Security Labs

![GitHub last commit](https://img.shields.io/github/last-commit/Sree-Ajitha/Cloud-Security-Labs)  
![GitHub repo size](https://img.shields.io/github/repo-size/Sree-Ajitha/Cloud-Security-Labs)  
![GitHub issues](https://img.shields.io/github/issues/Sree-Ajitha/Cloud-Security-Labs)  

## 🎯 Overview
Hands-on labs for **Google Cloud Associate Cloud Engineer training**, focused on deploying, securing, and automating cloud infrastructure. Labs are structured for **practical experience** in real-world scenarios.

---

## 📂 Lab Modules & Links
Click on each lab to view detailed step-by-step guides:

| Lab | Description | Badge |
|-----|------------|-------|
| [01 – Compute & Storage](01_Compute_Storage.md) | VM deployment, Cloud Storage, Cloud SQL integration | ![Compute](https://img.shields.io/badge/Compute-Storage-blue) |
| [02 – Networking](02_Networking.md) | VPC, subnets, firewall rules, VPC peering | ![Networking](https://img.shields.io/badge/Networking-Secure-green) |
| [03 – IAM & Access](03_IAM_Access.md) | Service accounts, RBAC, IAM policies | ![IAM](https://img.shields.io/badge/IAM-Security-orange) |
| [04 – Security & Monitoring](04_Security_Monitoring.md) | Cloud Armor, BCE, logging & alerting | ![Monitoring](https://img.shields.io/badge/Security-Monitoring-red) |
| [05 – Automation](05_Automation.md) | Terraform, n8n workflows, IaC | ![Automation](https://img.shields.io/badge/Automation-IaC-purple) |
| [06 – Load Balancing & Scaling](06_Load_Balancing.md) | HTTP/Internal LB, autoscaling, Pub/Sub | ![Scaling](https://img.shields.io/badge/Scaling-High%20Availability-yellow) |

---

## 🏆 Key Achievements
- Earned **Google Cloud Associate Cloud Engineer** certification  
- Deployed **secure, scalable cloud infrastructure**  
- Automated workflows and infrastructure provisioning using **Terraform & n8n**  
- Applied **zero-trust principles and cloud security best practices**  
- Practiced hybrid cloud integration, monitoring, and resilience testing

---
```mermaid
flowchart LR
    subgraph Cloud[Oracle Cloud Infrastructure]
        OCI_VM[Ubuntu 24.04 Cloud Server]
        Cloud_Storage[Cloud Storage & SQL]
        OCI_VPN[VPN Gateway]
    end

    subgraph Local[Local VMware / WSL Environment]
        Kali_VM[Kali Linux 2025.1]
        Win_VM[Windows Server 2025 / Windows 11]
        Ubuntu_VM[Ubuntu 24.04]
        Metasploitable[Metasploitable 2]
    end

    subgraph Security[Monitoring & Automation]
        Splunk[Splunk SIEM & SOAR]
        Wazuh[Wazuh HIDS]
        Terraform[Terraform Automation]
        n8n[n8n Workflows]
    end

    OCI_VM --> Cloud_Storage
    OCI_VM --> OCI_VPN
    OCI_VPN --> Local
    Local --> Kali_VM
    Local --> Win_VM
    Local --> Ubuntu_VM
    Local --> Metasploitable
    Kali_VM --> Security
    Win_VM --> Security
    Ubuntu_VM --> Security
    Cloud_Storage --> Security
    Terraform --> Local
    Terraform --> Cloud
    n8n --> Security
```
---

> This repository serves as a **hands-on portfolio** demonstrating real-world cloud deployment, automation, and security skills.
