![osTicket Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/7/70/OsTicket_Logo.svg/512px-OsTicket_Logo.svg.png)

# osTicket - Prerequisites and Installation

---

## 🧰 Environments and Technologies Used
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

## 💻 Operating Systems Used
- Windows 10 (21H2)

## ✅ List of Prerequisites
1. Microsoft Azure account
2. Virtual Machine with Windows 10 (21H2)
3. Remote Desktop Connection enabled
4. Internet Information Services (IIS) installed
5. PHP and MySQL setup

## 🛠 Installation Steps
1. Deploy Windows 10 VM in Azure
2. Connect to VM via RDP
3. Install IIS, PHP, and MySQL
4. Download and install osTicket
5. Configure MySQL database and osTicket settings

## 🔒 Disk Sanitization Steps
- Delete all test tickets and users in osTicket
- Power off the VM
- Delete the VM and its associated disks from Azure
- Confirm resource group is cleared of sensitive data
