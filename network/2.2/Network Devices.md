```
NIC – Network Interface Card
    The fundamental network device 
    No matter how you connect to a network, either through a wire or wirelessly, you will need some piece of hardware to make this connect happen, namely a network interface card
    Every single device on a network has a NIC
        Mobile phone
        Desktops
        Printers
        Servers
    NIC’s are often built into the motherboard or have a specific external adapter to attach them 
    Come in many different forms
        Single-port
        Multi-port 
        Fiber
        Copper
Repeater
    Networks have a maximum length that a signal can travel over a given topology
    Repeaters extend the signal distance by regenerating and sending the signal back out 
    There are no forwarding decisions being made, it is an automatic in/out process, the signal simply goes in one connection and out another
    Can be used to convert from one network type to another such as converting fiber to copper
    Can also extend the the capacity of a wireless network 
Hub
    In the early days of networking, a hub was used to connect a lot of devices together
    Sometimes referred to as a multi-port repeater
    In a hub, information is sent into one interface and then repeated to the rest of the interfaces 
        They can have up to hundreds of interfaces 
    Half-duplex communication
        This mean that two devices can’t be transmitting signals simultaneously
        One device will start AND finish a transmission before another one is allowed to start, this process becomes slow and very inefficient as networks grow in size
        10 and 100 mb/sec speeds available 

Bridge
    Bridges connect smaller networks together through their hubs
    More capability and control than a hub by being able to make forwarding decisions about which traffic should be forwarded through the bridge
        Does this based on the destination MAC address inside the Ethernet frame
        Used ot only have 2-4 interfaces available to make these forwarding decisions 
        Operates similarly to how modern day switches operate
    Made it possible for networks to be smaller and connect with each other insteading of growing the size of a single network 
        Hubs perform more efficiently with smaller network demands
    Different network topological can be connected 
        Ex. ethernet to WAN
    Traffic get distributed based on MAC addresses
Switch
    Expanded bridges to very large scale systems that can have hundreds of ports
    Forwarding decisions are made in the hardware
        Forwards traffic based on MAC address and data link address
        ASIC (Application Specific Integrated Circuit
    Extremely fast because switching is done in the hardware
    Multi-layer switch
        Includes routing functionality when the destination of the traffic is an IP address 
    Unmanaged switch
        Basic functionality with no configuration
        Plug and play
        Very little integration with external devices
        No management protocols
    Managed switch
        More functionality
        VLAN support on different interfaces
        Interconnect with other switches through 802.1Q
        Traffic prioritization
        Redundancy support via spanning tree protocol
        External management via SNMP 
        Troubleshooting via port mirroring/capturing packets
Router
    Device that makes forwarding decisions based on destination IP address
    Routes traffic between IP subnets
    Can be integrated into switches, sometimes referred to as “OSI Layer 3 switches”
    Can connect diverse network types and topologies
WAP – Wireless Access Point
    Similar to routers but with different functionality 
    A bridge that can extend a wired network onto a wireless network
    Wireless routers are routers and WAPs in one device
    Makes forwarding decisions based on MAC address
Wireless LAN Controller
    Large facilities like hospitals or universities manage many WAPs
    Wireless LAN controllers allow you to do this from a centralized location
        Deploy access points
        Performance/security monitoring
        Configure and deploy changes to all sites
        Report on access point use
    Usually a proprietary system made up of a controller and access points
    Can be cloud based allowing you to monitor and manage the console from anywhere physically
Firewall
    Manage and control the traffic flow through the network, especially from the internet
    Traditional firewalls filters by TCP/UDP port number, sometimes referred to as “OSI Layer 4 filtering”
    Modern firewalls can monitor everything in the signal all the way down to the application data
        Enable database transactions but prevent file transfers through the network
    Can create encrypted tunnels going in/out of the firewall
        Connect to a corporate firewall from an external remote location to get access to the internal resources of the network
    Older firewalls can act as a proxy, sitting between the two ends of the communication
    Can be used as a router (layer 3 device)
        Sits on the edge of the network and does routing/NAT based on the routing engine built into the firewall
Cable Modem
    Allows you to connect to a broadband internet connection that sends data using DOCSIS (Data Over Cable Service Interface Specification)
    Supports 4-250 mb/sec transfer speeds, sometimes up to gigabits/sec
    Transmission across multiple frequencies
    Supports different traffic types
        Data
        Voice
        Video
DSL Modem – (Digital Subscriber Line)
    Common alternative to cable modem that uses telephone lines
    Sometimes referred to as ADSL (Asymmetric DSL) meaning tat the download speed is greater than the upload speed
    Approx 10,000 ft distance from the CO (Central Office)
    Faster speeds the closer you are to the CO
        52 mb/sec downstream
        16 mb/sec upstream
	Adsl is normal in home because it is cheap
	sdsl is normal in bussese and the download and upload speed is the same
Cable Infrastructure in an office setting
    In a typical corporate office space, each workstation would have cabling connected to their devices and run to a networking closet connected to a patch panel
    The cables terminate on a 110 block connected to RJ45 connectors where ethernet patch cables can connect and reconnect different patches to the switches(also in the network closet)
        Allows for easy connections
    You only have to punch down the cables from the workstations one time, they are permanently connected to the patch panel 
```

*This model is not drawn to scale, it is meant for demonstration purposes only to show the functionality of how an office network is built

```
PoE – (Power Over Ethernet)
    On a WAP, there are traditionally two connections
        Network connection
        Power supply
    Modern devices provide PoE through the ethernet cable, allowing for only a single connection
    Endspan
        Power is provided at the switch and goes directly to the end device
    Midspan
        An additional, in-line power injector is added to provide power
    PoE switches are commonly marked on the switch or interface
EoP (Ethernet Over Power)
    Reverse of PoE, also called powerline communication (PLC)
    IEEE standard 1901
    500 mb/sec
```