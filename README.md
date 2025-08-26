# osTicket — Post-Install Configuration

This tutorial walks through the post-installation configuration of **osTicket**, setting up roles, departments, teams, SLA plans, and help topics.

---

## YouTube Demonstration

[![YouTube Demo](https://img.youtube.com/vi/PLACEHOLDER_VIDEO_ID/0.jpg)](https://www.youtube.com/watch?v=PLACEHOLDER_VIDEO_ID)

> *Click the thumbnail to watch a walkthrough video.*

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

**Path:** `Admin Panel → Agents → Roles`  
Example Role: **Supreme Admin**  

![Roles Screenshot](https://via.placeholder.com/600x300.png?text=Roles+Configuration+Screenshot)

[Documentation](https://docs.osticket.com/en/latest/Admin/Agents/Roles.html)

---

### 2. Departments (Ticket Visibility)

**Path:** `Admin Panel → Agents → Departments`  
Example Department: **SysAdmins**

![Departments Screenshot](https://via.placeholder.com/600x300.png?text=Departments+Configuration+Screenshot)

[Documentation](https://docs.osticket.com/en/latest/Admin/Agents/Departments.html)

---

### 3. Teams (Cross-Department Groups)

**Path:** `Admin Panel → Agents → Teams`  
Example Team: **Online Banking**

![Teams Screenshot](https://via.placeholder.com/600x300.png?text=Teams+Configuration+Screenshot)

[Documentation](https://docs.osticket.com/en/latest/Admin/Agents/Teams.html)

---

### 4. User Settings

**Path:** `Admin Panel → Settings → User Settings`  
> Uncheck “**unregistered users can create tickets**” to require registration.

![User Settings Screenshot](https://via.placeholder.com/600x300.png?text=User+Settings+Screenshot)

---

### 5. Agents (Workers)

**Path:** `Admin Panel → Agents → Add New`  
Example Agents:  
- Chris (Dept: SysAdmins) – pass: `chris1`  
- Yasmine (Dept: Support) – pass: `yasmine`

![Agents Screenshot](https://via.placeholder.com/600x300.png?text=Agents+Configuration+Screenshot)

[Documentation](https://docs.osticket.com/en/latest/Admin/Agents/Agents.html)

---

### 6. Users (Customers)

**Path:** `Agent Panel → Users → Add New`  
Example Users:  
- Karen  
- Ken  

![Users Screenshot](https://via.placeholder.com/600x300.png?text=Users+Configuration+Screenshot)

[Documentation](https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html)

---

### 7. SLA Plans

**Path:** `Admin Panel → Manage → SLA`  
- **Sev-A:** Grace 1 hour (24/7)  
- **Sev-B:** Grace 4 hours (24/7)  
- **Sev-C:** Grace 8 hours (Business Hours)

![SLA Screenshot](https://via.placeholder.com/600x300.png?text=SLA+Plans+Screenshot)

[Documentation](https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html)

---

### 8. Help Topics

**Path:** `Admin Panel → Manage → Help Topics`  
Examples:  
- Business-Critical Outage  
- Personal Computer Issues  
- Equipment Request  
- Password Reset  
- Other  

![Help Topics Screenshot](https://via.placeholder.com/600x300.png?text=Help+Topics+Screenshot)

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
