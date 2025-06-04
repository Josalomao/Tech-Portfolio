<p align="center">
  <img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

# On-premises Active Directory Deployed in the Cloud (Azure)

This project demonstrates deploying and configuring an Active Directory environment entirely within Microsoft Azure using Virtual Machines.

---

## 🧰 Environments and Technologies Used

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

---

## 💻 Operating Systems Used

- Windows Server 2022
- Windows 10 (21H2)

---

## 🧭 High-Level Deployment and Configuration Steps

1. Provision two Virtual Machines in Microsoft Azure  
2. Install and configure Active Directory Domain Services (AD DS) on the Windows Server VM  
3. Join the Windows 10 client VM to the domain  
4. Create and manage users, groups, and OUs using Active Directory tools  

---

## 🛠️ Deployment and Configuration Steps

### 1. Provision Virtual Machines in Azure

- Create a Resource Group
- Deploy a Windows Server 2022 VM (to serve as the Domain Controller)
- Deploy a Windows 10 VM (to serve as the domain-joined client)
- Ensure both VMs are on the same virtual network and subnet

### 2. Install Active Directory Domain Services

- Log into the Windows Server VM using Remote Desktop
- Open **Server Manager → Add Roles and Features**
- Select **Active Directory Domain Services**, complete the wizard
- Promote the server to a **Domain Controller** and create a new forest (e.g., `josiaslab.local`)

### 3. Join Windows 10 VM to the Domain

- Log into the Windows 10 VM
- Set DNS to point to the domain controller's private IP
- Go to **System Properties → Change settings → Domain**
- Enter the domain (e.g., `josiaslab.local`) and credentials
- Restart the machine to complete the join

### 4. Create and Manage Users/Groups

- On the domain controller, open **Active Directory Users and Computers**
- Create Organizational Units (OUs), Users, and Security Groups
- Use **Group Policy Management** to explore policies
- Optionally, use PowerShell to automate tasks like user creation

---

## 🔒 Disk Sanitization Steps

1. Remove all user accounts and test objects created during the lab  
2. Power off both VMs in Azure  
3. Delete the Virtual Machines and associated storage disks via the Azure Portal  
4. Ensure the Resource Group is cleaned up with no remaining resources  
