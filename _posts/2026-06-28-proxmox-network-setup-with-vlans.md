---
layout: post
title: "Proxmox Network Setup with VLANs"
date: 2026-06-28
categories: proxmox vlan
image_class: img-prox
image_text: "PROXMOX"
read_time: "7 min read"
views: "18"
---

Proxmox can use Linux bridges to connect virtual machines to VLAN networks.

## Example bridge

```bash
auto vmbr0
iface vmbr0 inet manual
    bridge-ports eno1
    bridge-stp off
    bridge-fd 0
    bridge-vlan-aware yes
```

Use VLAN tags on the VM network adapter.
