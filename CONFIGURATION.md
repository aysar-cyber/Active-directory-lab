# Configuration Documentation

## Lab Overview

This document outlines the configuration of the Active Directory home lab environment.

---

# Host Machine

Operating System:
- Arch Linux

Virtualization:
- KVM/QEMU
- Virt-Manager

---

# Virtual Machines

## Domain Controller

Operating System:
- Windows Server 2022

Roles Installed:
- Active Directory Domain Services (AD DS)
- DNS Server
- File Server

Hostname:
- DC01

Domain:
- HOMELAB.local

---

## Client Machine

Operating System:
- Windows 11

Domain Joined:
- HOMELAB.local

Purpose:
- Domain authentication
- User login testing
- File share testing

---

# Active Directory Configuration

## Organizational Units

- Users
- Groups
- Computers
- Servers
- HR
- IT

---

# Security Groups

- HR_Users
- IT_Users

Purpose:
- Role-based access control
- Department permission management

---

# User Accounts

Example users were created for testing authentication and file permissions.

Each user was assigned to the appropriate department security group.

---

# DNS

DNS is hosted on the Domain Controller.

Clients obtain name resolution through the domain controller.

---

# File Server

Shared Root:

C:\Shares

Folders:

- HR
- IT
- Finance

Permissions are managed using Active Directory Security Groups.

---

# Networking

Virtualization Platform:
- KVM

Network Type:
- NAT

Client and server communicate over the same virtual network.

---

# Administrative Tools Used

- Server Manager
- Active Directory Users and Computers
- DNS Manager
- File Explorer
- Command Prompt
- PowerShell

---

# Validation

The following functionality has been verified:

- Domain Controller operational
- Active Directory accessible
- Organizational Units created
- Users created
- Security Groups configured
- Windows 11 successfully joined to the domain
- Shared folders created
