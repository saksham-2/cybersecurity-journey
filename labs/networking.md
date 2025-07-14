🌐 Networking Fundamentals (TryHackMe)
🚀 What is Networking?
Networking is how computers communicate with each other.

Uses protocols (standardized rules) for devices to send / receive data.

Examples: HTTP, TCP/IP, DNS, SMTP, FTP.

📦 Key Concepts
🔗 IP Address
Unique address for each device on a network.

Like your house address — needed to send/receive data.

IPv4: 192.168.1.1

IPv6: 2001:0db8:85a3::8a2e:0370:7334

🛣️ Routing
Decides path packets take to reach destination.

Routers forward packets from one network to another.

🖧 Subnet
Divides large networks into smaller ones.

Helps improve performance & security.

🗄️ DNS (Domain Name System)
Converts human-friendly names (tryhackme.com) to IP addresses (104.26.3.240).

📬 MAC Address
Hardware address of NIC (Network Interface Card).

Used inside local networks (switches use this).

🌍 OSI Model Layers
Layer	Example Protocols	What it does
7. Application	HTTP, FTP, DNS	Interface for user applications
6. Presentation	SSL, TLS	Encrypt / decrypt, compression
5. Session	NetBIOS	Starts, maintains, ends sessions
4. Transport	TCP, UDP	Reliable/unreliable delivery
3. Network	IP	Logical addressing, routing
2. Data Link	Ethernet	MAC addressing
1. Physical	Cables, Wi-Fi	Actual bits over medium

💡 TIP: TCP is like sending registered mail, UDP is like sending a postcard.

🔍 Common Tools & Commands
🖥 ping
Checks if a host is reachable.

bash
Copy
Edit
ping google.com
🗺 tracert / traceroute
Shows path packets take.

bash
Copy
Edit
traceroute tryhackme.com
🛠 nslookup
Looks up DNS records.

bash
Copy
Edit
nslookup tryhackme.com
🔧 ipconfig / ifconfig
Shows local IP configuration.

🌐 HTTP & How The Web Works
Web browsers use HTTP to communicate with servers.

Request → Response model:

Browser sends HTTP GET request to server.

Server sends back HTTP Response (HTML, CSS, JS).

HTTP Status Codes:

Code	Meaning
200	OK
404	Not Found
500	Server Error

🛡 Basic Security Concepts
Firewalls block/allow traffic based on rules.

IDS/IPS systems detect/prevent malicious activity.

Packets can be sniffed with tools like Wireshark.