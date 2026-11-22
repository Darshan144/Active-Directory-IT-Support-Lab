# Active-Directory-IT-Support-Lab

## Project Overview

This project documents the design, deployment, administration, and troubleshooting of a simulated corporate IT environment for a fictional company called **TechCorp**.

The lab is built using Oracle VirtualBox and Windows Server 2022, with the goal of developing practical skills relevant to Level 1 IT Support, Service Desk, Desktop Support, and Junior Systems Administration roles.

The project is being developed in stages, with technical documentation, screenshots, and troubleshooting records added as each milestone is completed.

## Lab Environment

| Component | Technology |
|---|---|
| Virtualization | Oracle VirtualBox |
| Host Operating System | Windows 11 |
| Server Operating System | Windows Server 2022 Evaluation |
| Server Hostname | TECHCORP-DC01 |
| Server Memory | 4 GB |
| Virtual Processors | 2 |
| Virtual Storage | 50 GB |
| Initial Network | NAT |

## Project Progress

### Phase 1: Windows Server Deployment — Completed

- Created a Windows Server 2022 virtual machine.
- Configured virtual hardware and initial networking.
- Installed Windows Server 2022 with Desktop Experience.
- Configured local Administrator access.
- Renamed the server to `TECHCORP-DC01`.
- Investigated and resolved a VirtualBox boot failure sufficiently to complete installation.

### Phase 2: Network Configuration — Planned

- Configure an isolated virtual network.
- Assign a static IP address.
- Validate network connectivity.

### Phase 3: Active Directory & DNS — Planned

- Install Active Directory Domain Services.
- Configure DNS.
- Create a new Active Directory domain.
- Create and manage employee user accounts and security groups.

### Phase 4: IT Support Administration — Planned

- Join a Windows client to the domain.
- Practise password resets and account administration.
- Configure Group Policy.
- Manage shared folders and NTFS permissions.
- Simulate and document common IT support tickets.

## Troubleshooting Experience

During the initial deployment, VirtualBox encountered a critical error:

`VINF_EM_TRIPLE_FAULT`

I investigated the VirtualBox diagnostic log, reviewed virtual machine boot settings, adjusted the boot configuration, and successfully completed the Windows Server installation.

The exact underlying cause of the triple fault was not conclusively established.

## Skills Demonstrated

- Windows Server installation and initial configuration
- Virtual machine deployment and resource allocation
- VirtualBox networking and boot configuration
- Operating system installation troubleshooting
- Diagnostic log analysis
- Technical documentation

## Project Status

**In Progress — Phase 1 completed**

This repository will be updated as additional lab configurations, screenshots, and troubleshooting scenarios are completed.

*This is an independently developed educational home lab, not a production corporate environment.*
