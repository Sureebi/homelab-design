# Homelab Network Topology

Public-safe network topology documentation for a personal homelab environment.

This project presents a high-level infrastructure map suitable for a GitHub README and portfolio. It focuses on architecture, roles, and service layout without exposing sensitive operational details such as public IP addresses, credentials, MAC addresses, exact port forwards, or raw device exports.

## Topology

![Homelab topology](assets/homelab-topology.png)

[View SVG version](assets/homelab-topology.svg)

## Architecture Summary

The homelab is organized around a small but practical home infrastructure stack:

- **MikroTik hAP ax3** as the network edge, router, firewall, and Wi-Fi gateway.
- **Home LAN / Wi-Fi** for trusted personal devices.
- **Homelab segment** for servers, virtualization, containers, and self-hosted services.
- **Raspberry Pi 5** as a lightweight services node for Docker workloads and dashboard tooling.
- **Dell OptiPlex 7060 Micro** as a compact virtualization host running Proxmox.
- **Application services** including media/photo management, dashboarding, reverse proxy, monitoring, game hosting, and admin tooling.

## What This Demonstrates

- Network architecture documentation
- Public-safe infrastructure design
- Home lab segmentation and service organization
- Linux server administration
- Docker-based self-hosting
- Proxmox virtualization
- Reverse proxy and service exposure planning
- Portfolio-focused technical communication

## Repository Structure

```text
homelab-design/
├── README.md
├── assets/
│   ├── homelab-topology.svg
│   ├── homelab-topology.png
│   └── topology-placeholder.svg
└── docs/
    ├── network-overview.md
    └── public-scope.md
```

## Public Scope

This repository is intentionally high level. It documents the shape of the infrastructure while keeping private implementation details out of the public repo.

See [docs/public-scope.md](docs/public-scope.md) for the public documentation boundaries.
