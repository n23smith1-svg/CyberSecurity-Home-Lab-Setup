# CyberSecurity-Home-Lab-Setup
A personal cybersecurity home lab built with Oracle VirtualBox, Windows 11, and Kali Linux security workstations. The virtual cybersecurity lab provides a controlled environment for hands-on cybersecurity training, including system administration, network security, vulnerability assessment, penetration testing, incident response, and security engineering.
## Project Overview
To create a foundation for hands-on learning, I built a virtualized lab environment using Oracle VirtualBox.
The current lab consists of:

- 🪟 Windows virtual machine — Endpoint
- 🐉 Kali Linux virtual machine — Security/Analyst workstation
- 📦 Oracle VirtualBox — Virtualization platform
- 🌐 Virtual network — Communication between the virtual machines

## Objectives
The main objectives of this project were:

- Build a virtualized cybersecurity laboratory.
- Configure Windows as a monitored endpoint.
- Configure Kali Linux as a security testing/analysis machine.
- Configure networking between the virtual machines.
- Verify communication between the systems.
- Explore Windows security logging.
- Create a foundation for future SOC detection and investigation exercises
  
## Lab Architecture
**Figure 1 — Architecture of the SOC home lab.**

```text
                         HOST MACHINE
                              │
                       Oracle VirtualBox
                              │
                ┌─────────────┴─────────────┐
                │                           │
                ▼                           ▼
        ┌───────────────┐           ┌───────────────┐
        │   Windows VM  │           │  Kali Linux   │
        │               │           │      VM       │
        │   Endpoint    │◄─────────►│   Analyst /   │
        │               │  Virtual  │ Security Lab  │
        └───────────────┘  Network  └───────────────┘
```

---
.
## Lab Enviroment

| Component | Purpose |
|---|---|
| Oracle VirtualBox | Virtualization platform |
| Windows VM | Endpoint / future monitored system |
| Kali Linux VM | Security testing and analysis |
| Virtual Network | Communication between VMs |

---
## Hardware & Software
| Component | Configuration |
|---|---|
| Host Operating System | Windows 11 |
| Host RAM | 8 GB |
| Host CPU | 11th Gen Intel Core i5-1155G7 |
| Host Storage | 170 GB |
| Hypervisor | Oracle VirtualBox |
| Kali Linux | 2026.1|
| Windows | Windows 11 (64-bit) |
| Network Type | NAT |

## Installing Oracle VirtualBox
The First step was to successfully install and setup Oracle VirtualBox, which provides the Virtualization environment required to run multiple operating systems on the host machine,
Leading to the following steps, to create separate virtual machines for Windows 11 and Kali Linux
<img width="958" height="539" alt="image" src="https://github.com/user-attachments/assets/5c1e6b98-e1ec-4183-a69f-a30d3ea7d8ea" />

## Virtual Machines
### Kali Linux
**Purpose:** Security testing and analysis workstation
- CPU: 2 processors
- RAM: 2048 MB
- Storage: 15.23 GB
- Network Adapter: NAT Intel PRO/1000 MT Desktop (82540EM)
- IP Address: 10.0.2.15

See: `documentation/02-kali-linux-setup.md`
<img width="959" height="530" alt="image" src="https://github.com/user-attachments/assets/610f25d9-d33c-4e59-b77d-f3e98d4346a1" />

### Windows

**Purpose:** Endpoint used for security testing, logging, and analysis.

- CPU: 2 processors
- RAM: 2048 MB
- Storage: 19.85 GB
- Network Adapter: NAT Intel PRO/1000 MT Desktop (82540EM)
- IP Address: 10.0.2.2

See: `documentation/03-windows-vm-setup.md`
<img width="956" height="522" alt="image" src="https://github.com/user-attachments/assets/36e5d29a-8c98-4804-9ed4-054a2e5145f6" />
<img width="531" height="448" alt="image" src="https://github.com/user-attachments/assets/7a5f775e-f62e-4a61-ae87-e24f6054c99f" />

## Network Configuration

- The network mode selected.
- Why you selected it.
- How the VMs receive IP addresses.
- How the VMs communicate.
- How you verified connectivity.

See: `documentation/04-network-configuration.md`

