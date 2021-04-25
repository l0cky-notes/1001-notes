    Most people use their smartphone, tablets, and other mobile devices to send and receive email
    In order to do this, we have to configure the appropriate email settings for the devices and services we are using
    Sending and receiving email from an ISP’s server are done using different protocols
        POP3/IMAP – Receiving email
        SMTP – Sending
    Many corporate networks have different processes as well, often using Microsoft Exchange
    Other 3rd party integrations such as iCloud, Goole, Yahoo will need additional configuration to set up as well
    POP3 – Post Office Protocol v.3
        Has been used for a very long time, before many of the 3rd party vendors mentioned above
        It’s used for downloading mail to local mail client, usually from the ISP
        You also have the option to delete the message from the server
        This makes sense when you only have one device 
        Now that we have many devices which can receive email, we need more flexibility
        Some legacy equipment may still use POP3 so some additional configuration will need to be done
            Name of the POP3 server (Host Name)
            Authentication – username/password
            Software may sometimes require network port information
                Defined by ISP/mail provider
                POP3: tcp/110
                POP3S – SSL settings (encryption): tcp/995
    IMAP4 – Internet Message Access Protocol
        Allows you to receive emails but leave them stored on a central server
        Customize email inbox using folders
        Can also perform server-side searches using IMAP
        Configuration is almost identical to the POP3 protocol
            Name of IMAP server (Host name)
            Authentication – username/password
            Network port information
                Defined by ISP/mail provider
                IMAP: tcp143
                IMAPS – SSL settings (encryption): tcp/993

    SMTP – Simple Mail Transfer Protocol
        Allows you to send mail from your local device to your ISP SMTP mail server
        When sending, it needs to be from a trusted device so there is often authentication required
            May be different credentials than used for incoming mail
        Network port information
            tcp/25 – SMTP with no autentication, relatively unused
            tcp/587 – SMTP with authentication
    Microsoft Exchange
        Enterprise email
        POP3, IMAP, and SMTP work fine for using email at home
        In a work setting, you will often want access to additional features such as contacts, calendars, reminders, etc.
        Integrates with a mobile device database allowing constantly update calendars, contacts, etc.
        Configuration options
            Email
            Server
            Windows domain name
            Authentication
        S/MIME – Secure/Multipurpose Internet Mail Extensions
            Integrated message encryption
            Digital signatures
    Commercial email providers
        When not using email functionality provided from your ISP or Microsoft Exchange, you can sign up with one of a number of different 3rd party providers
        Gmail
            Google email
            Splits inbox into tabs
            IMAP4/POP3 support but additional functionality available
        Exchange Online (cloud based version)
            IMAP4/POP3 support
        iCloud Mail
            Apple Mail
            IMAP4 support only
        Yahoo Mail
            Integrated Yahoo functionality
            IMAP4/POP3