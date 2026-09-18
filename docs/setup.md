# Phase 1 — VirtualBox & VM Setup
## Objective

Create the first Linux virtual machine for NetOpsLab and install Ubuntu Server.
The first VM will eventually act as the Linux gateway for the NetOpsLab environment.

---

## 1. Lab Environment
### Host Machine

The physical computer runs:
- Windows
- Oracle VM VirtualBox
VirtualBox is used to create and run Linux virtual machines locally.

### Virtual Machine

| Setting | Configuration |
|---|---|
| VM Name | `NetOpsLab-Gateway` |
| Operating System | Ubuntu Server |
| CPU | 2 cores |
| RAM | 2 GB |
| Disk | 25 GB |
| Initial Network | NAT |
| Linux User | `netops` |

---

## 2. Why VirtualBox
VirtualBox allows us to run Linux servers as virtual machines on the Windows host.
This lets us build a complete networking lab without requiring multiple physical servers.

**Physical Computer - Windows - VirtualBox - NetOpsLab-Gateway Ubuntu Server**

## 3. VM Creation
A virtual machine named `NetOpsLab-Gateway` was created in VirtualBox.

### Hardware Configuration
- **CPU:** 2 cores
- **RAM:** 2 GB
- **Disk:** 25 GB

The disk uses VirtualBox's dynamically allocated virtual disk.

---

## 4. Ubuntu Server Installation
Ubuntu Server was installed inside the virtual machine.
During installation, a Linux user was created:

- **Username:** `netops`
The server can now be accessed through the Ubuntu terminal.

---

## 5. VirtualBox Networking
The initial network configuration uses:
- **Adapter 1:** NAT

NAT is being used initially because the first objective is simply to provide the VM with Internet connectivity