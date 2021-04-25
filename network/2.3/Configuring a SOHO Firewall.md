    Firewall
        Allows you to access the internet but protects your internal network resources from outside the network
        Can’t be disabled
        All SOHO routers are firewalls, they have them built in
    DMZ (Demilitarized Zone)
        Midpoint between two sides (internal network and the internet)
        Internal IP address or physical port can be configured as the DMZ
        Can be set to allow unrestricted access, however this is not recommended
            Better to use other port forwarding rules
    NAT (Network Address Translation)
        Estimated 20 billion devices connected to the internet, and constantly growing
        Each of the devices needs a unique IP address
        The current IP address format, IPv4, space has been completely used up so no new ones can be given out
            Ipv4 supports roughly 4.3 billion individual addresses
        NAT is the technology that allows the additional 15+ billion devices to connect to the internet even though there are not IPv4 addresses left
            NAT is an always on function inside a SOHO router
            Translates all internal IP addresses of devices on a network to a single external IP address 
            This is not the only use case for NAT
        Can have 1000’s of devices on an internal network, but to the outside it looks like one single IP address
            Any device on the internet that receives the traffic will see the external translated IP address
        Sometimes referred to as Source NAT or PAT (Port Address Translation)
    Port Forwarding
        Allows you to create a NAT address but in reverse for traffic coming into the network from the internet
        Allows round-the-clock access to a service that is hosted internally
            Web server
            Game server
            Security System
        Doesn’t expire or time out
        External port number or IP number maps to the internal IP of the service and doesn’t have to be the same port
        May be referred to as Destination NAT or Static NAT
    UPnP (Universal Plug and Play)
        Allows any network device to automatically find and connect to a network and and configure other devices on the network
        Instead of manually configuring port forwarding rules, you can have applications communicate directly with the router to enable/disable port access
            No approvals needed
        Ports will only open when that specific app is in use and close when you are finished
        This can be a security concern because you are not in direct control of what ports are opening/closing
            For cases like this, it may be a good idea to disable UPnP and manually configure port forwarding rules
    Whitelist/Blacklist
        Many SOHO routers allow content filtering
            Can be done by url/url name or by IP address ranges
        Whitelisting
            Nothing passes a firewall unless is on a pre-approved list
            Very restrictive
        Blacklisting
            All traffic is allowed unless it’s on a block list
            More liberal than whitelisting
    MAC Filtering (Media Access Control)
        MAC addresses are the hardware addresses of your device, similar to a serial number
        Can limit access to a network based on MAC address to control exactly what devices are allowed to connect 
        Not very secure because MAC addresses can easily be spoofed, meaning it can be changed to get through a firewall
            Can be found by capturing packets going across the network
        Considered “security through obscurity”, not secure
    Wireless Channels and Encryption
        You will want to configure your wireless connecting to have the highest security and encryption 
            WPA@-AES is the best choice
            More secure than WPA or WEP
            Check all devices, not all of them allow for highest security
        When setting up the wireless networks, it’s best to use an open frequency range so it won’t be conflicting with other devices in the area
            Some routers will configure the best frequency automatically
    Managing QoS (Quality of Service)
        You can change priority of traffic on your network
            Which types of apps and traffic will be prioritized
        Prioritize apps, ports, MAC addresses, etc. 
            Feature of higher end SOHO routers
        Do this with caution so traffic that needs priority doesn’t lose it