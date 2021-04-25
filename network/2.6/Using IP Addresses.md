    SSL VPN – Secure Sockets Layer Virtual Private Network
        Uses common SSL/TLS protocol over tcp/443
        Avoids running into firewall issues
        Commonly used by end users to create a secure tunnel between your device and the corporate network 
        Authenticates users allowing them to use the same credentials they already use
        Don’t need digital certificates/shared passphrases like you would using IPSec
        Can be run from a browser or a VPN client installed in your OS
        Sometimes referred to as client-to-site or remote access VPN
        Requires software on user devices that will connect back to your corporate network through an encrypted tunnel 
        A VPN concentrator sits between your device and the network and decrypts the communication before it reaches the network 
        Also encrypts the communication as it goes back out from the network to your device
    LAN – Local Area Network
        Group of devices that share the same broadcast domain
        LAN’s can be isolated by using separate switches, for example separate networks for the emergency room and cafeteria in a hospital 
        VLAN – Virtual LAN
            Allows the same functionality of controlling two LANs, but from the same switch 
            Logical separation instead of physical 
            Simplifies administration/cost of running the networks
            Devices on separate VLAN networks cannot communicate with one another directly 
    NAT – Network Address Translation 
        20 billion devices connected to the internet throughout the world 
        IPv4 has 4.3 billion possible addresses to use and all of them are taken by this point 
        NAT allows us to connect more devices to the internet by translating multiple IP address from the same local network to one shared IP address the represents the entire network 
        Can have thousands of devices on a network be represented by one single public IP that’s facing out to the internet
        NAT has other functions as well

