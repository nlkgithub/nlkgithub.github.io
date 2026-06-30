---
layout: post
title: "Ubuntu Server Hardening Checklist"
date: 2026-06-27
categories: linux security
image_class: img-linux
image_text: "LINUX"
read_time: "6 min read"
views: "16"
---

Basic hardening steps for Ubuntu servers.

## Checklist

```bash
sudo apt update && sudo apt upgrade -y
sudo ufw enable
sudo ufw allow ssh
sudo systemctl enable unattended-upgrades
```

Also disable password SSH login and use SSH keys where possible.
