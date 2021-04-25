ost corporate offices or other large organizations have data centers dedicated to building the technological network of the organization

```
Consists of many racks of servers, routers, switches, firewalls, and all all the other physical devices that make up a network 
Not compatible for small office and home networks because of space limitation
Most of these dedicated pieces of equipment can be collapsed down into one device: a SOHO router 
```

SOHO Router (Small Office Home Office)

```
Single device with a lot of functionality to take care of networking on a small scale
Routing
    Connects the network to the outside world (internet, other networks), usually through DSL/cable
Switching
    Ethernet interfaces used to connect cables of more devices (VLAN, LAN1, LAN2, etc.)
Not much configuration needs to be done, routing and switching happens automatically
Many include WAP functionality and the ability to configure these settings
    Frequency bands: 2.4/5 GHz
    Configure SSID (name of wireless network)
        Might need to configure a new SSID for every frequency
    Security mode
        WPA2(recommended)
        Pre-shared keys
        Enterprise mode(username/password for every user)
    Configure a channel or set of channels for the particular access point 
```

IP Addressing

```
WAN and LAN connections need to have IP addresses assigned to them
    WAN IP is automatically assigned via DHCP from the ISP (may require authentication)
LAN interface will automatically assign IP addresses because the SOHO router itself is a DHCP server
    Internal IP addresses are defined in a given range from the SOHO router
    DNS servers are passed to clients during the DHCP process and if left blank, will default to the WAN values 
```

NIC Configuration

```
When you plug a wired Ethernet device into a SOHO router, its speed is automatically configured in duplex
    Can be manually set on devices
    10/100/1000 mb/sec speeds
    Duplex: half/full(full preferred)
Wireless network connection
    Enable/disable wireless adapter
    Select SSID from a list
    Provide a password to connect to the network 
```

End-user Device Configuration

```
Different OSs will have different ways of configuring their options and setting, but the names should generally be the same across platforms
Most efficient way is to enable DHCP and have the SOHO router internal configurations be used 
```

IoT Configurations

```
Used for home/office automation
These devices are becoming more and ore common
    Thermostats
    Security cameras
    Refrigerators
    Etc.
Usually connected to your network through an 802.11 wireless network connection
Usually connect outbound automatically when they are powered on 
    Connects to a central server with little to no configuration
```