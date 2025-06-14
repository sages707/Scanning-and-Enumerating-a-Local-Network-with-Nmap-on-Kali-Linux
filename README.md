# Scanning-and-Enumerating-a-Local-Network-with-Nmap-on-Kali-Linux

This project demonstrates how to perform network scanning and enumeration using Nmap on Kali Linux. It covers discovering active hosts, identifying open ports and services, and fingerprinting operating systems on a local network.

# Project Goals

- Learn how to use Nmap for network reconnaissance
- Understand different types of Nmap scans
- Enumerate services and detect OS and device types
- Develop a basic understanding of local network topologies

# Environment & Tools
- Base OS: Kali Linux 2023.x (Debian-based)
- Virtualization: VMware Workstation / VirtualBox (if applicable)
- Network Setup: Local Area Network (Wi-Fi or Ethernet)
- Main Tool: Nmap 7.94

# Installation

Nmap is preinstalled within Kali Linux. To verify the installation use: 
sudo apt-get update && sudo apt-get install nmap

# Process

Scan Number 1: Basic Network Scan
Command: nmap 192.168.231.0/24 (List of active devices with IP and Port)

Expected Output:<img width="690" alt="Regular Nmap" src="https://github.com/user-attachments/assets/96a381f2-02e8-485a-ba66-ccb842889a99" />

Scan Number 2: Scanning for a specific port
Command: nmap -p 80 192.168.231.0/24 (List of devices with specific port ie. 80)

Expected Output:<img width="589" alt="Nmap With Port" src="https://github.com/user-attachments/assets/2caedca5-fef3-4257-994c-b6f0d54be8f0" />

