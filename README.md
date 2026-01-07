# Azure Identity & Access Mini-Lab (Microsoft Entra ID)

## Overview
This project demonstrates hands-on experience with **Microsoft Entra ID (formerly Azure Active Directory)**, focusing on cloud identity and access management.

The lab is designed to reflect a **university IT environment**, where faculty, staff, students, and IT administrators require different access levels, security controls, and monitoring.

This project serves as a **starter identity lab** and provides a strong foundation for future work with **Hybrid Active Directory, Microsoft Intune, and Microsoft 365 administration**.

---

## Technologies Used
- Microsoft Entra ID (Azure Active Directory)
- Azure Portal
- Conditional Access / Security Defaults
- Multi-Factor Authentication (MFA)

---

## 1. Entra ID Tenant Setup
An Entra ID tenant was created and reviewed to represent the organization’s **identity boundary**, where all users, roles, and security policies are managed centrally.

**Tenant Overview**
<img width="4000" height="3000" alt="Tenant-Overview" src="https://github.com/user-attachments/assets/f506c0d9-501f-4995-94b2-8973bc35a015" />


---

## 2. User Management
Cloud users were created to represent common roles found in a university environment:
- IT Administrator  
- IT Support  
- Faculty/Staff  
- Student  

Password policies were configured, and users were required to change their password at first sign-in to improve security.

**Users List**
<img width="1873" height="950" alt="Users-List" src="https://github.com/user-attachments/assets/c1ad68b0-44c1-435d-8c79-149057282204" />


**Individual User Profile**
<img width="1876" height="950" alt="User-profile-IDadmin - Copy" src="https://github.com/user-attachments/assets/4e6383b9-06c6-4c14-894d-04e6dee415f0" />



---

## 3. Security Groups
Security groups were created to support **group-based access control**, allowing permissions and policies to be applied efficiently and at scale.

Groups created:
- `IT_Admins`
- `Faculty_Staff`
- `Students`

Users were assigned to groups based on their organizational role.

**Groups Overview**
<img width="1871" height="951" alt="Groups-List" src="https://github.com/user-attachments/assets/4e8eeb8d-ac6e-40cc-bb15-ec9a424c298d" />


**IT_Admins Group Membership**
<img width="1872" height="948" alt="Group-ITAdmin-members" src="https://github.com/user-attachments/assets/7dd5abb3-c91c-4a87-aa12-c8c192cdc381" />


---

## 4. Role-Based Access Control (RBAC)
Administrative roles were assigned following the **principle of least privilege** to reduce security risk.

Roles assigned:
- **User Administrator** – IT Support account  
- **Global Reader** – Read-only administrative access  

Global Administrator access was intentionally kept limited.

**User Administrator Role Assignment**
<img width="1916" height="951" alt="roles-useradmin" src="https://github.com/user-attachments/assets/f4f3f934-79df-4d9c-a8fc-441c87c9690e" />


**Global Reader Role Assignment**
<img width="1912" height="950" alt="roles-globalreader" src="https://github.com/user-attachments/assets/9a9927b0-90b7-4d38-b611-55b3f0470946" />


---

## 5. Security Configuration (MFA Enforcement)
Privileged accounts were secured by enforcing **Multi-Factor Authentication (MFA)** using Conditional Access or Security Defaults.

This helps protect administrative accounts from credential compromise.

**Conditional Access / Security Defaults**
<img width="429" height="903" alt="Security-Defaults-enabled" src="https://github.com/user-attachments/assets/43ff26b3-9f06-48d0-a8cf-48afda7f0563" />


---

## 6. Authentication Monitoring (Sign-In Logs)
Sign-in logs were reviewed to verify successful authentication, MFA enforcement, and Conditional Access outcomes.

This is essential for troubleshooting access issues and identifying suspicious sign-in activity.

**Sign-In Logs**
<img width="1855" height="844" alt="signin-logs-list" src="https://github.com/user-attachments/assets/2c9b6abf-0663-4150-9dbf-11839f72b160" />


---

## 7. Administrative Monitoring (Audit Logs)
Audit logs were reviewed to track administrative actions such as:
- User creation  
- Group membership changes  
- Role assignments  
- Security policy updates  

**Audit Logs**
*Add Members*

<img width="1857" height="507" alt="Add-Member-To-Group" src="https://github.com/user-attachments/assets/050a66ee-e9ff-45c4-9586-b8b75595f80e" />


*Add User*

<img width="1859" height="597" alt="Add-User-Logs" src="https://github.com/user-attachments/assets/2ce47228-9d29-48b9-8a9e-76ee5778835a" />


---

## Key Concepts Practiced
- Cloud identity management  
- Group-based access control  
- Role-based access control (RBAC)  
- Least-privilege security model  
- Multi-Factor Authentication (MFA)  
- Identity monitoring and troubleshooting  

---

## Why This Project Is Relevant
This project reflects real-world identity administration tasks performed by **Systems Administrators** in a university environment, including:
- Managing faculty, staff, and student identities  
- Securing privileged administrative accounts  
- Monitoring authentication and administrative activity  
- Preparing for hybrid identity integration  

---

## Next Steps
This lab will be expanded to include:
- On-premises Active Directory Domain Services (AD DS)  
- Azure AD Connect (Hybrid Identity)  
- Microsoft Intune device management  
- Microsoft 365 user and license administration  
- PowerShell automation for identity tasks  

---

## Author
**Kristin**  
Computer Science Graduate, Acadia University (May 2025)  
Aspiring Cloud/Systems Administrator | Microsoft Cloud & Hybrid Identity
