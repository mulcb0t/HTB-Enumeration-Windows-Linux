# HTB-Enumeration-Windows-Linux
Windows &amp; Linux Enumeration training (Medium difficulty) 

This project documents the enumeration phase of penetration testing using 2 different HackTheBox machines: Windows & Linux on Medium difficulty to simulate more realistic pentesting process


## Goal:

The goal of enumeration is to discover detailed technical information about the target, such as:

1. Open ports and its services
2. OS and version
3. Domain information
4. User/Group sessions
5. Shared resources and directories
6. Configurations
7. Potentially vulnerable endpoints


## Tools Used that have been used:

`nmap` : Scanning: ports, services, versions, scripts (NSE)
`enum4linux-ng` : SMB, RPC, LDAP enumeration
`rpcclient` : Remote procedure call enumeration (RPC anonymous connection)
`ldapsearch` : Active Directory Object and Domain discovery
`crackmapexec` : Automated SMB/AD enumeration
`smbclient` : Anonymous SMB access check
`nikto` : Web vulnerability scanner
`whatweb` : web server and technology fingerprinting
`curl` : to gather HTTP headers and redirection behavior
`gobuster` : web directory brute-forcing


## Windows Enumeration:

**Target IP:** `10.10.11.70`  
**OS:** `Windows Server 2022`  
**Domain:** `PUPPY.HTB`

## Key results:

1. SMBv1 disabled, SMB signing enabled and required
2. Enumerated services: LDAP, RPC, SMB
3. Partial anonymous access over SMB and LDAP
4. Domain and SID discovery
5. Supported SASL mechanisms and domain role


## Linux Machine Enumeration

**Target IP:** `10.10.11.67`  
**OS:** `Debian 12`
**Web Server:** `Nginx 1.22.1`  
**Framework:** `Laravel`

## Key results:

1. SSH with strong algorithms (for example: curve25519, chacha20)
2. Web tech stack exposed (Laravel, HTML5)
3. Login endpoints, session tokens and CSRF tokens found
4. Hidden directories via `Gobuster`
5. Web security headers and known vulnerabilities identified via `Nikto`

---

## Access to the project

Full technical report available in:

[Enumerácia.pdf](./Enumerácia.pdf) (written in Slovak)


## Author

Mulcb0t 
