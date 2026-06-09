# IT-Support-Lab-Isolated-Network
"Isolated heterogeneous Linux lab environment with static IP configuration and cross-distro connectivity testing."

# IT Support Lab: Isolated Network Environment

## 🎯 Project Overview
Created a completely isolated network environment using VMware with two different Linux distributions (Linux Mint and Debian) configured with static IP addresses. This lab simulates a secure corporate testing environment where servers are isolated from the internet and can communicate with each other.

## 🛠 Lab Configuration

### Network Details
- **Network Subnet:** 192.168.20.0/24
- **Netmask:** 255.255.255.0
- **Gateway:** 192.168.20.1
- **Isolation:** Complete (no internet access, private LAN only)

### Virtual Machines
1. **Linux Mint Workstation**
   - IP Address: 192.168.20.11
   - Role: Client/User Workstation
   - Purpose: Simulate end-user computer

2. **Debian Server**
   - IP Address: 192.168.20.10
   - Role: Server
   - Purpose: Simulate backend infrastructure

## ✅ Verification & Testing

### Cross-Distro Connectivity
Successfully verified bidirectional communication between VMs:
- From Mint: `ping 192.168.20.10` ✓ Success
- From Debian: `ping 192.168.20.11` ✓ Success

### Commands Used
```bash
# Check IP configuration
ip a

# Test connectivity
ping 192.168.20.10
ping 192.168.20.11
