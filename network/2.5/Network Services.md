```
Web Server
    Responds to a request from your browser when you go to a website
    Standard web protocols that are used are HTML and HTML5 (Hypertext Markup Language)
    Web pages are stored on the web server and when your browser makes request to access them, they are downloaded to your browser to allow you to visit and view to web page
        Static pages are pages that were previously created
        Dynamic pages are ones that are created in real time when some makes a request from the server 
File Server
    Centralized storage of documents, media, spreadsheets, and any other type of file an organization would need to store
    Standard protocols for file management:
        SMB (Server Message Board) – Microsoft
        AFP (Apple Filing Protocol) – Apple
    Clients/users don’t directly access the file management systems through these protocols, it’s done through a file manager winder in their operating system. The protocols handle all of the transactions behind-the-scenes
Print Server
    Connects a printer to the network that is available to all other devices
    Acts as a proxy between your computer and the printer
        Could be software in the client workstation 
        Could be built-in to the printer
        Standard printing protocols
            SMB (Server Message Block)
            IPP (Internet Printing Protocol)
            LPD (Line Printer Daemon)
DHCP Server
    Dynamic Host Configuration Protocol will automatically configure an IP address for your device
    Very common service found in most SOHO routers
    Enterprise DHCP may have multiple routers
DNS Server
    Domain Name System is a protocol that converts domain names into IP addresses and vice versa
    Distributed naming system with thousands of servers all around the world
    Usually managed by an ISP or enterprise IT department
    Very critical resource so there are usually backups ready to go in case of an emergency
Proxy Server
    Many organizations use a proxy server to access anything on the internet
    Acts as an intermediary (proxy) between your machine and the resource you are trying to access
    The client first makes a request to the proxy
    The proxy then performs the request on the clients behalf to the resource on the internet 
    The proxy then provides the results back to the client 
    Proxy has many useful features that make it a good place to perform security functions
        Access control
        Content scanning/filtering
        Caching
        Malware scanning
Mail Server 
    Allows you to access emails from all your devices
    Stores incoming and sends outgoing emails
    Managed by ISP or IT departments
    Very stringent and complex requirements for up time because they are import resources
    24/7 support
Authentication Server
    Device that checks credentials such as username and password when you’re trying to access resources on a network
    Centralized server that all members of a network will be connected to 
    Not usually seen on a SOHO network because there aren’t that many users and login credentials can be managed by the individuals 
    Mostly seen used in enterprise situations
    Redundant service meaning that the service is spread across multiple servers in case one goes down, another will back it up
    Import service, 24/7 support 
SIEM – Security Information and Event Management
    Allows you to log and manage all of your network activity from all of these different devices and services in one centralized location
    Commonly used by security teams to monitor network activity and look for trends in behavior
    Will give alerts and reporting in real-time
    Link diverse types of data to look for correlations in log aggregation over long periods of time 
    Can be used for forensic analysis after an event occurs
Syslog
    Standard process for transferring log files from the various network devices and servers to the SIEM
        Central logging receivers are integrated into SIEM 
    Extremely memory intensive to store the log files over long periods of time 
        Commonly uses WORM drives (Write Once Read Many – DVD-R)
        Information is written to an optical drive once and it cannot be changed or edited afterwards 
        Protects important security logs 
IDS/IPS – Intrusion Detection/Prevention System
    Allows network admins to watch for intrusions onto the network 
    Intrusions include:
        Exploits of OS or apps
        Buffer overflows
        Cross site scripting
        Database injection
    Detection vs. prevention systems
        Detection – alarms or alerts when something happens
        Prevention – stop the incident from happening before it gains network access and additional capabilities
All-in-one Security
    Many different capabilities:
        URL filtering/content inspection
        Malware inspection
        SPAM filtering
        WAN CSU/DSU
        Router, switch, firewall
        Bandwidth shaper
        Intrusion prevention system
    Goes by many different names:
        Next generation firewall
        UTM (Unified Threat Management)
        Web security gateway
Endpoint Management Server
    To avoid doing updates and performing management functions on every single device on a network, EMS allows an admin to do it from “a single pane of glass”
        Software installations/updates
        Driver installations
        Security patches 
        Remote troubleshooting
    Requires an initial install on the client device called an agent, but after that they are set up
        EMS sends the commands
        Agent executes the commands
Legacy and Embedded Systems
    Legacy systems
        Older and usually outdated systems
        Usually perform important functions 
    Embedded systems
        Purpose-built electronic systems outside the tradition network devices
        Specific, sometimes proprietary systems used for a specific task 
        Alarm systems
        Time car systems
        Etc.
```