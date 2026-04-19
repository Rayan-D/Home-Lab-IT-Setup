# Home IT Lab Environment

## Overview
This project is a simple IT lab set up using VirtualBox. The goal was to learn and practice basic Linux system administration, networking, and troubleshooting in a virtual environment.

---

## Setup
- Host OS: Windows
- Virtualization software: VirtualBox
- Guest OS: Ubuntu Desktop
- Network: Default NAT configuration

---

## System Setup
Installed Ubuntu and updated system packages:
sudo apt update
sudo apt upgrade -y

---

## User Management
Created a new user and gave sudo permissions:
sudo adduser labuser
sudo usermod -aG sudo labuser

---

## SSH Remote Access
Installed SSH server and enabled it:
sudo apt install openssh-server -y
sudo systemctl start ssh
sudo systemctl enable ssh

Connected using:
ssh labuser@<IP_ADDRESS>

---

## Networking Basics
Checked network configuration:
ip a

Tested connectivity:
ping google.com

Key notes:
- lo = local loopback
- enp... = main network interface

---

## Troubleshooting Practice
Simulated SSH failure and fixed it:
sudo systemctl stop ssh
sudo systemctl start ssh

Observed and resolved "connection refused" errors.

---

## System Monitoring
top
df -h
free -h

---

## What I Learned
- Linux command line basics
- User and permission management
- SSH setup and remote access
- Networking fundamentals
- Basic troubleshooting techniques

---

## Notes
- Done entirely in a VirtualBox virtual machine
- No cloud or external hardware used
- Focus was on Linux system administration basics