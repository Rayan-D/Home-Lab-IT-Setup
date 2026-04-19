# Home IT Lab Environment

## Overview
This project was built using a VirtualBox environment to practice basic Linux system administration, networking, and troubleshooting. The goal was to get familiar with common system tasks used in IT support and junior system administration roles.

---

## Setup
- Host OS: Windows
- Virtualization software: VirtualBox
- Guest OS: Ubuntu Desktop
- Network mode: NAT (default VirtualBox configuration)

---

## System Setup
Installed Ubuntu in a virtual machine and updated system packages.

sudo apt update
sudo apt upgrade -y

---

## User Management
Created a new user account and granted administrative privileges.

sudo adduser labuser
sudo usermod -aG sudo labuser

---

## SSH Remote Access
Installed and configured SSH to allow remote access to the system.

sudo apt install openssh-server -y
sudo systemctl start ssh
sudo systemctl enable ssh

Connected locally using:
ssh labuser@<IP_ADDRESS>

---

## Networking Basics
Checked network configuration and tested connectivity.

ip a
ping google.com

Identified key interfaces:
- loopback (lo)
- main network interface (enp...)

---

## Troubleshooting Practice
Practiced basic service troubleshooting by stopping and restarting the SSH service to simulate a connection issue.

sudo systemctl stop ssh
sudo systemctl start ssh

Observed and resolved a “connection refused” error during testing.

---

## What I Learned
- Basic Linux command line usage
- User account and permission management
- SSH setup and remote access
- Basic networking concepts (IP addresses, interfaces, connectivity)
- Simple troubleshooting of system services

---

## Notes
All work was completed inside a VirtualBox virtual machine. No external services or hardware were used.