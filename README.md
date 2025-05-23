# -Network-Intrusion-Detection-Systems-SNORT

# Overview
This project is a practical walkthrough of setting up and using Snort, an open-source Network Intrusion Detection System , to detect and respond to suspicious activity on a network. The setup involves a two-machine environment.

# Tools used 

-Snort	Intrusion detection engine

-Nmap	Network scanning and testing

-Kali Linux	Attack simulation
-Ubuntu	Snort host / Detection system
-ifconfig	Interface discovery
-gedit	Config and rule editing

# What is Snort?
Snort is an opern sourece network intrusion detection and prevention systems that analyzes network traffic to identify malicious activites. 
-Detect attacks (port scans, brute force, malware0
-Log packets 
-Tigger alerts based on predefined rules 
-Used as a lightweight intrusion prevention system 

# How Snort Works

Snort captures packets on your network interface and analyzes them against a set of **rules**. If the traffic matches a rule, Snort logs the event and triggers an alert.

### Key Components:
- **Sniffer Mode**: Logs traffic to the screen.
- **Packet Logger Mode**: Logs packets to disk.
- **NIDS Mode**: Detects and alerts based on rules.

