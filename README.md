# Network Administration Final Lab Report - GNS3 Project

**Student:** Hussein Reslan (ID: 1122037)  
**Course:** SECU316 System and Network Administration  
**Date:** May 15, 2025
---

## Project Overview

This lab project demonstrates the deployment, configuration, and hardening of a simulated enterprise network using GNS3 with Windows Server and Ubuntu Server virtual machines. The setup includes Active Directory, DHCP failover, secure web and SSH services, automated backups, SNMP monitoring, and network security testing.

---

## Network Topology

- Cisco Router  
- Layer 2 Switch  
- Windows Server (192.168.1.10)  
- Secondary Windows Server (192.168.1.20)  
- Ubuntu Server (192.168.3.10)  
- Windows 10 Client(s) (DHCP clients in 192.168.2.x subnet)  

---

## Software & Tools Used

- GNS3 (latest)  
- Windows Server 2022  
- Ubuntu Server 22.04 LTS  
- Windows 10 Client  
- Wireshark  
- Putty/SSH Client  

---

## Configuration Highlights

### Windows Server

- Active Directory Domain Services configured and promoted to domain controller.  
- DHCP Server configured with failover and reservations.  
- Group Policy Objects implemented for security (password policy, account lockout, USB block).  
- SNMP monitoring set up with secure community strings.  
- Automated backups scheduled to network shares.

### Ubuntu Server

- Apache Web Server installed and secured with HTTPS and ModSecurity.  
- SSH hardened with key-based authentication and password disabled.  
- UFW firewall enabled with restricted ports and optional geo-blocking.  
- SNMP monitoring configured.  
- Automated backups scripted and scheduled, storing backups on Windows Server share.

---

## Testing & Monitoring

- DHCP failover tested by shutting down primary DHCP and renewing IP on clients.  
- SNMP polling confirmed from management station.  
- Wireshark captures used for network traffic analysis.  
- Logs monitored via Windows Event Viewer and Linux syslogs.

---

## Conclusion

The project achieved a secure, functional network environment demonstrating key skills in Windows and Linux server administration, network security, and troubleshooting within a simulated enterprise context.

---

## How to Use

Clone or download this repository to review the configuration steps and scripts. Use this as a reference or template for similar network lab setups or enterprise environment simulations.

---

## License

© 2025 Hussein Reslan. All rights reserved.

