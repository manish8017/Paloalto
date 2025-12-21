🔐 Cisco ASA Multi-Zone Firewall Configuration Lab

This repository contains a Cisco ASA Firewall lab designed to demonstrate multi-zone security architecture with proper access control and traffic flow enforcement.

🏗️ Network Topology Overview

The lab is built using the following security zones:

Inside Zone (Security Level 100)

Network: 10.11.11.0/24

Trusted internal LAN

DMZ Zone (Security Level 50)

Network: 192.168.30.0/24

Hosts public-facing services

Outside Zone (Security Level 0)

Network: 172.16.3.0/24

Untrusted external network

Management Network

Network: 192.168.0.0/24

Dedicated ASA management access

⚙️ Key Configurations

Named Extended ACLs applied using access-group

Interface-based traffic filtering

Security-level based traffic behavior

ICMP testing and packet verification

Management plane isolation

Static routing between zones

🔍 Traffic Flow Behavior
Source	Destination	Result
Inside → Outside	Allowed (Stateful)	
Inside → DMZ	Allowed	
DMZ → Inside	Denied (ACL Controlled)	
Outside → Inside	Denied (ACL Controlled)	
Management → ASA	Allowed	
Outside → Management	Denied	
🧪 Verification & Troubleshooting

packet-tracer for flow simulation

show access-list

show capture (ICMP / ARP)

show arp

🎯 Learning Objectives

Understand ASA security levels

Configure and apply named ACLs

Control inter-zone communication

Perform real-time traffic troubleshooting

Implement secure management access

🖼️ Topology Diagram

Refer to the network diagram included in this repository.

🚀 Tools Used

Cisco ASA (ASAv)

Cisco Routers & Switches

EVE-NG / GNS3 (Lab Environment)

📚 Use Case

This lab is ideal for:

CCNA / CCNP Security preparation

Firewall fundamentals

Network security practice

🏷️ Tags

cisco asa firewall network-security ccna ccnp lab

✅ Note

This is a practice lab created for learning and testing purposes.
