📋 Overview
This lab is designed for security researchers, students, and professionals to practice offensive and defensive techniques without risking production systems. The environment is fully isolated from your host network by default. 

Core Components:

Attacker: Kali Linux – Equipped with standard penetration testing tools (Nmap, Metasploit, Burp Suite).
Target Server: Ubuntu Linux – Configurable server hosting vulnerable services (SSH, Web, FTP).
Victim Endpoint: Android OS (via Android-x86 or Genymotion) – For mobile security testing and ADB exploitation. 
Hypervisor: VirtualBox – Manages virtualization and network isolation.

Kali Linux
Debian-derived Linux distribution
Wikipedia
kali.org
Kali Linux 2.0 wordmark
🏗️ Architecture & Network Topology
The lab utilizes a Host-Only Network adapter in VirtualBox to ensure total isolation. Traffic between VMs never leaves your physical host.

Network Configuration
VM Role	OS	Recommended IP (Host-Only)	Adapter Settings
Attacker	Kali Linux	192.168.56.101	Host-Only Adapter
Server	Ubuntu Linux	192.168.56.102	Host-Only Adapter
Victim	Android OS	192.168.56.103	Host-Only Adapter

Note: A secondary NAT adapter can be temporarily enabled for updates but should be disabled during active exercises to maintain isolation.


VirtualBox host-only network configuration guide

View all
📦 Prerequisites
Before cloning this repository, ensure your host machine meets the following requirements:

Hypervisor: VirtualBox (Latest version recommended) & Extension Pack.
Hardware:
RAM: Minimum 8GB (16GB recommended for smooth operation).
CPU: 4+ Cores with Virtualization Technology (VT-x/AMD-V) enabled in BIOS.
Storage: At least 50GB of free space.
ISO Images:
Kali Linux (Installer or Pre-built VM).
Ubuntu Server LTS.
Android-x86 ISO or Genymotion image
