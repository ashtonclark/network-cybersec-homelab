# Network & Cybersec Homelab
My hands-on networking, cybersecurity, and systems admin homelab using Proxmox VE, Ubuntu Server, and Kali Linux.

The project focuses on designing, deploying, securing, and troubleshooting virtualized network infrastructure. My long-term goal is to expand the environment into a cloud security lab incorporating network segmentation, firewall management, centralized monitoring, automation, and AI-assisted threat analysis.

# Goals
- Build and administer a virtualized Linux server environment.
- Develop practical networking skills involving IP addressing, switching, routing, and network segmentation.
- Configure and troubleshoot network interfaces and firewall policies.
- Analyze network traffic and vulnerabilites using Wireshark and Nmap.
- Implement isolated environments for cybersecurity testing.
- Explan into cloud networking and AI incorporation.
# Hardware 
Lenovo Thinkcentre M720q
- CPU: i5-8400T, 6 core
- RAM: 32GB (upgraded by myself from 8GB)
- Storage: 256 GB SSD
- Hypervisor: Proxmox VE
- Administration: Lenovo Thinkpad

Planning on incorporating a physical switch, seperate router, and possibly firewall to expand practical knowledge.

# VM Infrastructure
Current Environment:

| VM | OS | vCPU | RAM | Purpose |
|--- | --- | --- | --- | --- |
| Ubuntu Server | Ubuntu Server 24.04 LTS | 2 | 4 GB | Linux Administration |
| Kali Linux | Kali Linux XFCE | 2 | 6 GB | Netowrk Security Testing |
| Ubuntu Target | Ubuntu Server 24.04 LTS | 2 | 2 GB | Isolated Security Testing | 

# Network Architecture

Environment currently uses two Proxmox Linus bridges:

- vmbr0: Home LAN connectivity and infrastructure management.
- vmbr1: Private virtual network used for security testing.

Kali Linux is dual-homed, with interfaces connected to both bridges. Ubuntu Target connects only to the private virtual bridge and has no default gateway.

Additional network isolation controls are planned.

# Network Topology

<img width="603" height="452" alt="Screenshot 2026-11-13 at 11 34 05 PM" src="https://github.com/user-attachments/assets/c8b317f7-1bf9-43fb-8983-d05035c35edd" />

# Technologies & Skills 

Virtualization & Infrastructure

- Proxmox VE
- QEMU/KVM
- Linux virtual networking

Networking

- TCP/IP and IPv4 subnetting
- Static IP configuration
- Linux bridges
- SSH
- NetworkManager and Netplan

Cybersecurity

- Nmap
- Wireshark
- UFW
- TCP packet analysis
- Network Reconnaissance

# Future Development

- Virtual routing and firewall segmentation
- VLAN configuration and inter-VLAN routing
- Centralized logging and security monitoring
- Hybrid cloud networking using AWS
- AI-powered network intrusion detection
- Security automation and incident analysis
