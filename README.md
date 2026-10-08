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
| Windows | [Version] |
| Network Type | [NAT / Host-Only / Internal / NAT Network] |
