# osTicket — Post-Install Configuration

This tutorial walks through the post-installation configuration of **osTicket**, setting up roles, departments, teams, SLA plans, and help topics.

---

## Environments and Technologies Used

- **Microsoft Azure** – Virtual Machines / Compute  
- **Remote Desktop Protocol (RDP)** – To connect to VMs  
- **Internet Information Services (IIS)** – For hosting osTicket  
- **osTicket** – Ticketing System

---

## Operating Systems Used

- **Windows 10 (21H2)**  

---

## Post-Install Configuration Objectives

- Understand **Agent Panel vs Admin Panel**
- Create and configure **Roles, Departments, Teams**
- Add **Agents (workers)** and **Users (customers)**
- Define **SLA Plans** and **Help Topics**
- Secure ticket creation by enabling registration

---

## Configuration Steps

### 1. Roles (Grouping Permissions)

Purpose: Define what each group of agents can and cannot do in the system.

**Path:** `Admin Panel → Agents → Roles`  
Example Role: **Supreme Admin**  

![Roles Screenshot](https://github.com/user-attachments/assets/e404676c-1b43-49c2-ac38-7e608afa72e0)

[Documentation](https://docs.osticket.com/en/latest/Admin/Agents/Roles.html)

---

### 2. Departments (Ticket Visibility)

Purpose: Organize your helpdesk into logical groups; tickets can be assigned to specific departments.

**Path:** `Admin Panel → Agents → Departments`  
Example Department: **SysAdmins**

![Departments Screenshot](https://github.com/user-attachments/assets/ac4ec845-8d58-442f-9cc2-960367511f9d)

[Documentation](https://docs.osticket.com/en/latest/Admin/Agents/Departments.html)

---

### 3. Teams (Cross-Department Groups)

Purpose: Pull agents from multiple departments into specialized teams for certain issues.

**Path:** `Admin Panel → Agents → Teams`  
Example Team: **Online Banking**

![Teams Screenshot](https://github.com/user-attachments/assets/69806f19-8906-4cea-b523-fa475f9ac604)


[Documentation](https://docs.osticket.com/en/latest/Admin/Agents/Teams.html)

---

### 4. User Settings

Purpose: Define how users can create tickets.

**Path:** `Admin Panel → Settings → User Settings`  
> Uncheck “**unregistered users can create tickets**” to require registration.

![User Settings Screenshot](https://github.com/user-attachments/assets/06d839b5-4c6c-4504-b015-af8fdcd3e744)

---

### 5. Agents (Workers)

Purpose: Create accounts for helpdesk workers who will manage tickets.

**Path:** `Admin Panel → Agents → Add New`  
Example Agents:  
- Chris (Dept: SysAdmins) 
- Yasmine (Dept: Support) 

![Agents Screenshot](https://github.com/user-attachments/assets/ae439ebd-6386-4a74-8556-7e3ff3049363")

[Documentation](https://docs.osticket.com/en/latest/Admin/Agents/Agents.html)

---

### 6. Users (Customers)

Purpose: Add end users who will submit support tickets.

**Path:** `Agent Panel → Users → Add New`  
Example Users:  
- Karen  
- Ken  

![Users Screenshot](https://github.com/user-attachments/assets/31d5622c-8d7a-485a-bd80-bcb54b81d30d")

[Documentation](https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html)

---

### 7. SLA Plans

Purpose: Define response and resolution times based on issue severity.

**Path:** `Admin Panel → Manage → SLA`  
- **Sev-A:** Grace 1 hour (24/7)  
- **Sev-B:** Grace 4 hours (24/7)  
- **Sev-C:** Grace 8 hours (Business Hours)

![SLA Screenshot](https://github.com/user-attachments/assets/3f786704-b32f-4c79-a855-3e8d8853630c")

[Documentation](https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html)

---

### 8. Help Topics

Purpose: Help users select the right category when submitting tickets.

**Path:** `Admin Panel → Manage → Help Topics`  
Examples:  
- Business-Critical Outage  
- Personal Computer Issues  
- Equipment Request  
- Password Reset  
- Other  

![Help Topics Screenshot](https://github.com/user-attachments/assets/31dd9e80-b699-4c41-a7e8-25ff5950b29a")

[Documentation](https://docs.osticket.com/en/latest/Admin/Manage/Help%20Topic.html)

---

## References

- [osTicket Roles](https://docs.osticket.com/en/latest/Admin/Agents/Roles.html)  
- [osTicket Departments](https://docs.osticket.com/en/latest/Admin/Agents/Departments.html)  
- [osTicket Teams](https://docs.osticket.com/en/latest/Admin/Agents/Teams.html)  
- [osTicket Agents](https://docs.osticket.com/en/latest/Admin/Agents/Agents.html)  
- [osTicket Users](https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html)  
- [osTicket SLA Plans](https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html)  
- [osTicket Help Topics](https://docs.osticket.com/en/latest/Admin/Manage/Help%20Topic.html)
