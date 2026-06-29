IP Addressing Foundation



\## Overview



This document summarizes the core IP addressing concepts from \*\*Binary Math\*\* to \*\*IPv6\*\*. These topics are fundamental for networking, cybersecurity, cloud, and IT operations.



\## Learning Flow



```text

Binary Math → IPv4 → Subnet Mask → Subnetting → SDN/VXLAN/Zero Trust/IaC → IPv6

```



\## Key Concepts



\### 1. Binary Math



Computers read data as binary: `0` and `1`.



```text

192 = 11000000

10  = 00001010

```



Binary is the base of IP addressing and subnetting.



\### 2. IPv4 Addressing



IPv4 identifies devices in a network.



```text

Example: 192.168.1.10

```



Key points:



```text

IPv4 = 32-bit address

4 octets

Each octet = 0–255

DHCP = automatic IP assignment

APIPA = 169.254.x.x when DHCP fails

```



Private IP ranges:



```text

10.0.0.0/8

172.16.0.0/12

192.168.0.0/16

```



\### 3. Classful Addressing



Old IPv4 addressing method based on address classes.



```text

Class A: 1–126      /8

Class B: 128–191    /16

Class C: 192–223    /24

Class D: 224–239    Multicast

Class E: 240–255    Reserved

```



```text

127.0.0.1 = loopback / local device

```



\### 4. Subnet Mask



Subnet masks separate an IP address into:



```text

Network portion

Host portion

```



Common masks:



```text

/8  = 255.0.0.0

/16 = 255.255.0.0

/24 = 255.255.255.0

```



\### 5. IPv4 Subnetting



Subnetting divides a large network into smaller networks.



Benefits:



```text

Better IP organization

Reduced broadcast traffic

Improved security

Efficient IP usage

```



Formula:



```text

Usable hosts = 2^host bits - 2

Host bits = 32 - CIDR

```



Example:



```text

/26 = 64 total IPs

/26 = 62 usable hosts

```



\### 6. Magic Number



Used to calculate subnet ranges quickly.



```text

Magic Number = 256 - interesting octet

```



Example:



```text

/26 = 255.255.255.192

256 - 192 = 64

Ranges: 0, 64, 128, 192

```



\### 7. Seven Second Subnetting



Quick subnetting reference:



```text

/24 = 254 hosts

/25 = 126 hosts

/26 = 62 hosts

/27 = 30 hosts

/28 = 14 hosts

/29 = 6 hosts

/30 = 2 hosts

```



Magic numbers:



```text

/25 = 128

/26 = 64

/27 = 32

/28 = 16

/29 = 8

/30 = 4

```



\### 8. SDN



Software Defined Networking centralizes network control.



```text

Traditional = configure devices one by one

SDN         = manage network from a central controller

```



Benefits:



```text

Automation

Centralized policy

Better monitoring

Flexible deployment

```



\### 9. VXLAN



VXLAN is used for large-scale network virtualization.



```text

VLAN  = limited scale

VXLAN = scalable virtual networking

```



Key terms:



```text

VNI      = VXLAN ID

VTEP     = VXLAN tunnel endpoint

Overlay  = virtual network

Underlay = physical network

```



\### 10. Zero Trust



Zero Trust security principle:



```text

Never trust automatically. Always verify.

```



Core concepts:



```text

Verify explicitly

Least privilege

Assume breach

```



\### 11. Infrastructure as Code



IaC manages infrastructure using code.



```text

Manual = click and configure

IaC    = write code and deploy automatically

```



Common tools:



```text

Terraform

Ansible

CloudFormation

Azure Bicep

Pulumi

```



Security note:



```text

Never store passwords, API keys, or secrets in public repositories.

```



\### 12. IPv6 Addressing



IPv6 is the modern replacement for IPv4 limitations.



```text

IPv4 = 32-bit

IPv6 = 128-bit

```



Example:



```text

2001:db8::1

```



Key points:



```text

Uses hexadecimal

Separated by colons

:: can shorten continuous zeros

:: can only be used once

IPv6 does not use broadcast

```



Common IPv6 types:



```text

Global Unicast = public IPv6

Link-local     = fe80::

Unique Local   = fd00::

Multicast      = ff00::

Loopback       = ::1

Unspecified    = ::

```



\## Quick Summary



```text

IP Address  = device address

Subnet Mask = network boundary

Subnetting  = dividing a network into smaller networks

Gateway     = exit point to another network

SDN         = centralized network control

VXLAN       = scalable VLAN for cloud/data centers

Zero Trust  = verify every access request

IaC         = infrastructure managed by code

IPv6        = next-generation IP addressing

```



\## Final Notes



IP addressing is a core networking skill.

IPv4 and subnetting help organize networks.

Modern networking uses SDN, VXLAN, Zero Trust, and IaC.

IPv6 provides a larger and more scalable address space.

