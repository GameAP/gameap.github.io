---
title: GameAP Daemon Install
layout: default
lang: en
category: GameAP Daemon
order: 50
---


## Debian

It is actual for Debian Jessie and Debian Stretch.

## Add repositories

Download and add key:
```bash
wget -O - http://packages.gameap.ru/gameap-rep.gpg.key | apt-key add -
```

Add new repository:
```bash
echo "deb http://packages.gameap.ru/debian/ $(lsb_release -sc) main" > /etc/apt/sources.list.d/gameap.list
```

Update packages list and run install:
```bash
apt-get update
apt-get install gameap-daemon
```
