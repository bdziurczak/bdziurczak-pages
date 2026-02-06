---
title: "Project: VM Debian Server"
date: 2026-02-06
---
**Goal is to configure Debian Server in VM in a way that website hosted by nginx server is accessible in LAN on distinct IP address. I want VM to be treated like a different host. I will use VirtualBox as a supervisor.**
### [06-02-2026] Init
Today I set up VM(debserver0), it's netcard is in bridged mode, IP address of enp0s3 interface is statically set to address that is in scope of all LAN devices. Basically I can SSH into my VM from any device in LAN. 

**To look into**
When I connect via ssh i get message like
```bash
The authenticity of host 'xxx.xxx.xxx.xxx (xxx.xxx.xxx.xx)' can't be established.
EDXXXXX key fingerprint is SHA256: xxxxxxxxxxxxxxxxxxxxxx.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])?
```
I must dig into it