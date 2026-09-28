# Network Overview

This document contains the public architecture summary used for the topology diagram.

## Inventory

### Router / Edge

The network edge is represented by a MikroTik hAP ax3. In this public view, it is described only by role:

- Internet edge
- Router
- Firewall
- Wi-Fi gateway
- Traffic boundary between home devices and homelab systems

### Network Segments

The public topology groups the environment into high-level zones:

- Home LAN
- Wi-Fi clients
- Homelab systems
- Public-facing service boundary, shown only as an architectural concept

### Physical Hosts

- Raspberry Pi 5: lightweight always-on services node
- Dell OptiPlex 7060 Micro: compact virtualization host for Proxmox workloads

### Virtual Machines / Containers

Virtualization and container workloads are represented by category instead of exact internal inventory:

- Proxmox virtual machines
- Linux lab VMs
- Docker containers
- Management and admin tools

### Services

The public service map includes high-level service categories:

- Dashboard
- Docker / Portainer management
- Photo and media service
- Reverse proxy
- Monitoring
- Game server
- Lab and security VMs

## Diagram Notes

The diagram shows only public-safe relationships:

- Internet edge to router/firewall
- Router/firewall to confirmed LAN or VLAN segments
- Physical hosts connected to their confirmed segments
- VMs, containers, and services under their confirmed hosts
- Public-facing services as a general boundary only

No raw exports, exact WAN details, credentials, or sensitive operational information should be included.
