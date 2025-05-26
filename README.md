# task_01
Internship task - Day 1



PRE-REQUISITES:

Tools Used:
1. nmap: Nmap (Network Mapper) is a free, open-source tool used for network discovery and security auditing. It helps identify devices, open ports, and services running on a network, making it essential for network administrators and security professionals. Nmap runs on all major operating systems, including Windows, Linux, and macOS.

Resources Used:
1. https://nmap.org/download#windows
   => Website to download "nmap" tool for windows, linux and macOS.



PROCEDURE:

Step 1: First, I used "ipconfig" to find my local IP range. This IP range is the range in which a router assigns IP addresses dynamically to devices connected to it.

![image](https://github.com/user-attachments/assets/5d31bf7c-2b06-4e13-bcab-c37afcb7eebf)

![image](https://github.com/user-attachments/assets/e64409c1-6e3c-4fcf-b7af-bfe19a627420)


Step 2: Then, I used "nmap --help" to find out about the various parameters that can be used to scan through an IP address.

![image](https://github.com/user-attachments/assets/0cb6ae48-47af-4579-b6dc-a15805339af2)


Step 3: I found out that "-sS" can be used to perform

![image](https://github.com/user-attachments/assets/cf59f72f-e377-4116-be3c-7cf9e2e5de19)


Step 4: Then I ran the given command "nmap -sS <IP_ADDRESS>" on the target




Step 5: The following ports were open and the services used on them were as follows:



RESULTS:

PORT    STATE    SERVICE
21/tcp  filtered ftp
23/tcp  filtered telnet
53/tcp  open     domain
80/tcp  open     http
139/tcp filtered netbios-ssn
443/tcp open     https
445/tcp filtered microsoft-ds



CONCLUSION:

Common services running on the ports:
-> Port 21: FTP -> File Transfer Protocol
   Port 22: SSH -> Secure Shell
   Port 23: Telnet -> Unencrypted Remote Access
   Port 25: SMTP -> Email Sending
   Port 53: DNS -> Domain Name System
   Port 80: HTTP -> Web Browsing
   Port 110: POP3 -> Email Retrieval
   Port 143: IMAP -> Email Management
   Port 443: HTTPS -> Secure Web Browsing
   Port 445: SMB -> Windows File Sharing
   Port 3389: RDP -> Remote Desktop Access

Security vulnerabilities posed by open ports:
-> Open ports can expose your network to several security risks, as they provide entry points that attackers may exploit to gain unauthorized access. If the services behind open ports are unpatched, misconfigured, or     vulnerable, attackers can use them to launch malware, perform brute-force or injection attacks, and even disrupt services through denial-of-service (DoS) attacks. Open ports also make it easier for cybercriminals      to scan your network, gather information for further attacks, and potentially steal sensitive data or compromise system integrity. Reducing unnecessary open ports and properly securing those that must remain open      is essential for minimizing your attack surface and preventing breaches.
