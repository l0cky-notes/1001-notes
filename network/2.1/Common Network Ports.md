Protocol Name Port
FTP File Transfer Protocol tcp/20
tcp/21
SSH Secure Shell tcp/22
TELNET Telecommunications Network tcp/23
SMTP Simple Mail Transfer Protocol tcp/25
HTTP Hypertext Transfer Protocol tcp/80
HTTPS Hypertext Transfer Protocol Secure tcp/443
POP3 Post Office Protocol v.3 tcp/110
IMAP4 Internet Message Access Protocol v.4 tcp/143
RDP Remote Desktop Protocol tcp/3389
SMB Server Message Board tcp/445
AFP Apple Filing Protocol tcp/548
SLP Service Location Protocol tcp/427
LDAP Lightweight Directory Access Protocol tcp/389

```
HTTP – Hypertext Transfer Protocol
    tcp/80
    Protocol for a web browser to communicate with a web server 
    Other applications may use the protocol as well
    In-the-clear communication
HTTPS – Hypertext Transfer Protocol Secure
    tcp/443
    Encrypted version of HTTP
POP3 – Post Office Protocol v.3
    tcp/110
    Basic protocol for receiving email on mobile devices and computers
	downloads the email to your device from a mail server 
	ONLY downloads what's in your inbox folder
IMAP – Internet Message Access Protocol
    tcp/143
    More advanced protocol for receiving email
    Has additional functionality such as inbox filtering, management of multiple clients, etc.
	gmail as an exsample 
RDP – Remote Desktop Protocol
    tcp/3389
    Protocol that allows you to remotely access the desktop of another computer
    Can access the entire desktop or a single file
    Remote Desktop Service is available for Windows and there are other clients for other operating systems
SMB – Server Message Board
    tcp/445
    Modern Windows proprietary system for transferring files, print sharing, etc.
    Full-featured
    Sometimes referred to as CIFS (Common Internet File System)
NBNAME – NetBIOS
    udp/137
    Older Windows systems used NetBIOS
    Name services
NBDATAGRAM
    udp/138
    Datagram services
NBSESSION
    udp/139
    Session services
AFP – Apple Filing Protocol
    tcp/548
    Apple’s proprietary protocol for transferring files 
    Full-featured
    Works with SLP to be able to view the available list of servers
SLP – Service Location Protocol
    tcp/427
    Protocol that allows you see available servers
LDAP – Lightweight Data Access Protocol
    tcp/389
    Provides authentication credentials when you try to access a corporate network, either through a VPN or a server on the network
    Database the stores usernames and passwords for the network and changes about permissions etc. can be made in one location 
```

Common UDP Ports
Protocol Name Port
DNS Domain Name System udp/53
DHCP Dynamic Host Configuration Protocol udp/67
udp/68
nbname NetBIOS Name Services udp/137
nbdatagram NetBIOS Datagram Services udp/138
nbsession NetBIOS Session Services udp/139
SNMP Simple Network Management Protocol udp/161
udp/162
SLP Service Location Protocol udp/427

```
FTP – File Transfer Protocol
    tcp/20 – active mode data transmission
    tcp/21 – communication control
    One of the first ways of transferring a file from one device to another
    Can have security features built in like authentication using a username and password
        Anonymous login also supported
    Full-featured functionality meaning other file functions can be performed as well such as add, delete, list, etc. 
SSH – Secure Shell
    tcp/22
    Protocol that allows you to connect remotely and securely from the command line of one device to another
        Encrypted communication link, similar to remote connections done using Telnet
Telnet – Telecommunications Network
    tcp/23
    Older version of remote communication done in-the-clear, meaning no encryption and the entire transmission can be read including sensitive information like username and passwords
    Some legacy equipment can’t establish a secure connection using SSH, so it will utilize Telnet
SMTP – Simple Mail Transfer Protocol
    tcp/25
    Protocol used for sending email messages
    Can be sent from devices to servers or from servers to servers
    Not used for receiving email, this is done by another protocol
DNS – Domain Name System
    udp/53
    When you visit a website by tying a domain name into your browser, the DNS protocol is working behind the scenes to translate the domain name of the website with the IP address of the website stored on the web server
    DNS servers are extremely critical so they will often have backup servers ready to take over incase of a server failure to keep the website online
DHCP – Dynamic Host Configuration Protocol
    udp/67
    udp/68
    When you turn on your computer for the first time, it automatically configures itself with an IP address on the network your connected to
    Once the computer receives the IP address, it’s “leased” for a specified amount of time and before the time is up, it will check back in with the DHCP server to see if the address is still available
    IP addresses are given out in real-time from a pool
    Can be configured with reservation, meaning that when a device requests and IP address, the server can recognize the MAC address of the device and provide it the same IP address every time
SNMP – Simple Network Management Protocol
    udp/161 (queries)
    udp/162 (traps/alerts)
    Network admins can be in control of well over 1000 devices on a network
    SNMP is a protocol that allows communication and gathering of statistics about the devices on the network
    Version 1 – in-the-clear
    Version 2- in-the-clear, bulk transfers added
    Version 3 – encryption and authentication features added
SLP – Service Location Protocol
    udp/427
    Protocol that allows you to locate available servers
```