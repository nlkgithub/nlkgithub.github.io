---
layout: post
title: "Cisco VLAN Configuration Guide for Beginners"
date: 2026-06-30
categories: cisco vlan
image_class: img-vlan
image_text: "VLAN 10 / 20 / 30"
read_time: "8 min read"
views: "24"
---

This guide explains basic VLAN configuration on Cisco switches.

## Create VLANs

```bash
configure terminal
vlan 10
 name USERS
vlan 20
 name SERVERS
exit
```

## Configure access port

```bash
interface g0/1
 switchport mode access
 switchport access vlan 10
 spanning-tree portfast
```

## Verify

```bash
show vlan brief
show interfaces trunk
```
