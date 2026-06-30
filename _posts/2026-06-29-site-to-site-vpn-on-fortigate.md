---
layout: post
title: "Site-to-Site VPN on FortiGate"
date: 2026-06-29
categories: fortinet vpn
image_class: img-forti
image_text: "FORTINET"
read_time: "10 min read"
views: "31"
---

A site-to-site VPN connects two networks securely through IPsec.

## Basic checklist

1. Verify both public IP addresses.
2. Match Phase 1 proposal.
3. Match Phase 2 selectors.
4. Add firewall policies.
5. Add static routes.

## Useful commands

```bash
get vpn ipsec tunnel summary
diagnose vpn tunnel list
diagnose debug application ike -1
diagnose debug enable
```
