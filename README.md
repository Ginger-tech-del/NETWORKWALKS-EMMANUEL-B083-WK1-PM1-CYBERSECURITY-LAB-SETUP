About

Isolated virtual lab built with virtualBox and Kali Linux for cybersecurity testing and penetration testing practice

NETWORKWALKS WEEK 1: CYBERSECURITY LAB SETUP

1. Project Overview

This project documents the setup of a cybersecurity testing environment using Oracle VirtualBox and Kali Linux. The lab provides an isolated environment for learning networking, cybersecurity fundamentals and ethical penetration testing.

The setup follows the Networkwalks Week 1 Cybersecurity Lab Setup instructions.

2. Project Objectives

- Install and configure Oracle VirtualBox.
- Set up Kali Linux as the testing machine.
- Configure a NAT Network for virtual machine connectivity.
- Assign Kali Linux a static IP address.
- Establish internet connectivity.
- Configure shared folders between the host and virtual machine.
- Enable shared clipboard and drag-and-drop functionality.
- Verify the network configuration and document the process.

3. Lab Architecture

The lab consists of a Windows host machine running Oracle VirtualBox, with Kali Linux operating as the virtual machine.

Architecture:

Windows Host Machine
↓
Oracle VirtualBox
↓
NAT Network
↓
Kali Linux Virtual Machine
↓
Internet Connectivity

4. Lab Configuration

Component| Configuration
Virtualization software| Oracle VirtualBox
Testing operating system| Kali Linux
Network mode| NAT Network
Network subnet| 10.0.0.0/24
Kali Linux IP address| 10.0.0.2/24
Default gateway| 10.0.0.1
DNS server| 8.8.8.8
Future VM IP range| 10.0.0.3–10.0.0.99
Shared folder| Host Downloads folder
Shared clipboard| Bidirectional
Drag and drop| Bidirectional

5. Implementation Procedure

Step 1: Virtualization Setup

Enabled hardware virtualization in the computer's BIOS/UEFI settings to allow VirtualBox to run virtual machines.

Step 2: VirtualBox Installation

Installed Oracle VirtualBox and prepared the environment for running Kali Linux.

Step 3: Kali Linux Setup

Created and launched the Kali Linux virtual machine in VirtualBox.

Step 4: NAT Network Configuration

Created a NAT Network using the assigned subnet of 10.0.0.0/24.

Step 5: Static IP Configuration

Configured Kali Linux with the assigned static IP address, default gateway and DNS settings.

Step 6: Shared Folder Configuration

Configured the host Downloads folder as a shared folder to allow file exchange between Windows and Kali Linux.

Step 7: Clipboard and Drag-and-Drop

Enabled bidirectional shared clipboard and drag-and-drop functionality in the virtual machine settings.

6. Network Verification

The following commands are useful for verifying the network configuration:

Check IP configuration

ip -4 addr

Check default gateway

ip route

Test gateway connectivity

ping -c 4 10.0.0.1

Test internet connectivity

ping -c 4 8.8.8.8

Test DNS resolution

nslookup google.com

Check Nmap installation

nmap --version

7. Problems Encountered and Solutions

BIOS Virtualization Restriction

Problem: VirtualBox initially encountered a BIOS virtualization restriction.

Solution: Accessed the computer's BIOS/UEFI configuration and enabled hardware virtualization before launching the virtual machine again.

Network Configuration

Configured the NAT Network and assigned the required static IP settings to Kali Linux.

8. Learning Outcomes

Through this exercise, I gained practical experience in:

- Virtual machine installation and management.
- Linux operating system configuration.
- Virtual networking and NAT.
- Static IP addressing and DNS configuration.
- Host-to-guest file sharing.
- Basic network troubleshooting.
- Cybersecurity lab preparation.

9. Tools and Technologies

- Oracle VirtualBox
- Kali Linux
- Windows
- NAT Networking
- Nmap
- Linux Terminal

10. Ethical Considerations

This laboratory environment is intended strictly for educational purposes, authorized security testing and responsible cybersecurity learning. All testing activities should be conducted on systems for which permission has been granted.

11. Project Information

Program: Networkwalks Cybersecurity Training
Week: Week 1
Project: Cybersecurity Lab Setup
Author: Networkwalks Participant
Repository: NETWORKWALKS-EMMANUEL-B083-WK1-PM1-CYBERSECURITY-LAB-SETUP
