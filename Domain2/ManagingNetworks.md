## Managing Secure Networks

### Firewall Rule Management
* Rules define how the firewall should act when it sees a new connection request

### Configuration Errors on Firewalls
* Shadowed rules
* Promiscuous rules allow more access than necessary
* orphaned rules allow access to decommissioned systems and services

### Router Configuration Security
* Can reduce the load of firewalls by filtering traffic
* Makes use of standard and extended access control lists

### Switch Configuration Security
* An attacker who gains physical access to your switch controls that portion of the network
* VLANs increase security
    * VLAN Pruning
    * VLAN Trunk Negotiation
    * Port Security
        * Static Mode: configure valid MAC addresses for each port
        * Switches memorize the first MAC address they see on each port and limit access to that port
        
### Maintaining Network Availability
* SYN Flood: fill connection state tables on firewall with half-open connection entries
* MAC Flood: Fill switch's MAC address table with many entries causing it to flood traffic on all ports
* Flood Guard technology: protects network devices about flood attacks

### Network Monitoring
* Firewall logs contains many details about connections such as time, source/destination IPs, firewall rules
* Security Information and Event Managament (SIEM): aggregates logs from multiple systems
* SIEMs facilitate rapid analysis

### Simple Network Management Protocol (SNMP)
* Managing network devices manually is impractical
* SNMP automates these tasks
* Use SNMPv3, earlier versions are insecure as they send information unencrypted

### Storage Networks
* Network Attached Storage: simple self-contained storage devices
* Storage Area Networks: complex massive storage
    * SANs present raw storage to devices rather than file systems
    