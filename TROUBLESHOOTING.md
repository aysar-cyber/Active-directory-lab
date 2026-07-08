# Troubleshooting Log

This document records issues encountered while building the Active Directory home lab and the steps taken to resolve them.

---

## Issue 1: Active Directory Installation Prerequisite Failure

### Problem
The Active Directory Domain Services installation failed during the promotion process because prerequisite checks were not satisfied.

### Resolution
- Reviewed the prerequisite warnings.
- Corrected the server configuration.
- Re-ran the promotion wizard.
- Successfully promoted the server to a Domain Controller.

---

## Issue 2: Windows Server Networking

### Problem
The Windows Server virtual machine was not receiving proper network connectivity.

### Resolution
- Verified the virtual NIC configuration in KVM.
- Installed the required VirtIO network drivers.
- Confirmed network connectivity using `ipconfig` and `ping`.

---

## Issue 3: File Share Permissions

### Problem
Users were unable to access shared folders due to permission configuration issues.

### Resolution
- Reviewed NTFS permissions.
- Compared NTFS permissions with SMB share permissions.
- Corrected administrator access.
- Retested access from the Windows client.

---

## Issue 4: Windows 11 Domain Connectivity

### Problem
The Windows 11 client experienced issues accessing domain resources.

### Resolution
- Verified domain membership.
- Confirmed DNS resolution.
- Tested connectivity using both hostname and IP address.
- Continued troubleshooting share authentication.

---

## Lessons Learned

- Share permissions and NTFS permissions work together. Both must allow access.
- Active Directory security groups simplify permission management.
- DNS is essential for Active Directory environments.
- Troubleshooting should follow a structured process: identify the problem, isolate the cause, test a solution, and verify the fix.
