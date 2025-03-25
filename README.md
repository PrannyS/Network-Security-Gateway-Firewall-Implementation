# Network-Security-Gateway-Firewall-Implementation
![Status](https://img.shields.io/badge/Status-Completed-green)
![Static Badge](https://img.shields.io/badge/Tools-%20iptables%2C%20Netplan%2C%20bind9%20%20-%20blue)

## 📌 Overview 
This project involved configuring a Linux VM as a secure gateway for a Windows VM, implementing advanced network security controls using iptables and bind9. The goal was to understand key networking concepts such as routing, NAT, SSH, DNS, HTTPS, and firewalls while setting up security rules to control traffic and enhance protection.

---
## 📖 Table of Contents
- [Key Topics Covered](#key-topics-covered)  
- [Architecture Overview](#architecture-overview)    
- [Setup and Configuration](#setup and configuration)  
  - [Network Configuration](#0️⃣-network-configuration)  
  - [DNS Configuration](#1️⃣-dns-configuration)  
  - [Routing](#2️⃣-routing)  
  - [iptables](#3️⃣-iptables) 
  - [Advanced Firewall Rules](#4️⃣-advanced-firewall-rules) 
  - [Testing and Validation](#5️⃣-testing-and-validation)
- [Ethical Considerations](#ethical-considerations)  
- [Learning Outcomes](#learning-outcomes)  
- [Contact](#contact)  
- [Acknowledgements](#acknowledgements)

---

### Key Topics Covered
- Routing and NAT using iptables
- DNS configuration using bind9
- Firewall rules for selective traffic control
- Advanced traffic filtering, logging, and rate limiting

---

### Architecture Overview
The project created a secure network architecture with the following components:
***Linux VM:***Configured as a gateway with two network interfaces:
- Adapter 1: NAT interface for internet access
- Adapter 2: Internal network interface for communication with the Windows VM

***Windows VM*** – Connected to the Linux VM through an internal network, using the Linux VM as a gateway
### 0️⃣ Environment Setup

![alt text](image.png)