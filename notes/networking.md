MODULE 1 – Networking Basics and Security Layers
1. Networking Essentials
Computer Networks:
A set of interconnected devices that share data and resources.

IP Address:

A unique number that identifies devices on a network.

IPv4: 32-bit (e.g., 192.168.1.1).

IPv6: 128-bit (e.g., 2001:db8::1).

2. DNS – Domain Name System (Full Cycle)
Purpose: DNS converts human-readable domain names into IP addresses that computers understand.

DNS Resolution Steps (Full Cycle):

User Enters URL – e.g., www.google.com in a browser.

Check Browser Cache: The browser first checks if it already knows the IP address of www.google.com.

Check OS Cache (Host File): If not in browser cache, the OS checks the local host file and DNS cache.

Query Recursive Resolver: The request goes to the ISP’s DNS resolver.

Root Server: If the ISP resolver doesn’t have the answer, it queries a Root DNS server.

TLD Server: The root server responds with the address of the TLD server (e.g., .com server).

Authoritative Name Server: The TLD server provides the IP of the authoritative server for google.com.

IP Address Returned: The authoritative server returns the actual IP (e.g., 142.250.182.46) to the resolver.

Cache & Response: The resolver caches the result and returns it to the user’s device.

Browser Connects: The browser uses the IP to establish a connection (via TCP/UDP).

DNS Record Types:

A Record: Maps domain → IPv4.

AAAA Record: Maps domain → IPv6.

MX: Mail server.

CNAME: Alias domain.

TXT: Miscellaneous text data (SPF, DKIM).

3. OSI vs TCP/IP Models
OSI Model (7 Layers):

Physical

Data Link

Network

Transport

Session

Presentation

Application

TCP/IP (4 Layers):
Network Access → Internet → Transport → Application.

Key Protocols:

HTTP/HTTPS: Web browsing.

SSH: Secure shell.

FTP/SFTP: File transfer.

SMTP, IMAP, POP3: Email protocols.

DNS: Name resolution.

MODULE 2 – Security Architecture & Defense-in-Depth
1. Defense-in-Depth (DiD)
Layered approach for reducing single points of failure.

Types of Security Controls:

Preventive: Firewalls, MFA, strong passwords.

Detective: IDS, SIEM alerts, logs.

Corrective: Backups, patching, recovery procedures.

2. Network Segmentation
Dividing networks into smaller, isolated segments.
Benefits:

Limits lateral movement by attackers.

Improves performance and security.

VLANs: Virtual LANs separate traffic logically.

DMZ (Demilitarized Zone): For hosting public services like web servers.

3. Firewalls
Packet-Filtering Firewall:
Allows or blocks packets based on headers (IP, port, protocol).

Stateful Firewall:
Tracks connection states (e.g., only allows packets from established sessions).

Application Firewall / WAF:
Filters specific web traffic (e.g., block SQLi attacks).

MODULE 3 – Authentication, Authorization & Encryption
1. Authentication vs Authorization
Authentication:
Proves who you are (e.g., password, OTP).

Authorization:
Determines what you can do (permissions, roles).

2. Multi-Factor Authentication (MFA)
Combines two or more factors:

Something you know: Password.

Something you have: OTP on phone.

Something you are: Biometrics (fingerprint, face ID).

3. Zero Trust Security
Principle:
Never trust any request, even from internal network.

Approach:
Verify every user and device using strict authentication.

4. Encryption
Symmetric Encryption:
Single key (e.g., AES).

Asymmetric Encryption:
Public/private key pair (e.g., RSA).

TLS/SSL:

Provides secure communication between client and server.

Uses handshake process and certificates (PKI).

MODULE 4 – SIEM & Incident Response
1. SIEM (Security Information and Event Management)
Functions:

Centralized log collection (e.g., from servers, firewalls).

Correlation & analysis (detects suspicious patterns).

Alerting & dashboards (visualize anomalies).

Reporting for compliance.

2. Incident Response Phases
Preparation:
Policies, incident response plan, tools ready.

Detection & Analysis:
Identifying threats (via SIEM, IDS).

Containment:
Isolate infected systems.

Eradication:
Remove malware, patch vulnerabilities.

Recovery:
Resume normal operations, monitor systems.

Lessons Learned:
Post-mortem analysis & documentation.

MODULE 5 – Practical Applications
Create a network diagram showing firewalls, DMZ, VLANs.

Simulate a mock incident: Document Detection → Containment → Recovery steps.

Learn real SIEM dashboards (e.g., Splunk Free, Google Chronicle).

EXTRA CONCEPTS (ESSENTIAL ADD-ONS)
1. TCP Handshake (3-Way)
Client → SYN → Server.

Server → SYN-ACK → Client.

Client → ACK → Server.
Connection established.

2. Ports and Protocols
Port 80: HTTP.

Port 443: HTTPS.

Port 22: SSH.

Port 53: DNS.

Port 25/587: SMTP (Email).

3. NAT & VPN Basics
NAT (Network Address Translation): Converts private IPs to public IPs.

VPN: Encrypted tunnel for secure communication.

