```
iTCP/IP is one of the most popular protocols used today
Transferring data in a network from one device/location to another can roughly be equated to the process of moving you and your family from one house to another:
    Network topology = road
    TCP/IP (internet protocol) = moving truck
    TCP/UDP Data = boxes 
    Application data = belongings
Visualization
    A client sends information to a server using an ethernet frame. Inside the frame, there is a header at the beginning and a trailer at the end. Between the header and trailer is the ethernet payload. We can keep going in deeper through the ethernet frame to see how the rest of the data is organized. Inside the ethernet payload is an IP header followed by an IP payload. Inside the IP payload is a TCP header followed by a TCP payload (TCP could be UDP), and ultimately inside the TCP payload is the application data you are trying to send. This can be a number of different kinds of data. For example HTTP data that is being sent to a web server.

TCP and UDP
    Encapsulation
        With the nesting of data as seen above, we can describe the process as follows:
        Ethernet is surrounding IP which is surrounding TCP or UDP data which is surrounding the application data we are trying send
        Different types of applications have different features and have certain requirements for how they will be sent
        Encapsulation gives us several different ways to move data from one location to another
            TCP “box”
            UDP “box”
        This whole process is one part of what is often referred to as the OSI model and may be called an OSI process
        TCP/UDP operate at OSI level 4, the transport layer
    Multiplexing
        The concept of being able to put multiple applications in different frames and send them all across the network at the same time
        Allows you to perform many different functions simultaneously over the same network connection
TCP – Transmission Control Protocol
    Connection-oriented
        There is a formal process to start and stop the communication
        Similar to a phone call
    “Reliable” form of delivery because if any errors occur there is a process for re-transmitting the data to get everything across
    Flow control – the receiver can manage how much data is sent. There is an ACK (acknowledgement) everytime data is sent, and if it doesn’t get through, it will be resent
UDP – User Datagram Protocol
    Connectionless-oriented
        No formal open or close to the connection
        Data is simply sent through the network and arrives on the other side
        “Unreliable” form of delivery
            No error recovery
            No reordering data or retransmission
            This doesn’t mean that there is any less chance of the data reaching its destination, only that there are no acknowledgments that data is being sent
        No flow control – the sender determines the amount of data being transmitted 
Delivery of data
    The IP “delivery truck” transports packets of data from one IP address to another
    Similarly to how every house on a street has an address, every computer or device has an IP address determining its “location”
    Once data gets to its destination IP address, it needs to know which “room” it’s supposed to be put in
    IP uses port numbers as rooms
    Depending on the type of data being transmitted, a specific service designated by a port number will be where the data is brought inside the server
        Ex. port 80, port 443, etc.
Sockets
    Putting all this together, we have what’s known as an IP socket
    Ex. IPv4 socket
        Server IP > Protocol(TCP/UDP) > Server app port #
        Client IP > Protocol(TCP/UDP) > Client port #
Types of ports
    To be able to communicate, we need to be able to use many different port #’s at the same time
        Non-ephemeral ports (permanent)
            Port #’s 0-1023
            Usually on a server or service
            Usually assigned to an application 
            Ex. A web server often uses port 80
        Ephemeral ports (temporary)
            Port #’s 1024-65535
            Determined randomly in real time by the client when the server is communicating back
            These ports will only be in use during the current session, thus being ephemeral
    TCP/UDP ports can be any number from 0-65535
    Most servers (services) use non-ephemeral port #’s, but not always
    Port numbers are used for communication, not security, therefore there are not explicit rules determining which ports get used 
    Service port numbers need to be “well-known” because the client you are using needs to know the port number open on the server
        Ex. Web browsers expect to use tcp/80 on a web server. If the server is using any other port for web browsers, by default your browser will not be able to communicate with the server
        To fix this, you will need to manually specify your browser to use a different port number that matches the one on the server
    This could become very complicated if everyone using a web browser gets to decide the port number their browser would connect to on the server
        tcp/80 has become a standard allowing all web browsers  to be able to know how to access all web servers on the internet
        Even though this seems like a rule, it is not hardcoded into the actual process, it’s more of a general rule-of-thumb
    TCP/UDP are not the same
        One application can be using tcp/80 and another using udp/80 and the application will not be in communication
```