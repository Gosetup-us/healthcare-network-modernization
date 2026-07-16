# Project Roadmap

## Purpose

This document defines the planned development stages for the SF Rehab healthcare network infrastructure. The roadmap is updated as the project progresses and serves as a reference for future implementation.

---

# Phase 1 – Foundation ✅ Completed

- [x] Install Proxmox VE
- [x] Create Ubuntu Server VM
- [x] Install UniFi OS Server
- [x] Deploy UniFi Network Controller
- [x] Migrate all UniFi devices
- [x] Configure static IP address (192.168.10.126)
- [x] Verify Wi-Fi operation
- [x] Verify wired network performance (900+ Mbps)
- [x] Create VM Snapshot
- [x] Create Full VM Backup

---

# Phase 2 – Infrastructure Services

## 1. Homepage Dashboard
**Status:** Planned

**Purpose**
- Central dashboard for the entire infrastructure.
- Quick access to Proxmox, UniFi, Omada, printers, documentation and future services.

---

## 2. Vaultwarden (Bitwarden)
**Status:** Planned

**Purpose**
- Secure password management.
- Store credentials for infrastructure devices and services.

---

## 3. Uptime Kuma
**Status:** Planned

**Purpose**
- Monitor:
- Internet connection
- Proxmox Server
- UniFi Controller
- Switches
- Access Points
- Printers

**Expected Result**
- Immediate notification when a device or service goes offline.

---

## 4. WireGuard VPN
**Status:** Planned

**Purpose**
- Secure remote access to the hospital network.

---

## 5. Paperless-ngx
**Status:** Planned

**Purpose**
- Store documentation, manuals, scanned documents and network diagrams.

---

## 6. Grafana + Prometheus
**Status:** Planned

**Purpose**
- Infrastructure monitoring and performance dashboards.

---

## 7. Pi-hole
**Status:** Planned

**Purpose**
- Network-wide DNS filtering.
- Ad and tracker blocking.

---

## 8. Dozzle
**Status:** Planned

**Purpose**
- Docker container log viewer.

---

## 9. Home Assistant
**Status:** Future

**Purpose**
- Automation testing.
- Smart building integration.

---

# Phase 3 – Network Core Modernization

## Protectli + OPNsense

**Status:** Planned

Tasks:

- Replace TP-Link Omada ER707-M2
- Configure VLANs
- Configure Firewall
- Configure IDS/IPS
- Configure VPN
- Configure Dual WAN
- Configure Security Policies

---

# Phase 4 – Backup Infrastructure

## Proxmox Backup Server

**Status:** Future

Purpose:

- Scheduled VM backups
- Long-term backup retention
- Disaster recovery
- Centralized backup management

---

# Current Project Status

**Current Phase:** Phase 1 Completed ✅

The virtualization platform is fully operational.

The UniFi Controller has been successfully migrated to Proxmox.

All network devices are online.

The environment has been protected with both Snapshot and Full Backup.

The next milestone is deploying the Infrastructure Services. 
