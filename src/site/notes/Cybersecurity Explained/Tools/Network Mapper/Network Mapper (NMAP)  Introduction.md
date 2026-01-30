---
{"dg-publish":true,"permalink":"/cybersecurity-explained/tools/network-mapper/network-mapper-nmap-introduction/","tags":["NMAP","CyberSec","Networking","HackTheBox"]}
---









[[Network Mapper (NMAP)  Introduction \|Network Mapper (NMAP)  Introduction ]]
[[Cybersecurity Explained/Tools/Network Mapper/Network Mapper  Port State\|Network Mapper  Port State]]
[[Cybersecurity Explained/Tools/Network Mapper/Network Mapper  Scanning Active Ports\|Network Mapper  Scanning Active Ports]]
[[Cybersecurity Explained/Tools/Network Mapper/Firewalls & Prevention Systems/Firewalls & Prevention Systems\|Firewalls & Prevention Systems]]
[[Cybersecurity Explained/Networking/TCPIP  Internet Control Message Protocol \|TCPIP  Internet Control Message Protocol ]]

# Introduction
Network Mapper (NMAP), a specialized software designed to intercept available packets on a given network. Able to identify Operating Systems, Version Information, and crucial vulnerabilities relating to the host. Packets received are processed and scanned, which can determine packet information and other crucial network information. 

## Use Case's 
- Audit Security Aspects on a Network. 
- Simulate Penetration Tests
- Check Firewall & IDS/IPS Behavior.
- Network Mapping (Packet Analytics)


# Enumeration 
Network Enumeration is a systematic reconnaissance process that establishes active connections to target systems, to discover open ports and crucial network services, including User Accounts, Passwords, Name Servers, and file services. 

The goal of enumeration is to gather the **largest** amount of information possible out of a network, including network structure and protocols, crucial to network vulnerability assessment. 


## Target System
Accessing a Target System is possible with possible with external tools and software.
Information that we analyze and collect, are used to gather crucial information and statistics on the network structure, including mapping out vulnerabilities. 

## Banner Grabbing
NMAP (Network Mapper), identifies packets using banners collected through the scanning process. If the process is unable to identify version information, NMAP will attempt to gather additional information using a process known as <mark style="background: #D2B3FFA6;">Signature Based Matching System.</mark> 

After a **successful** Three-Message Handshake, the server often sends a `Banner,` used for identification, which allows the client which service it's working with. 


