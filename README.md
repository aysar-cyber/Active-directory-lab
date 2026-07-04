# Active-directory-lab
This project documents the design, configuration, deployment, and administration of a Window Active Directory enviorment hosted on KVM/QEMU virtualization platform. The objective for this project is to develop stong technical experience with enterprise Windows infrastructure while strengthening systems administration, networking, virtualization, and troubleshooting skills.

Rather than following a tutorial start to finish, this lab was built by solving real deployment and configuration encountered troughout the entire setup process.

##Objectives
- Deploy Windows server as an Active DIrectory Domain Controller
- Configure Dns and networking for an enterprise enviorment
- Create and manage Active DIrectory Domain
- Join Windows client machines to the Domain
- Develop troubleshooting skills for common user issues
- Document every stage of deployment

##Technologies Used
Operating systems
- Windows server 2025
- Windows 11
- Arch Linux (Host)
- Ubuntu server

Virtualization
- KVM
- QEMU
- libvirt
- virt-manager

 Windows Services
- Active Directory Domain Services (AD DS)
- DNS
- Group Policy
- Active DIrectory Users and COmputers

Networking
- NAT networking
- DHCP
- Static IPV4 Config
- DNS Resolution
- Virtual Bridges (virbr0)

##LAB ARCHITECTURE
Arch Linux Host
│
├── KVM/QEMU
│
├── Windows Server 2025
│      ├── Active Directory
│      ├── DNS
│      └── Domain Controller (DC01)
│
└── Windows 11 Client
       └── Joined to homelab.local

Skills Demonstrated
- Windows Server Administration
- Active Directory Deployment
- Linux system Administration
- Virtualization
- Network configuration
- Network Configuration
- DNS
- DHCP
- Windows Troubleshooting
- Powershell
- Enterprise Authentication
- Technical Documentation

Challenges Encountered
During this project I experienced and resolved several infrastructure isues including:
- DHCP failures resulting in APIPA (192.254.X.X) addressing
- libvirt networking configuration issues
- Windows server driver installation
- Active directory deployment troubleshooting
- Server Manager Configuration problems
Detailed write-ups for each issue are available in TROUBLESHOOTING.md.

#Future Improvements
- Create organizational Units
- Create domain users and groups
- Join Windows 11 workstation to the domain
- Configure Group Policy Objects
- Implement file shares and NTFS permissions
- Deploy Splunk or Wazuh
- Generate security events for SOC detection practice
- Integrate Kali Linux for attack simulation
