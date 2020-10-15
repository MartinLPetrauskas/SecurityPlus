## Wireless Networking

### Wi-Fi
* Standards set by IEEE
* How devices communicate over wireless networks
* Replaces network cables with radio transmitters and receivers
* Wireless Access Points connect wireless networks to wired networks and the Internet
* Wifi signals travel over open airwaves and are subject to undetectable interception

### Wi-Fi Standards
* 802.11 (1997) allows 2Mbps communication
* 802.11b (1999) allows 11Mbps communication
* 802.11g (2003) allows 22Mbps communication
* 802.11n (2009) allows 600 Mbps communication
* 802.11ac (2014) allows 1+ Gbps communication

### Basic Wireless Security
* Service Set Identifiers (SSID): identify wireless networks
* Disabling SSID broadcasting hides networks in plain sight
* Mac filtering: filters Wi-Fi connections by devices
* VPNs can allow the secure use of insecure wireless networks

### WEP, WPA, and WPA2
* Encryption hides the contents of network communications from eavesdroppers
* No Encryption: insecure option that sends all wireless communication unencrypted
* Wired Equivalent Privacy (WEP): insecure encryption that is susceptible to attack
* Wi-Fi Protected Access (WPA): uses the Temporal Key Integrity Protocol (TKIP) to implement strong encryption
* Wi-Fi Protected Access v2 (WPA2): Uses CCMP to apply the Advanced Encryption Standard to wireless networks

### Wireless Authentication
* Preshared Keys (PSK): require entry of a password, which is then converted into a encryption key using PBKDF2
* Enterprise Authentication: uses a username and password, using the RADIUS protocol
    * Lightweight EAP: insecure protocol that relies on MS-CHAP
    * EAP: broad framework with many variants, some secure, some not so much
        * EAP-TLS: Uses Transport Layer Security to protect authentication sessions
        * EAP-TTLS: Uses Tunneled TLS to protect authentication sessions
        * EAP-FAST: Provides flexible authentication via Secure Tunneling (FAST) using a Cisco protocol
        * 802.1x uses EAP to provide access control
    * Protected EAP: Tunnels EAP inside an encrypted TLS session
    
### Wireless Signal Propogation
* Antenna-type influences signal patterns
    * Omnidirectional antennas send signals in all directions
    * Directional antennas direct all of the power from an access point in a single direction
    * Beamforming is an 802.11ac feature, like a virtual directional antennas
    * Optimal access points placement depends on building characteristics
* Site Surveys determine the best places for wireless access points

### Wireless Network Equipment
* Wireless Access Points
    * Fat Access Points: contain all the hardware and software needed to operate a wireless network
    * Thin Access Points: rely upon wireless controllers for configuration and to server as the "brains" of the network
    * Wireless controlls manage configurations, optimize performance and reduce interference amongs access points
* Wireless Scanners: search for rogue devices and access points on a network