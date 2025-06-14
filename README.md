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

*Scan Number 1: Basic Network Scan*
Command: nmap 192.168.231.0/24 (List of active devices with IP and Port) *Note you should use your own IP here, use command: ip a in order to obtain the IP*

Expected Output:

<img width="690" alt="Regular Nmap" src="https://github.com/user-attachments/assets/96a381f2-02e8-485a-ba66-ccb842889a99" />

*Scan Number 2: Scanning for a specific port*
Command: nmap -p 80 192.168.231.0/24 (List of devices with specific port ie. 80)

Expected Output:

<img width="589" alt="Nmap With Port" src="https://github.com/user-attachments/assets/2caedca5-fef3-4257-994c-b6f0d54be8f0" />

*Scan Number 3: Service Version Detection*
Command: nmap -sV 192.168.231.0/24 (Lists all of the ports with their service and version details)

Expected Output:

<img width="1357" alt="Nmap with sV" src="https://github.com/user-attachments/assets/c694a08e-86e1-438e-9ab2-9b16977eff65" />

*Scan Number 4: Operation System Detection*
Command: sudo nmap -O 192.168.231.0/24 (Lists the operating systems of the listed networks)

Expected Output:

<img width="839" alt="Nmap with -O" src="https://github.com/user-attachments/assets/8136a767-2de1-42b2-a2b0-4142e946eb1e" />

*Scan Number 5: Aggressive Scan*
Command: sudo nmap -A 192.168.231.0/24 (Lists everything, including OS, version, scripts and traceroute)

Expected Output: 

<img width="841" alt="Nmap with -A P3" src="https://github.com/user-attachments/assets/b69c1040-4c7f-4290-94f6-822214ba268c" />
<img width="1349" alt="Nmap with -A P2" src="https://github.com/user-attachments/assets/631a8a4f-35af-49ff-b17b-925e4c9b66b1" />
<img width="579" alt="Nmap with -A P1" src="https://github.com/user-attachments/assets/45b2c89a-f6bb-4d16-90a4-ae33c9076068" />




