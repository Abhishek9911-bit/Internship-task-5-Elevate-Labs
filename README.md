# Internship-task-5-Elevate-Labs
 Capture live network packets and identify basic protocols and traffic types.
 Network Traffic Capture and Analysis Using Wireshark

## Project Overview
This project involves capturing and analyzing network traffic using Wireshark. The capture session aimed to generate diverse network traffic on a wireless interface and analyze it across multiple protocol layers to understand normal network behavior and security aspects.

## Setup and Configuration
- **Tool Used:** Wireshark version 4.x on Windows
- **Interface:** Wireless network adapter (Wi-Fi)
- **Capture Mode:** Promiscuous mode enabled to capture all traffic
- **Duration:** Approximately 1-2 minutes of active capture
- **Filters:** No initial capture filters to ensure comprehensive data collection

## Traffic Generation Methodology
Various activities were performed to generate network traffic including:
- Web browsing with multiple HTTP/HTTPS requests
- DNS queries for domain name resolution
- Background system updates and service communications
- Network service discovery protocols enabled

## Protocols Analyzed
### Transport Layer Protocols
- **TCP:** Dominant reliable transmission protocol with observed three-way handshake (SYN, SYN-ACK, ACK) and proper connection teardown
- **UDP:** Used primarily for DNS queries, multicast DNS (mDNS), and Simple Service Discovery Protocol (SSDP)

### Application Layer Protocols
- **HTTP/HTTPS:** Typical web browsing traffic, multiple GET requests, responses with status codes, and user-agent strings observed
- **DNS:** Extensive domain name resolution activities including Google, Microsoft, and CDN domains
- **TLS/SSL:** Secure encrypted communications with proper handshake and certificate validation, versions TLS 1.2 and 1.3 detected

## Network Traffic Statistics
- **Total Packets Captured:** 6,806 packets
- **Packet Size Range:** 54 to 1,514 bytes (standard Ethernet frames)
- **Average Packet Rate:** 60-70 packets/second
- **Protocols Identified:** 8 distinct protocols including TCP, UDP, HTTP/HTTPS, DNS, TLS/SSL

## Security Analysis
- All DNS queries resolved to legitimate domains
- TLS connections validated certificates properly
- No port scanning or reconnaissance detected
- HTTP requests targeted legitimate services only
- No suspicious or malicious activity observed during the capture period

## Technical Implementation Details
- Proper TCP header fields: ports, sequence numbers, flags, window size
- Correct IP header fields: IPv4 addresses, TTL, protocol field, checksums
- Employed display filters in Wireshark for targeted protocol analysis (e.g., tcp, http, dns)

## Skills Developed
- Network traffic capture configuration and execution
- Protocol identification and classification
- Traffic pattern and anomaly analysis
- Security protocol verification and network baseline establishment

## Professional Application
The exercise demonstrates essential cybersecurity competencies for:
- Incident response through traffic capture and forensic evidence
- Network security monitoring for abnormal behavior detection
- Vulnerability assessment by identifying insecure communications 

## Conclusion
This Wireshark analysis task successfully captured and analyzed diverse network traffic, verifying normal network behavior and security compliance while enhancing practical network analysis skills.

---

Prepared by Sankabathula Abhishek  
Cybersecurity Internship Task 5  
GD Goenka University, Gurugram
This README format highlights the key points and insights from the original report in a concise, structured manner suitable for GitHub or project documentation. Let me know if any section needs further customization or expansion.
