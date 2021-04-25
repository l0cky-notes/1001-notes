    In the early days of networking, IPv4 configuration used to be manual
    All setting and configurations had to be entered by hand in order to connect to a network
        IP address
        Subnet mask 
        Gateway
        DNS servers
        NTP servers
    BootP – Bootstrap Protocol 
        Introduced in Oct. 1993
        Made some network configurations automatic but not all of them 
        Wasn’t able to tell when an IP address would become available
        Couldn’t add VOIP gateway information
    DHCP – Dynamic Host Configuration Protocol
        Introduced in 1997 with continuous updates throughout the years 
        Provides automatic IP address assigning to almost all devices
        Process for assigning IP addresses:
            Discover
                Workstation device send out broadcast to udp/67 over the network and will reach DHCP servers that have been configured on the network 
            Offer
                If the DHCP server has an available IP address, it will broadcast back to the client workstation through port udp/68
            Request
                Now that the client knows an IP address is available, it will send a request for the address back over port udp/67
            Acknowledgement
                Once the DHCP server receives the request for the IP address, it will send an acknowledgement back to the client over udp/68
            The client can now configure the IP address

    IP Reservation
        DHCP servers assign IP addresses from a pool of available addresses and because of this, sometime your IP will change
        To avoid this you can disable DHCP on your device, but then you would have to go an manually add all the configuration information to connect to the network
        IP reservation can be configured on DHCP to reserve specific address for specific devices based on their MAC addresses
    APIPA – Automatic Private IP Addressing
        If your device can’t connect with a DHCP server for any number of reasons , you can still get an IP address and communicate with devices on your network through APIPA
        Link-local address
            Allows you to communicate inside a local subnet but not outside of it 
            Forwarding by routers to other destinations is not available
            IETF reserved a set ranges of IP’s to be used as local/private IP addresses
                169.254.0.1 > 169.254.255.254
            The first an last 256 of these are reserved from being used, so the actual functional range of addresses:
                169.254.1.0 > 169.254.254.255
            This assignment is done automatically if DHCP is not found
            Before the address is actually assigned, an ARP (address resolution protocol) will be sent out to the network making sure no other devices have claimed the IP address
    IPv6 Link-local Addresses
        Functionality that’s automatically assigned to all IPv6 addresses
        May have  a link-local address as well as an IPv6 address that allows it to communicate outside your subnet
        Link-local addresses are written:
            fe80:: (followed by all 0’s for the first 64 bits)
            The last 64 bits are usually created from the devices MAC address so there is some uniqueness to it