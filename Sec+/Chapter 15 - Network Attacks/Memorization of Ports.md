---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---

| Service                                                                     | Purpose                                                                                                  | Port      | TCP/UDP  |
| --------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | --------- | -------- |
| File Transfer Protocol (FTP)                                                | To transfer files from host to host                                                                      | 21        | TCP      |
| Secure Socket Shell (SSH)                                                   | Remote administration of network devices                                                                 | 22        | TCP*/UDP |
| Secure File Transfer Protocol (SFTP)                                        | Secure transfer of files from host to host                                                               | 22        | TCP      |
| Secure Copy Protocol (SCP)                                                  | Secure transfer of files from host to host                                                               | 22        | TCP      |
| Telnet                                                                      | Unencrypted method to remotely administer network devices                                                | 23        | TCP*/UDP |
| Simple Mail Transfer Protocol (SMTP)                                        | Send email over internet                                                                                 | 25        | TCP      |
| Domain Name Service (DNS)                                                   | Hostnames to IPs and IPs to hostname                                                                     | 53        | TCP/UDP* |
| Trivial File Transfer Protocol (TFTP)                                       | Simplified FTP that uses UDP. "Lightweight"                                                              | 69        | UDP      |
| Hypertext Transfer Protocol (HTTP)                                          | Transmit webpage data to a client for unencrypted browsing                                               | 80        | TCP      |
| Kerberos                                                                    | Network authentication with a ticket system in a Windows environment                                     | 88        | TCP/UDP* |
| Post Office Protocol Version 3 (POP3)                                       | Receive unencrypted mail from a mail server                                                              | 110       | TCP      |
| Network News Transfer Protocol (NNTP)                                       | Transports Usenet articles to a client                                                                   | 119       | TCP      |
| Remote Procedure Call/Distributed Component Object Model (RFC/DCOM)         | RPC attempts to locate DCOM ports to request a service from a program on another computer on the network | 135       | TCP*/UDP |
| NetBIOS                                                                     | Conducts name querying, sending data, and other functions over a NetBIOS connection                      | 137 - 139 | TCP*/UDP |
| Internet Message Access Protocol (IMAP)                                     | Receive mail from other mail server with more features than POP3                                         | 143       | TCP      |
| Simple Network Management Protocol (SNMP)                                   | Used to remotely monitor network devices                                                                 | 161       | UDP      |
| Simple Network Management Protocol Trap (SNMP Trap)                         | Send InformRequest to the SNMP manager on a network                                                      | 162       | TCP/UDP* |
| Lightweight Directory Access Protocol (LDAP)                                | Maintain directories of users and other objects                                                          | 389       | TCP*/UDP |
| Hyper Text Transfer Protocol Secure (HTTPS)                                 | Secure/Encrypted version of HTTP using SSL/TLS                                                           | 443       | TCP      |
| Server Message Block (SMB)                                                  | Provides shared access to files and other resources on a network                                         | 445       | TCP      |
| Simple Mail Transfer Protocol with SSL/TLS (SMTP with SSL/TLS)              | SMTP with an SSL/TLS secure/encrypted connection                                                         | 465/587   | TCP      |
| Syslog                                                                      | Conduct computer logging especially for routers and firewalls                                            | 514       | UDP      |
| Lightweight Directory Access Protocol with SSL/TLS (LDAPS)                  | LDAP over secured/encrypted SSL/TLS                                                                      | 636       | TCP*/UDP |
| iSCSI                                                                       | Link data storage over IP such as in a Storage Area Network (SAN)                                        | 860       | TCP      |
| File Transfer Protocol Secure (FTPS)                                        | Secure/Encrypted FTP over TLS (SSL now deprecated)                                                       | 989/990   | TCP      |
| Internet Message Access Protocol with SSL/TLS (IMAP4*/IMAPS)                | Secure/Encrypted IMAP over SSL/TLS                                                                       | 993       | TCP      |
| Post Office Protocol Version 3 with SSL/TLS (POP3S)                         | Secure/Encrypted POP3 over SSL/TLS                                                                       | 995       | TCP      |
| Microsoft Server Structured Query Language (MS-SQL)                         | Microsoft SQL receives SQL database queries from clients                                                 | 1433      | TCP      |
| Remote Authentication Dial-in User Service Alternative (RADIUS Alternative) | Alternative ports for RADIUS                                                                             | 1645/1646 | UDP      |
| Layer 2 Tunnel Protocol (L2TP)                                              | Underlying VPN protocol that is unencrypted with no security. Should run IPSEC on top of                 | 1701      | UDP      |
| Point-to-Point Tunneling Protocol (PPTP)                                    | Underlying VPN protocol that is encrypted                                                                | 1723      | TCP/UDP  |
| Remote Authentication Dial-In User service (RADIUS)                         | Authentication, Authorization, and Accounting                                                            | 1812/1813 | UDP      |
| Fiber Channel Internet Protocol (FCIP)                                      | Encapsulates Fiber Channel Frames within TCP/IP packets                                                  | 3225      | TCP/UDP  |
| iSCSI Target                                                                | Listening port for an iSCSI targeted device when linking data storage facilities over IP                 | 3260      | TCP      |
| Remote Desktop Protocol (RDP)                                               | Remotely view and control other Windows systems via a GUI                                                | 3389      | TCP/UDP  |
| Diameter                                                                    | A more advanced AAA that acts as a replacement for RADIUS                                                | 3868      | TCP      |
| Syslog over TLS (Syslog over TLS)                                           | Secure/Encrypted Syslog over SSL/TLS                                                                     | 6514      | TLS         |
  
- See also [[Ports and Protocols]]

# Objectives
---
- [[Objectives#3.1 - Given a scenario, implement secure protocols|3.1 - Given a scenario, implement secure protocols]]