<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

# On-premises Active Directory Deployed in the Cloud (Azure)

## Environments and Technologies Used
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

## Operating Systems Used
- Windows Server 2022
- Windows 10 (21H2)

## Deployment and Configuration Steps
1. Create Windows Server 2022 VM
2. Set static IP & DNS
3. Install Active Directory Domain Services
4. Promote the server to a Domain Controller
5. Test domain joins with a Windows 10 VM

## Disk Sanitization Steps
1. Remove domain-joined test VMs
2. Demote and delete domain controller
3. Power off and delete all Azure resources
4. Ensure all VHDs are deleted
