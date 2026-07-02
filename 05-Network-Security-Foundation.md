Network Security Foundation



A concise summary of essential Network+ security concepts, common attacks, device hardening, and traffic control.



\## Overview



Network security protects data, verifies users, limits access, segments networks, secures devices, and controls traffic using layered defenses.



\## Core Concepts



\* \*\*Data in Transit\*\*: Data moving across a network.



&#x20; \* Protection: HTTPS, TLS, VPN, IPsec.

\* \*\*Data at Rest\*\*: Data stored on devices or servers.



&#x20; \* Protection: encryption, permissions, access control.

\* \*\*Encryption\*\*: Makes data unreadable without the correct key.

\* \*\*PKI / Certificates\*\*: Verify digital identity and trust.

\* \*\*IAM\*\*: Manages user identity and access.

\* \*\*Least Privilege\*\*: Give users only required access.

\* \*\*RBAC\*\*: Assign permissions based on roles.



\## Authentication



Authentication verifies that users or devices are legitimate.



Key points:



\* \*\*Authentication\*\*: Proves identity.

\* \*\*Authorization\*\*: Defines allowed access.

\* \*\*Accounting\*\*: Logs activity.

\* \*\*MFA\*\*: Adds extra login protection.

\* \*\*SSO\*\*: One login for multiple services.



Common technologies:



\* RADIUS

\* LDAP

\* SAML

\* TACACS+

\* TOTP



\## Risk and Security Principles



Key terms:



\* \*\*Vulnerability\*\*: A system weakness.

\* \*\*Threat\*\*: A possible danger.

\* \*\*Exploit\*\*: A method used to attack a weakness.

\* \*\*Risk\*\*: The chance of loss or damage.



CIA Triad:



\* \*\*Confidentiality\*\*: Keep data private.

\* \*\*Integrity\*\*: Keep data accurate.

\* \*\*Availability\*\*: Keep systems accessible.



\## Compliance



Organizations must follow laws, standards, and policies.



Examples:



\* \*\*GDPR\*\*: Protects personal data.

\* \*\*PCI DSS\*\*: Protects payment card data.

\* \*\*Data Localization\*\*: Controls where data is stored.



Non-compliance can cause fines, legal issues, failed audits, and reputation damage.



\## Network Segmentation



Segmentation separates networks to reduce risk.



Common segments:



\* Staff

\* Servers

\* Guest

\* IoT

\* BYOD

\* Management

\* OT / SCADA / ICS



Common controls:



\* VLANs

\* ACLs

\* Firewall rules

\* NAC

\* Security policies



\## Common Attacks



\### DoS / DDoS



Makes services unavailable.



Defenses:



\* DDoS protection

\* CDN

\* Rate limiting

\* Firewall filtering

\* Monitoring



\### VLAN Hopping



Attempts to move between VLANs without permission.



Defenses:



\* Disable dynamic trunking

\* Use access ports for users

\* Limit allowed VLANs

\* Change native VLAN

\* Avoid VLAN 1 for users



\### MAC Flooding



Fills a switch MAC table with fake MAC addresses.



Defenses:



\* Port security

\* MAC address limits

\* Disable unused ports

\* 802.1X

\* Monitoring



\### ARP / DNS Poisoning



Manipulates address resolution.



Defenses:



\* Dynamic ARP Inspection

\* DHCP Snooping

\* DNSSEC

\* HTTPS/TLS validation

\* Trusted DNS servers



\## Rogue Services



Unauthorized services or devices inside a network.



Examples:



\* Rogue DHCP server

\* Rogue access point

\* Evil twin Wi-Fi



Defenses:



\* DHCP Snooping

\* WIDS / WIPS

\* 802.1X

\* NAC

\* Port security

\* User awareness



\## Social Engineering



Attacks that target people instead of systems.



Common types:



\* Phishing

\* Spear phishing

\* Whaling

\* Smishing

\* Vishing

\* Pretexting

\* Impersonation

\* Baiting

\* Tailgating

\* Shoulder surfing



Defenses:



\* Verify requests

\* Never share passwords or OTPs

\* Check links and sender addresses

\* Use MFA

\* Report suspicious activity



\## Malware



Malicious software used to steal, damage, spy, or gain access.



Common types:



\* Virus

\* Worm

\* Ransomware

\* Trojan

\* Rootkit

\* Keylogger

\* Spyware

\* Adware

\* Logic bomb

\* Backdoor

\* Botnet



Defenses:



\* Patch systems

\* Use EDR or antivirus

\* Keep secure backups

\* Avoid suspicious files and links

\* Apply least privilege

\* Enable MFA



\## Device Security



Best practices:



\* Close unused ports

\* Disable unnecessary services

\* Change default credentials

\* Use strong passwords

\* Disable unused switch ports

\* Enable port security

\* Limit MAC addresses per port

\* Use NAC and 802.1X

\* Manage certificates and keys



> MAC filtering can help, but it should not be the only control because MAC addresses can be spoofed.



\## Security Rules



Security rules define allowed and blocked traffic.



Common controls:



\* ACLs

\* Firewall rules

\* Inbound rules

\* Outbound rules

\* Content filtering

\* DMZ

\* Security zones



Best practices:



\* Allow only required traffic

\* Deny unknown traffic by default

\* Place specific rules above general rules

\* Separate public servers from internal systems

\* Review rules regularly

\* Log important traffic



Example:



```text

ALLOW Internet -> Web Server HTTPS

DENY  Internet -> Database Server

DENY  Guest Network -> Internal Network

ALLOW Admin Network -> Switch Management

DENY  Unknown Traffic -> Any

```



\## Key Takeaways



\* Protect data in transit and at rest.

\* Verify users and devices.

\* Use least privilege.

\* Segment networks.

\* Harden devices.

\* Monitor suspicious activity.

\* Enforce clear security rules.

\* Train users against social engineering.



\## Conclusion



Network security is a layered process that combines encryption, authentication, segmentation, device hardening, monitoring, compliance, and traffic control.

