# Troubleshooting Case Study: VirtualBox Boot Failure

## 1. Incident Summary

**Environment:** Oracle VirtualBox 7.1.12, Windows Server 2022 Evaluation

**Affected VM:** TECHCORP-DC01

**Issue:** Windows Server installation failed during the initial virtual machine deployment.

**Error:** `VINF_EM_TRIPLE_FAULT` (VirtualBox Guru Meditation)

**Status:** Resolved for the lab deployment. Exact root cause not conclusively established.

## 2. Problem Description

While deploying Windows Server 2022 in Oracle VirtualBox, the virtual machine encountered a critical failure during the boot and installation process.

VirtualBox displayed a Guru Meditation error, preventing the operating system installation from continuing.

## 3. Troubleshooting and Investigation

The following troubleshooting activities were performed:

1. Examined the VirtualBox diagnostic log (`VBox.log`).
2. Identified the `VINF_EM_TRIPLE_FAULT` error.
3. Reviewed virtual machine boot settings.
4. Disabled floppy boot.
5. Enabled EFI firmware and left Secure Boot disabled.
6. Retried booting from the Windows Server 2022 installation ISO.
7. Removed the partitions created during the unsuccessful installation attempt.
8. Performed a clean Windows Server installation using the unallocated virtual disk space.

## 4. Resolution

Following the configuration changes, the virtual machine successfully booted from the installation media.

Windows Server 2022 Standard Evaluation with Desktop Experience was installed successfully.

The local Administrator account was configured, and the server was renamed to `TECHCORP-DC01`.

Although the installation succeeded after these changes, the exact cause of the original triple fault was not conclusively isolated.

## 5. Verification

Successful deployment was verified by:

- Logging in to Windows Server 2022.
- Opening Server Manager.
- Confirming the server hostname as `TECHCORP-DC01`.
- Confirming that the operating system was running in VirtualBox.

Supporting screenshots are available in the `screenshots/day-01/` directory.

## 6. Lessons Learned

This incident reinforced the importance of:

- Reviewing diagnostic logs instead of relying only on error messages.
- Checking virtual machine firmware and boot configuration.
- Understanding the difference between BIOS and EFI boot environments.
- Verifying the result after troubleshooting.
- Recording technical problems and resolutions for future reference.

## 7. Relevance to IT Support

The troubleshooting process reflects practical skills used in IT Support and Service Desk environments, including incident investigation, log analysis, system configuration, problem resolution and technical documentation.
