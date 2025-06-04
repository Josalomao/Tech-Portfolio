![osTicket Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/7/70/OsTicket_Logo.svg/512px-OsTicket_Logo.svg.png)

# osTicket - Ticket Lifecycle: Intake Through Resolution

---

## 🧰 Environments and Technologies Used

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

---

## 💻 Operating Systems Used

- Windows 10 (21H2)

---

## 🔄 Ticket Lifecycle Stages

### 1. **Intake**
- A user submits a support ticket through the client portal.
- Required fields are filled in (e.g., name, email, help topic, message).
- The ticket is logged and visible to support agents.

### 2. **Assignment and Communication**
- The ticket is assigned to a department and/or specific agent.
- Internal or external notes can be added.
- Agents can communicate with the user through ticket responses.

### 3. **Working the Issue**
- The agent begins investigating and addressing the issue.
- Troubleshooting steps and status updates are documented in the ticket.
- The status might change (e.g., Open → In Progress).

### 4. **Resolution**
- Once the issue is resolved, the agent updates the final response.
- The ticket is marked as **Resolved** or **Closed**.
- End-user receives notification and, optionally, can reopen the ticket.

---

## 🔒 Disk Sanitization Steps

1. Delete all test data and users from the osTicket system.
2. Power off the Virtual Machines in Azure.
3. Delete the VMs and associated storage disks via the Azure Portal.
4. Confirm no data remnants exist in the Resource Group.

---
