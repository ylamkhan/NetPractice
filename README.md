# NetPractice

![1337 School](https://img.shields.io/badge/1337-School-000000?style=flat&logo=1337&logoColor=white)
![Network](https://img.shields.io/badge/Network-TCP%2FIP-blue)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📋 Table of Contents

- [About](#about)
- [Learning Objectives](#learning-objectives)
- [Key Concepts](#key-concepts)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Exercises Overview](#exercises-overview)
- [Essential Networking Knowledge](#essential-networking-knowledge)
- [Common Mistakes](#common-mistakes)
- [Tips and Strategies](#tips-and-strategies)
- [Resources](#resources)
- [Contributing](#contributing)

## 🎯 About

NetPractice is a 1337 School project designed to teach fundamental networking concepts through practical exercises. Students learn to configure small-scale networks by solving 10 different networking scenarios, each requiring proper IP address configuration, subnet masks, and routing tables.

The project focuses on understanding:
- TCP/IP protocol suite
- Subnetting and CIDR notation  
- Network routing
- IP address classes and private ranges
- Network troubleshooting

## 🎓 Learning Objectives

By completing NetPractice, you will:

- ✅ Understand IP addressing and subnetting
- ✅ Configure network interfaces and routing tables
- ✅ Apply CIDR notation effectively
- ✅ Troubleshoot basic network connectivity issues
- ✅ Grasp fundamental concepts of network topology
- ✅ Learn to work with private and public IP ranges

## 🔑 Key Concepts

### IP Addresses
- **IPv4 Structure**: 32-bit addresses written in dotted decimal notation
- **Classes**: A (1.0.0.0-126.255.255.255), B (128.0.0.0-191.255.255.255), C (192.0.0.0-223.255.255.255)
- **Private Ranges**: 
  - Class A: 10.0.0.0/8
  - Class B: 172.16.0.0/12
  - Class C: 192.168.0.0/16

### Subnet Masks
- **Purpose**: Define network and host portions of IP addresses
- **CIDR Notation**: /24 = 255.255.255.0, /16 = 255.255.0.0, etc.
- **Subnetting**: Dividing networks into smaller subnetworks

### Routing
- **Default Gateway**: Router interface for external network access
- **Routing Tables**: Define paths for packet forwarding
- **Static vs Dynamic**: Manual configuration vs automatic updates

## 📁 Project Structure

```
NetPractice/
├── README.md
├── level1/
├── level2/
├── level3/
├── level4/
├── level5/
├── level6/
├── level7/
├── level8/
├── level9/
└── level10/
```

## 🚀 Getting Started

1. **Download the project files** from the 1337 intranet
2. **Extract** the archive to your workspace
3. **Open** each level in your browser
4. **Configure** the network parameters for each scenario
5. **Test** your configuration using the "Check again" button
6. **Export** your solutions when complete

### Prerequisites

- Basic understanding of binary and hexadecimal systems
- Familiarity with command line networking tools
- Web browser (for the interactive exercises)

## 📚 Exercises Overview

### Level 1-3: Basic IP Configuration
- Simple point-to-point connections
- Basic subnet mask application
- Interface IP assignment

### Level 4-6: Intermediate Routing
- Multiple network segments
- Router configuration
- Default gateway setup

### Level 7-10: Advanced Scenarios
- Complex network topologies
- Multiple routing tables
- Subnet optimization
- VLSM (Variable Length Subnet Masking)

## 🌐 Essential Networking Knowledge

### Subnetting Quick Reference
--------------------------------------------
| CIDR | Subnet Mask    | Hosts| Networks  |
|------|----------------|-------|----------|
| /24  | 255.255.255.0  | 254   | 256      |
| /25  | 255.255.255.128| 126   | 512      |
| /26  | 255.255.255.192| 62    | 1024     |
| /27  | 255.255.255.224| 30    | 2048     |
| /28  | 255.255.255.240| 14    | 4096     |
| /29  | 255.255.255.248| 6     | 8192     |
| /30  | 255.255.255.252| 2     | 16384    |
--------------------------------------------

### Binary to Decimal Conversion

```
128 | 64 | 32 | 16 | 8 | 4 | 2 | 1
----+----+----+----+---+---+---+---
 1  | 1  | 1  | 1  | 1 | 1 | 1 | 0  = 254
 1  | 1  | 1  | 1  | 1 | 1 | 0  | 0  = 252
 1  | 1  | 1  | 1  | 1 | 0  | 0  | 0  = 248
```

## ❌ Common Mistakes

### IP Address Conflicts
- **Issue**: Same IP assigned to multiple interfaces
- **Solution**: Ensure unique IPs within each network segment

### Incorrect Subnet Masks
- **Issue**: Mismatched subnet masks prevent communication
- **Solution**: All devices in same network need identical subnet masks

### Wrong Network Ranges
- **Issue**: Using broadcast or network addresses for hosts
- **Solution**: Remember first and last IPs in range are reserved

### Routing Loops
- **Issue**: Circular routing paths cause packet loss
- **Solution**: Verify routing tables for logical paths

## 💡 Tips and Strategies

### Planning Your Network
1. **Identify required subnets** and their size requirements
2. **Calculate appropriate subnet masks** using CIDR notation
3. **Assign IP ranges** avoiding overlaps
4. **Configure routing** from specific to general routes

### Troubleshooting Steps
1. **Check IP conflicts** within network segments
2. **Verify subnet masks** match across devices
3. **Validate routing tables** for complete paths
4. **Test connectivity** using the built-in checker

### Memory Aids
- **Private IP ranges**: 10.x.x.x, 172.16-31.x.x, 192.168.x.x
- **Subnet calculation**: 2^n hosts, where n = host bits
- **CIDR shortcuts**: /24 = 256 hosts, /25 = 128 hosts, etc.

## 📖 Resources

### Official Documentation
- [RFC 791 - Internet Protocol](https://tools.ietf.org/html/rfc791)
- [RFC 950 - Internet Standard Subnetting Procedure](https://tools.ietf.org/html/rfc950)
- [RFC 1918 - Private Internet Address Allocation](https://tools.ietf.org/html/rfc1918)

### Learning Materials
- [Subnet Calculator](https://www.subnet-calculator.com/)
- [Visual Subnet Calculator](https://www.davidc.net/sites/default/subnets/subnets.html)
- [Cisco Networking Basics](https://www.netacad.com/courses/networking)

### Command Line Tools
```bash
# IP configuration
ip addr show
ifconfig

# Routing table
ip route show
route -n

# Network testing
ping <ip_address>
traceroute <ip_address>
```

## 🤝 Contributing

This is an educational project for 1337 School. While direct collaboration on solutions isn't permitted, you can:

- Share general networking knowledge and explanations
- Help debug conceptual misunderstandings
- Provide resources and learning materials
- Discuss theoretical aspects of networking

## 📝 Notes

- Each level must be completed sequentially
- Solutions are auto-graded by the system
- Export your configurations before closing the browser
- Practice with real networking tools to reinforce learning

## 🎉 Completion

Successfully completing NetPractice demonstrates solid understanding of:
- IP addressing and subnetting fundamentals
- Basic network routing principles  
- Network configuration and troubleshooting
- Essential skills for system administration

---

**Good luck with your networking journey!** 🌐

> "The best way to learn networking is by doing. Each subnet you configure and every route you establish builds your understanding of how the internet works."
