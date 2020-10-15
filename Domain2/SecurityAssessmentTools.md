## Security Assessment Tools

### Protocol Analyzers
* Allows deep inspection of traffic
* Troubleshooting network issues
* Investigate security incidents
* Wireshark & tcpdump are popular protocol analyzers
* Both are built on the libpcap library

### Network Scanning
* network mapping detects active systems
* nmap is the most common network mapping tool
* Banner Grabbing: retrieves information over a network connection that explicitly identifies the operating system and version
* Network fingerprinting: analyzes details of network communication to find oddities particulat to a specific operating system and version

### Exploitation Framework
* Metasploit: most common exploitation framework

### Command-Line Network Tools:
* ping: uses ICMP to check if a system is up/available
    * ICMP Echo and ICMP Reply
    * Some systems don't respond to ping requests
* traceroute: determines the network path between two systems
    * tracert on Windows systems
* ifconfig/ipconfig: displays network configuration information
* Address Resolution Protocol: translates IP addresses used at the network layer and MAC addresses used at the ethernet layer
* arp: displays the arp cache
* netstat: displays network statistics 
* nc: opens raw network connections on Mac/Linux

### DNS Harvesting
* dig: performs DNS lookups on Mac and Linux systems
* nslookup: performs DNS lookups on Windows systems
* whois: discover ownership information about domains and IP addresses
* reverse whois: discovers domains associated with a name or email address