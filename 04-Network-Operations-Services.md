Network Operations \& Services



A concise Network+ summary covering documentation, monitoring, recovery, IP services, DNS, VPN, and remote access.



\## Key Objectives



\* Document network infrastructure

\* Monitor network health and security

\* Manage device configurations

\* Prepare for failures and recovery

\* Automate IP and name resolution services

\* Secure remote connectivity



\---



\## 1. Network Documentation



Documentation helps teams understand and troubleshoot the network faster.



\*\*Includes:\*\*



\* Network maps

\* Physical and logical diagrams

\* Asset inventory

\* IP address records

\* Cable documentation

\* Site survey reports



\*\*Goal:\*\* reduce downtime and avoid guesswork.



\---



\## 2. Life Cycle Management



Network devices must be managed from purchase to disposal.



```text

Procure → Deploy → Maintain → Upgrade → Retire → Dispose

```



\*\*Goal:\*\* avoid outdated hardware, unsupported software, and security risks.



\---



\## 3. Configuration Management



Configuration management keeps network settings controlled and recoverable.



\*\*Key practices:\*\*



\* Maintain baseline configs

\* Back up production configs

\* Track changes

\* Prevent configuration drift

\* Roll back failed changes



\*\*Goal:\*\* make every change documented and recoverable.



\---



\## 4. SNMP



SNMP monitors network devices remotely.



| Component | Purpose                  |

| --------- | ------------------------ |

| Manager   | Monitoring platform      |

| Agent     | Runs on device           |

| MIB/OID   | Defines monitored values |

| Polling   | Manager requests data    |

| Trap      | Device sends alert       |



```text

UDP 161 = Polling

UDP 162 = Traps

```



\*\*Best practice:\*\* use SNMPv3.



\---



\## 5. Logs and Monitoring



Logs and monitoring provide visibility into network activity.



\*\*Tools:\*\*



\* Syslog

\* SIEM

\* Alerts

\* Flow data

\* Packet capture

\* Protocol analysis



\*\*Goal:\*\* detect issues before they become major incidents.



\---



\## 6. Network Solutions



Network tools help discover and troubleshoot infrastructure.



\*\*Examples:\*\*



\* Network discovery

\* LLDP / CDP

\* Ping scan

\* Port scan

\* Traffic analysis

\* Performance monitoring

\* Availability monitoring

\* Configuration monitoring



\*\*Goal:\*\* troubleshoot using data, not assumptions.



\---



\## 7. Disaster Recovery



Disaster recovery prepares systems for major failures.



| Term | Meaning                       |

| ---- | ----------------------------- |

| DRP  | Recovery plan                 |

| RTO  | Maximum downtime              |

| RPO  | Maximum data loss             |

| MTTR | Average repair time           |

| MTBF | Average time between failures |



\*\*Recovery sites:\*\*



\* Hot site: fastest, expensive

\* Warm site: partially ready

\* Cold site: slowest, cheaper



\*\*Goal:\*\* restore services quickly and safely.



\---



\## 8. Network Redundancy



Redundancy prevents one failure from taking down the network.



\*\*Concepts:\*\*



\* Single Point of Failure

\* High Availability

\* Failover

\* Failback

\* Load balancing

\* Redundant links

\* Redundant power



\*\*Goal:\*\* improve uptime and reliability.



\---



\## 9. DHCP



DHCP automatically assigns IP settings to devices.



```text

Discover → Offer → Request → ACK

```



\*\*Key terms:\*\*



\* Scope / Pool

\* Lease

\* Reservation

\* Exclusion

\* Relay / Helper



```text

UDP 67 = Server

UDP 68 = Client

```



\*\*Goal:\*\* reduce manual IP configuration.



\---



\## 10. IPv6 and SLAAC



IPv6 provides scalable addressing for modern networks.



\*\*Key concepts:\*\*



\* 128-bit addressing

\* Hexadecimal format

\* Link-local: `fe80::`

\* Global unicast

\* SLAAC

\* Router Advertisement

\* DAD

\* NDP

\* DHCPv6



\*\*Goal:\*\* support large and future-ready networks.



\---



\## 11. DNS



DNS translates domain names into IP addresses.



```text

google.com → IP address

```



\*\*Key concepts:\*\*



\* Forward lookup

\* Reverse lookup

\* Resolver

\* Authoritative DNS

\* Cache

\* TTL

\* Hosts file

\* DNSSEC / DoT / DoH



\*\*Goal:\*\* make network resources easy to access by name.



\---



\## 12. DNS Records



DNS records define domain behavior.



| Record | Purpose               |

| ------ | --------------------- |

| A      | IPv4 address          |

| AAAA   | IPv6 address          |

| CNAME  | Alias                 |

| MX     | Mail server           |

| NS     | Name server           |

| SOA    | Zone authority        |

| TXT    | Text verification     |

| SPF    | Allowed email senders |

| DKIM   | Email signature       |

| DMARC  | Email policy          |

| SRV    | Service location      |

| PTR    | Reverse DNS           |



\*\*Goal:\*\* support websites, email, security, and services.



\---



\## 13. Time Protocols



Time synchronization is required for logs, authentication, certificates, and investigations.



\*\*Key terms:\*\*



\* NTP

\* NTP Server

\* NTP Client

\* Stratum

\* Time Drift

\* NTS

\* PTP



```text

UDP 123 = NTP

```



\*\*Goal:\*\* keep timestamps accurate and reliable.



\---



\## 14. VPNs



VPNs create encrypted tunnels over public networks.



\*\*Types:\*\*



\* Client-to-site

\* Site-to-site

\* Clientless VPN

\* Full tunnel

\* Split tunnel



\*\*Goal:\*\* secure remote users and branch connectivity.



\---



\## 15. Remote Access



Remote access allows admins to manage systems from anywhere.



\*\*Methods:\*\*



\* SSH

\* Console access

\* In-band management

\* Out-of-band management

\* Jump box

\* Bastion host

\* API integration

\* RDP / GUI



\*\*Best practices:\*\*



\* Disable Telnet

\* Use SSH

\* Enable MFA

\* Restrict admin access

\* Use VPN or jump boxes

\* Log all admin activity

\* Patch remote services



\---



\## Final Summary



Professional network operations require infrastructure that is:



```text

Documented

Monitored

Secure

Redundant

Recoverable

Scalable

Remotely manageable

```



These practices help build reliable, secure, and production-ready networks.

