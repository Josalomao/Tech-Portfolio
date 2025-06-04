![osTicket Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/7/70/OsTicket_Logo.svg/512px-OsTicket_Logo.svg.png)

# osTicket - Post-Installation Configuration

---

## 🧰 Environments and Technologies Used

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

## 💻 Operating Systems Used

- Windows 10 (21H2)

---

## 🎯 Post-Install Configuration Objectives

1. Access the osTicket Admin Panel
2. Configure Roles
3. Configure Departments
4. Configure Teams
5. Configure Help Topics

---

## 🛠️ Configuration Steps

### 1. Access the osTicket Admin Panel

- Navigate to: `http://localhost/osTicket/scp/login.php`
- Log in using the admin credentials created during installation.

### 2. Configure Roles

Roles define the permissions granted to agents within specific departments.

1. Navigate to: **Admin Panel → Agents → Roles**
2. Click on **Add New Role**
3. Enter a role name (e.g., "Support Agent")
4. Assign appropriate permissions for the role.
5. Save the role.

### 3. Configure Departments

Departments categorize incoming tickets and can be used to control agent access.

1. Navigate to: **Admin Panel → Agents → Departments**
2. Click on **Add New Department**
3. Enter a department name (e.g., "Technical Support")
4. Set other preferences as needed.
5. Save the department.

### 4. Configure Teams

Teams allow grouping agents from different departments to handle specific issues.

1. Navigate to: **Admin Panel → Agents → Teams**
2. Click on **Add New Team**
3. Enter a team name (e.g., "Level 1 Support")
4. Assign agents to the team.
5. Save the team.

### 5. Configure Help Topics

Help Topics streamline ticket categorization and routing.

1. Navigate to: **Admin Panel → Manage → Help Topics**
2. Click on **Add New Help Topic**
3. Enter a topic name (e.g., "Password Reset")
4. Assign to the appropriate department.
5. Set other preferences as needed.
6. Save the help topic.

---

## Disk Sanitization Steps
1. Delete all test data and users from the osTicket system.
2. Power off the Virtual Machines in Azure.
3. Delete the VMs and associated storage disks via the Azure Portal.
4. Confirm no data remnants exist in the Resource Group.
