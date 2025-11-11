https://github.com/victoria-spec/Ontario-Skills-Competition/tree/main
# 🖥️ Hyper-V Template VMs

A collection of **preconfigured Hyper-V virtual machine templates** for quick deployment and testing of Windows operating systems.

## 📦 Overview

This repository provides Hyper-V templates for the following Microsoft operating systems:

1. **Windows 11**
2. **Windows Server 2022**
3. **Windows Server 2019**
4. **Windows Server 2025**

Each template is optimized for:
- Fast deployment
- Sysprep generalization
- Standardized configuration (CPU, RAM, network, etc.)
- Easy cloning and customization

---

## 🧱 VM Specifications

| OS Version | Edition | Default CPU | Default RAM | Disk Size | Notes |
|-------------|----------|--------------|--------------|------------|--------|
| Windows 11 | Pro / Enterprise | 2 vCPU | 4 GB | 64 GB | Secure Boot + TPM enabled |
| Windows Server 2019 | Standard / Datacenter | 2 vCPU | 4 GB | 100 GB | Core + Desktop Experience |
| Windows Server 2022 | Standard / Datacenter | 2 vCPU | 8 GB | 127 GB | Core + Desktop Experience |
| Windows Server 2025 | Standard / Datacenter | 2 vCPU | 8 GB | 127 GB | Preview build (if applicable) |

---

## 🛠️ Prerequisites

Before using these templates, ensure you have:
- **Windows 10/11 Pro or Enterprise** with **Hyper-V** feature enabled  
- **Sufficient disk space** for multiple virtual hard disks (VHDX)  
- **Administrator privileges**  
- **ISO images** for Windows installation (if not already included)

Enable Hyper-V (if not already done):
```powershell
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All
