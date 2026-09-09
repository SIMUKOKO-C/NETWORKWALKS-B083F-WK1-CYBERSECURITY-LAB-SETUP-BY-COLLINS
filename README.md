# NETWORKWALKS-B082-WK1-CYBERSECURITY-LAB-SETUP
This is Cybersecurity Lab environment setup using  Oracle VirtualBox ,Kali Linux and And Network configuration
In this lab the purpose is to create a environment that is controlled with cybersecurity tools,  reconnaissance, vulnerability assessme,ntnetwork scanning, and other security-testing activities can be performed safely and repeatedly.
# NETWORKWALKS-B082-WK1-CYBERSECURITY-LAB-SETUP

## 🛡️ Cybersecurity Lab Setup

This project is about setting up my own **cybersecurity lab environment** using **Oracle VirtualBox, Kali Linux, Windows virtual machines, and a custom NAT Network**.

The main idea of this lab is to have a safe and controlled environment where I can practice cybersecurity skills such as **network scanning, reconnaissance, vulnerability assessment, penetration testing, and other ethical hacking activities** without affecting real systems.

> ⚠️ **Disclaimer:** This lab is for learning and authorized security testing only. Any testing should be done on systems that I own or have permission to test.

---

## 🎯 What I have Achieved
* Set up a working cybersecurity practice environment.
* Install and configure Oracle VirtualBox.
* Install Kali Linux as my main cybersecurity machine.
* Create a custom NAT Network for the virtual machines.
* Configure IP addresses for the VMs.
* Test communication between the machines.
* Take snapshots so I can easily restore the VMs when needed.
* Use the environment for ethical hacking and cybersecurity practice.
* Prepare the lab for future CTFs and practical cybersecurity exercises.
## 🌐 Network Setup

For this lab, I created a custom **NAT Network** in VirtualBox.

```text
Network: 10.0.0.0/24
Range:   10.0.0.2 - 10.0.0.99
```


These addresses can be changed depending on the configuration of the virtual machines.

---

# 🚀 Setting Up the Lab

## Phase 1: Basic Setup

### 1. Install WinRAR

I used **WinRAR** to extract the compressed virtual machine files before importing them into VirtualBox.

After downloading the required VM files, I extracted them using WinRAR and prepared them for use in VirtualBox.

**Tool used:** WinRAR

---

### 2. Install Oracle VirtualBox

Next, I installed **Oracle VirtualBox** on my computer.

VirtualBox is the software I used to create and run the virtual machines in this lab.

Official download:

https://virtualbox.org/wiki/Downloads

---

### 3. Create the NAT Network

Inside VirtualBox, I created a custom NAT Network.

```text
Network: 10.0.0.0/24
```

The NAT Network allows the virtual machines to communicate with each other while keeping the lab environment controlled.

---

### 4. Install Kali Linux

I downloaded and open the **Kali Linux virtual machine** into VirtualBox.

Kali Linux is the main machine I use for cybersecurity and ethical hacking practice.

Official download:

https://www.kali.org/get-kali/

---

### 5. Configure Kali Linux Networking

After installing Kali Linux, I connected its network adapter to the NAT Network.

The network configuration is based on:

```text
Network:       10.0.0.0/24
Subnet Mask:   255.255.255.0
IP Address:    8.8.8.8
```

To check the IP address in Kali Linux:

```bash
ip addr
```

or:

```bash
ip a
```

To test communication with another machine:

```bash
ping <target-ip>
```

---


### Check IP address

```bash
ip addr
```

### Check routing table

```bash
ip route
```

### Test connectivity

```bash
ping 10.0.0.1
```

Or test another VM:

```bash
ping <VM-IP>
```

These commands help me confirm that the network is working before starting any cybersecurity exercises.


---

# ✅ Lab Checklist

* [ ] Install WinRAR
* [ ] Extract the VM files
* [ ] Install Oracle VirtualBox
* [ ] Create NAT Network
* [ ] Configure `10.0.0.0/24`
* [ ] Import Kali Linux
* [ ] Configure Kali networking
* [ ] Check Kali IP address
* [ ] Install Windows VM
* [ ] Install Android VM (optional)
* [ ] Connect all VMs to the NAT Network
* [ ] Test connectivity using `ping`
* [ ] Create VM snapshots
* [ ] Test Internet connectivity
* [ ] Add screenshots and documentation

---

# 🧠 What I Learned

From this lab, I learned how to build a basic virtual cybersecurity environment from scratch.

I practiced:

* Setting up Oracle VirtualBox.
* Using WinRAR to extract VM files.
* Installing and managing virtual machines.
* Creating a NAT Network.
* Configuring IP addresses.
* Connecting different operating systems to the same virtual network.
* Testing network connectivity.
* Creating and using VM snapshots.
* Preparing a controlled environment for cybersecurity experiments.

---
  CHALLENGES I FACED
🩻when using the terminal use correct spellings
🩻its is also case sensitive (lower or uppercase where needed or it will not work)
---

# ⚠️ Ethical Use

This project is for **educational purposes and authorized cybersecurity testing**.

I should only test systems that I own or have permission to test.

I will not use the techniques from this lab against:

* Other people's computers
* Networks without permission
* Public systems
* Other people's accounts
* Organizations without authorization

The goal is to learn cybersecurity in a **safe and responsible way**.

---

# 📚 Reference

This lab setup was based on the **Practical Lab Environment Setup for Pentesting, Ethical Hacking & Cybersecurity** guide by **COLLINS L SIMUKOKO, Networkwalks Academy**.

---

## 👨‍💻 Project Information

**Project:** NETWORKWALKS-B082-WK1-CYBERSECURITY-LAB-SETUP
**Type:** Cybersecurity Lab
**Virtualization:** Oracle VirtualBox
**Main OS:** Kali Linux
**Network:** VirtualBox NAT Network
**Network Range:** `10.0.0.0/24`
**Archive Tool:** WinRAR

---

⭐ **Learning cybersecurity one lab at a time.**
