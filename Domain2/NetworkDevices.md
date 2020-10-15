## Network Devices

### Switches
* Switches create networks
* reside in wiring closets and connect the computers in a building together
* Ethernet jacks are at the other end of network cables connected to switches
* Wireless access points connect to switches and create Wi-Fi networks
* Generally operate at Layer 2
* Some switches do have Layer 3 capabilities

### Routers
* Routers connect networks together
* router access control lists generally perform stateless inspections

### Bridges
* Layer 2 devices
* connect two networks together at Layer 2 using MAC Addresses

### Media Gateways
* Connect different telecommunications networks together

### Firewalls
* Firewalls act like security guards and block unwanted traffic
* Usually lie at the edge of a network
* Often connect three networks:
    * Internal Network
    * Internet
    * DMZ
* Stateful Inspection: tracks open connections
* Firewall Rules:
    * Source/destination system addresses
    * Port/Protocol
    * Action (allow or deny)
* Implicit Deny Principle: if traffic is not explicitly allowed, it will always be denied
    
### Demilitarized Zone (DMZ)
* Contains systems that must accept direct external connections
* Isolates those systems due to risk of compromise

### Web Application Firewall
* specifcially protect web applications by using applicaiton awareness that look deep into applicaiton layer

### Proxy Server
* Proxy server sits in the middle of the connection
* Anonymization
* Performance Boosting
* Content Filtering
* Forward proxies work on behalf of the client
* Reverse proxies work on behalf of the servers
* Transparent proxies: work without client of server's knowledge
* Proxies can handle many applications, not just web traffic

### Load Balancers
* Instead of the DNS entry pointing to the web server, it points to the load balancer, also known as the virtual IP
* Round-robin scheduling: each number gets an equal number of requests
* Advanced scheduling algorithms choose servers based on performance and ability
* They become a single point of failure
* High availability:
    * Active-Active: two or more load balancers actively handle network traffic
    * Active-Passise: one load balancer handlers all traffic and assumes responsibility, if primary fails

### Virtual Private Networks
* Site-to-Site VPNs
* Remote Access VPNs
* Use encryption to create a virtual tunnel
* VPN Endpoints:
    * Firewall
    * Router
    * Server
    * VPN Concentrator
* IPSec: network layer VPN protocol commonly used for site-to-site VPNs, difficult to configure
* SSL/TLS: application layer VPN protocol commonly used for remote access VPNs and easier to configure
* Full-Tunnel VPN: all network traffic leaving connected device is routed through the VPN Tunnel
* Split-Tunnel VPN: only traffic destined for the corporate network is sent through the VPN Tunnel
* Always-on VPN: connect automatically to VPN on corporate mobile devices

### IPSec
* Adds security to TCP/IP
* Secures the entire payload
* Encapsulating Security Protocol (ESP): provides confidentiality and integirty protection for packet payloads
* Authentication Headers (AH): Provides integrity protection for packet headers and payloads
* Security Associations (SAs): identify cryptographic algorithms
* Can be used to support VPNs

### Intrusion Detection and Prevention

### Intrustion Detection Systems
* Alert administrators to suspicious activity
* require someone to monitor and take appropriate action

### Intrusion Prevention Systems
* Block suspicious activity automatically

### Signature Detection System
* Contain databases with rules describing malicious activity
* Alert administrators to traffic matching signatures
* Fail to detect brand new attacks
* Reduce false positive rate

### Anomaly Detection Systems
* Builds a model of "normal" activity
* Alert administrators to activity not matching the model
* Detect previously unknown rate
* Increased false positive rate
* Also known as behaviour or hueristic detection

### IPS Development Modes
* In-band (inline) Deployments:
    * devices sits in the path of network communications
    * Device can block suspicious traffic from entering the network
* Out-of-band (passive0 Deployments:
    * Device connects to a SPAN port on a switch
    * Device can react after suspicious traffic enters the network

### Unified Threat Management
* combine multiple security functions into a single appliance

### OAuth and OpenID Connect
* OAuth: authorization protocol designed to work across a variety of web services
* OpenID Connect: identification and authentication protocol designed to work with OAuth