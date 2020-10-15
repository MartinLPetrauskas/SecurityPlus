## TCP/IP Suite

### Internet Protocol
* routes information across networks
* providing an addressing scheme
* deliver packets from source to destination

### Transport Layer Protocols
* TCP
    * connection oriented protocol
    * guarantees delivery through acknowledgement
    * Widely used for critical applications
    * TCP Flags:
        * SYN: opens a connection
        * FIN: closes a connection
        * ACK: acknowledges a SYN or FIN
    * Threeway Handshake:
        * SYN
        * SYN/ACK
        * ACK
* UDP
    * lightweight, connectionless protocol
    * does not send acknowledgements
    * is used for voice or video
    
### OSI Model
* Physical Layer: wires, radio, and fiber optics
* Data Link Layer: data transfers between two nodes
* Network Layer: Internet Protocol (IP)
* Transport Layer: TCP & UDP
* Session Layer: Exchange between system
* Presentation Layer: Data translation and encryption
* Application Layer: User programs

### IP Addresses
* Dotted Quad Notation: i.e. 215.67.90.125
* Uniquely identifies system on a network
* Must not be reused on Internet connected systems
* May be reused if on private networks

### Subnets
* IP addresses are divided into two parts: network and host address

### IPv6
* Replaces IPv4 due to address exhaustion
* Uses 128 bits
* Consists of eight groups of  four hexadecimal digits

### Domain Name Service (DNS)
* translates domain names into IP addresses
* functions over UDP port 53
* computer sends DNS query to local DNS server first
* if not, other DNS servers are contacted using a hierarchical system

### Network Ports
* like apartment numbers, they guide traffic to the correct final destination
* 65536 possible ports, 0-65535
* port ranges:
    * 0-1023: well known ports
    * 1024-49151: registered ports
    * 49152-65535: dynamic ports
* Port 21: File Transfer Protocol (FTP)
* Port 22: Secure Shell (SSH)
* Port 3389: Remote Desktop Protocol (RDP)
* Port 137, 138, 139: NetBIOS
* Port 53: Domain Name System (DNS)
* Port 25: Simple Main Transfer Protocol (SMTP)
* Port 110: Post office Protocol (POP)
* Port 143: Internet Message Access Protocol (IMAP)
* Port 80: Hyper Test Transfer Protocol (HTTP)
* Port 443: Secure HTTP (HTTPS)

### ICMP
* ping: identifies live systems
    * ICMP ECHO REQUEST
    * ICMP ECHO REPLY
* traceroute: identifies network paths