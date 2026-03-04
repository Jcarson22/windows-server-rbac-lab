# windows-server-rbac-lab
Windows Server 2022 lab demonstrating role-based access control (RBAC), user/group management, and NTFS permissions.

## Overview
This lab demonsrates how to implement **Role-Based Access Control (RBAC)** using NTFS permissions on a Windows file server.
The objective was to simulate a company file server where departments can only access their own data. Users are assigned to security groups, and groups control access to folders.
This lab was built using a virtualized Windows Server environment.

---

# Technologies Used
- Windows server 2022
- Oracle VirtualBox
- NTFS Permissions
- Windows Local User and Groups
- Server Manager

---

## Lab Environment
Host Machine:
-Windows 11

Virtual Machine:
- Windows Server 2022
- 6GB RAM
- 2 CPU cores
- 60GB virtual disk
- NAT networking

Visualization Platform:
-Oracle VirtualBox

---
## File Server Structure
```
C:\Company
│
├── HR
├── Finance
└── IT
```
Each department folder is restricted so that only the corresponding group can access it.
---
## Users Created

| User | Department |
|-----|-----|
| Derek Jeter | HR |
| Alex Rodriguez | Finance |
| Babe Ruth | IT |

---

## Security Groups

| Group | Members |
|-----|-----|
| HR | Derek Jeter |
| Finance | Alex Rodriguez |
| IT | Babe Ruth |

Users are placed into groups, and groups control access to resources.

---
## Permission Model (RBAC)

Instead of assigning permissions directly to users:

```
User → Group → Folder
```

This approach simplifies management and follows enterprise security best practices.

---
## Skills Demonstrated

- Windows Server administration
- File system management
- User account creation
- Security group management
- NTFS permission configuration
- Role-Based Access Control (RBAC)

---
## Screenshots

Screenshots demonstrating the configuration process will be included in the `screenshots` folder.

Examples include:
- Server Manager dashboard
- Folder structure configuration
- User creation
- Group creation
- NTFS permissions configuration

---
## Key Takeaways

This lab demonstrates foundational **system administration skills** used in enterprise IT environments.

RBAC principles implemented here are also used in:

- Active Directory
- AWS IAM
- Azure RBAC
- Linux group permissions

Understanding these concepts is essential for systems administration and cloud infrastructure roles.
