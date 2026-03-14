Subnetting Basics

Objective: Understand IP addresses, subnet masks, and how to divide networks into subnets.

**Core Concepts
**
IPv4 Address: 32 bits divided into 4 octets (e.g., 192.168.1.10)

Subnet Mask: Determines which part of the IP is the network and which part is for hosts.

CIDR Notation: /24 means 24 bits are used for the network.

Example:

IP: 192.168.1.10/24
Subnet Mask: 255.255.255.0
Network bits: 24
Host bits: 8
Usable hosts: 2^8 - 2 = 254

**Borrowing Bits
**
Subnetting is borrowing host bits to create more networks.

Original /24 → 1 network, 254 hosts

Borrow 1 bit → /25 → 2 networks, 126 hosts each

Borrow 2 bits → /26 → 4 networks, 62 hosts each

Pattern: each borrowed bit halves the number of hosts and doubles the networks.

**The Block Size Trick (Engineer Shortcut)
**
Subtract the last octet of the subnet mask from 256 → block size

Count by block size to find subnets

Identify which subnet an IP belongs to

Example: /26

Subnet Mask: 255.255.255.192
Block size: 256 - 192 = 64

Subnets:
192.168.1.0 – 192.168.1.63
192.168.1.64 – 192.168.1.127
192.168.1.128 – 192.168.1.191
192.168.1.192 – 192.168.1.255

**Exercises Solved
**
/27, IP 192.168.1.77 → subnet 192.168.1.64

/26, IP 192.168.1.150 → subnet 192.168.1.128
