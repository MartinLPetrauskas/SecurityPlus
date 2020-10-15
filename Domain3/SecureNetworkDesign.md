## Secure Network Design

### Security Zones
* Internet Zone: the outside world of the Internet
* Intranet Zone: internal network of the organization
* DMZ: zone specifically for resource that need to be accessed by the outside world, i.e. web server
* Extranet: Intranet segments extendeds to business partners
* Honey Nets: decoy networks designed to attract attackers
* Ad Hoc Networks: temporary network that may bypass security controls

### Public & Private Addresses
* Public IP Addresses: assigned by a central authority and are routable over the Internet
    * IPv4 Addresses are now scarce, no large blocks available 
* Private IP Addresses: Available for anyone to use, but not routable over the Internet
    * 10.0.0.1 - 10.255.255.255
    * 172.16.0.1 - 172.31.255.255
    * 192.168.0.1 - 192.168.255.255
* Network Address Translation: translates private IP addresses
    * Hides internal addresses from Internet systems
    * Limits direct access to systems
    * Makes it difficult to identify the true origin of traffic
* Port Address Translation:
    * Allows multiple systems to share the same public address
    * Assigned unique ports to each communication
    
### Subnetting
* subdivides large networks
* Subnet Masks: identifies the dividing line between network and host addresses

### VLANs
* separate systems on a network into logical groups based upon function, regardless of physical location
* VLANs extends the broadcast domain
* Configuring VLANs:    
    * Enable VLAN trunking
    * Assign switchports to VLANs
    
### Security Device Placement
* Network Traffic Controllers
    * Intrusion Detection and Prevention sensors
    * Network taps
    * Port mirrors
* Security Information and Event Management
    * Gathers information using collectors
    * Analyze information with a centralized correlation engine
    * Place collectors near the system generating records
    * Place the correlation engine in a secure location
* Proxy servers and content filters typically belong in the DMZ
* VPN Concentrators:
    * Aggregate remote user connections
    * Often resie in their own VLAN, where access control may restrict remote user activity
    * Sophisticated designs may use multiple VLANs
* SSL Accelerators: Handle the difficult cryptographic work of setting up TLS connections
* Load Balancers: Distribute connection requests among multiple servers

### Software Defined Networking (SDN)
* Network Functions:
    * Control Plane: responsible for making routing and switching decisions
    * Data Plane: responsible for carrying out the instruction of the control plane
* SDN Security Benefits
    * Allows granular network configuration
    * Facilitates faster response to security incidents
* SDN increases network complexity

### Port Isolation
* Port isolation and private VLANs are the same thing
* Port isolation restricts traffic from a source port to a single destination port
* Why use port isolation:
    * Prevents devices on the same switch from communicating with each other
    * Blocks data-link later attacks like ARP spoofin
* Port isolation isn't effective on a corporate network
