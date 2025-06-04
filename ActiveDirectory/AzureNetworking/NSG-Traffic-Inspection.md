# 🛰️ Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines

---

## 🧰 Environments and Technologies Used

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Wireshark (Protocol Analyzer)
- Network Protocols: SSH, RDP, DNS, HTTP/S, ICMP

---

## 💻 Operating Systems Used

- Windows 10 (21H2)
- Ubuntu Server 20.04

---

## 🧭 High-Level Steps

1. Deploy a Windows 10 VM and an Ubuntu VM in the same Virtual Network
2. Install and configure Wireshark on the Windows VM
3. Send various types of traffic between the VMs using different protocols
4. Modify NSG rules and observe changes in connectivity and traffic capture

---

## 🔍 Actions and Observations

### 1. Deploy Azure VMs
- Create a **Windows 10 VM** and an **Ubuntu Server 20.04 VM** in the same Resource Group and Virtual Network.
- Allow necessary inbound ports in the NSG (e.g., SSH for Ubuntu, RDP for Windows).

### 2. Install Wireshark on Windows VM
- Download and install Wireshark.
- Run Wireshark as administrator and begin capturing on the appropriate network interface.

### 3. Generate and Analyze Network Traffic
- From the Windows VM, initiate:
  - **ICMP** (Ping) to Ubuntu
  - **HTTP/S** requests using a browser or curl
  - **DNS** queries via nslookup
  - **RDP or SSH** connections
- Watch for packets in Wireshark (use filters like `icmp`, `tcp.port == 443`, etc.)

### 4. Modify NSG Rules
- Edit NSG rules in Azure to **allow**, **deny**, or **restrict** specific traffic types.
- Observe how traffic is blocked or allowed in real-time via Wireshark and connection attempts.

---

## 🔒 Disk Sanitization Steps

1. Delete all captured data, logs, or temporary tools from the VMs.  
2. Power off the Virtual Machines in Azure.  
3. Delete the VMs and associated storage disks via the Azure Portal.  
4. Confirm all resources in the Resource Group are deleted.  

---
