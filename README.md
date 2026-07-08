# Active Directory Home Lab

## Overview

This project documents the creation of a Windows Server Active Directory home lab built in a virtualized environment using KVM/QEMU. The goal of this lab was to gain hands-on experience with Windows Server administration, Active Directory Domain Services (AD DS), user and group management, file sharing, and troubleshooting common enterprise administration tasks.

This lab was built to simulate a small business environment and strengthen practical IT administration skills beyond classroom learning.

---

## Objectives

- Deploy a Windows Server virtual machine
- Install and configure Active Directory Domain Services (AD DS)
- Promote the server to a Domain Controller
- Create an Active Directory domain
- Organize resources using Organizational Units (OUs)
- Create and manage domain users and security groups
- Configure shared folders
- Practice Windows administration and troubleshooting

---

## Lab Environment

### Host System

- Arch Linux
- KVM/QEMU
- virt-manager

### Virtual Machines

- Windows Server 2022
- Windows 11 Client

---

## Technologies Used

- Active Directory Domain Services
- Windows Server 2022
- Windows 11
- DNS
- NTFS Permissions
- SMB File Sharing
- KVM/QEMU Virtualization
- Virt-Manager

---

# Active Directory Deployment

The Windows Server virtual machine was promoted to a Domain Controller using Active Directory Domain Services.

The server was configured to host the lab domain and provide centralized authentication and management for domain resources.

Completed tasks included:

- Installing AD DS
- Promoting the server to a Domain Controller
- Creating the Active Directory domain
- Verifying domain functionality
- Managing the environment through Server Manager

---

# Organizational Unit Structure

To simulate an enterprise environment, Organizational Units (OUs) were created for administrative organization.

Example structure:

```
HOMELAB
├── Users
├── Groups
├── Computers
├── Servers
├── HR
└── IT
```

---

# User Management

Multiple domain user accounts were created to simulate employees.

Tasks completed:

- Created domain user accounts
- Configured passwords
- Assigned users to appropriate Organizational Units
- Verified successful account creation

---

# Group Management

Security groups were created to simplify permission management.

Examples include:

- HR_Users
- IT_Users

Users were assigned to department-specific security groups to support role-based access control.

---

# File Server

A departmental file share structure was created.

```
C:\Shares
├── HR
├── IT
└── Finance
```

The lab included configuring:

- Shared folders
- NTFS permissions
- Share permissions
- Security group access

During implementation, permission conflicts were encountered and resolved, providing valuable experience troubleshooting Windows file permissions.

---

# Troubleshooting Experience

One of the most valuable parts of this project was resolving real administrative issues.

Examples included:

- Virtual machine networking configuration
- Driver installation during Windows Server deployment
- Active Directory installation prerequisites
- DNS configuration
- Windows file permission troubleshooting
- NTFS and Share permission configuration
- User access validation

Working through these problems provided hands-on experience similar to real-world IT support scenarios.

---

# Skills Demonstrated

- Windows Server Administration
- Active Directory Administration
- User and Group Management
- Organizational Unit Design
- Virtualization
- File Server Administration
- Windows Networking
- DNS
- Access Control
- Troubleshooting
- Documentation

---

# Lessons Learned

This project reinforced the importance of hands-on learning. Building the environment from scratch required researching problems, troubleshooting configuration issues, and understanding how Windows Server components work together.

The experience improved my understanding of enterprise identity management, Windows administration, and system troubleshooting far more than simply watching tutorials.

---

# Future Improvements

- Configure Group Policy Objects (GPOs)
- Deploy DHCP services
- Add roaming profiles
- Configure folder redirection
- Implement Remote Desktop Services
- Deploy Windows clients automatically
- Integrate PowerShell automation
- Configure Windows Server Backup
- Expand the lab with additional domain controllers

---

# Repository Contents

```
README.md
Screenshots/
Documentation/
```

---

## Author

**Aysar Aljiryawee**

Cybersecurity Student

Focused on Windows administration, networking, Linux, virtualization, and cybersecurity.
