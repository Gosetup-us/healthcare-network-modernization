# Proxmox VE Deployment

## Overview

This document describes the deployment and configuration of the Proxmox VE virtualization platform used as the foundation for the SF Rehab infrastructure modernization project.

The virtualization host provides a centralized platform for running infrastructure services, including the UniFi OS Server and future network management applications.

---

## Hardware Platform

| Component | Description |
|----------|-------------|
| Platform | Dell OptiPlex 3040 |
| Hypervisor | Proxmox VE |
| Deployment Type | Bare Metal |
| Purpose | Infrastructure Virtualization |

---

## Deployment Objectives

- Build a dedicated virtualization host
- Provide an isolated environment for infrastructure services
- Simplify backup and recovery
- Enable future expansion
- Support enterprise-style change management

---

## Initial Virtual Machine

A dedicated Ubuntu Server virtual machine was deployed to host the UniFi OS Server.

The VM was configured with:

- Ubuntu Server 24.04 LTS
- VirtIO storage
- VirtIO network adapter
- Dynamic IP address (DHCP)
- LVM storage layout

The virtual machine serves as the primary platform for UniFi Network management.

---

## Storage Expansion

During deployment of the UniFi OS Server, additional storage capacity became necessary.

The virtual disk was expanded within Proxmox VE.

Following the virtual disk expansion, the guest operating system storage was extended by resizing the LVM physical volume, logical volume, and filesystem.

Storage expansion was verified using:

- lsblk
- pvs
- vgs
- lvs
- df -h

---

## Validation

The deployment was considered successful after confirming:

- Proxmox VE operational
- Ubuntu Server virtual machine running
- Expanded storage available
- Filesystem successfully resized
- VM ready for UniFi OS deployment

---

## Status

Completed.
