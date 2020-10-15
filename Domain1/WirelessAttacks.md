## Wireless Attacks

### Wireless Networking
* Governed by the IEEE 802.11 standard
* Uses plaintext Service Set Identifiers (SSID)
* Use "beaconing" to advertise other devices

### Wireless Security Concerns
* Encryption is paramount to wireless technologies

### Wireless Encryption Options
* No Encryption
* Wired Equivalent Privacy (WEP): uses a static key
* Wi-Fi Protected Access (WPA): uses a Temporal Key Integrity Protocol (TKIP)
* Wi-F- Protected Access v2 (WPA2): uses Advanced Encryption Standard (AES) via CCMP

### Hacking WEP
* Initialization Vector is sent unencrypted
* Can be brute forced
* WEP attacks rely on capturing initialization vectors (IVs)

### Hacking WPA
* relies on RC4 encryption standard
* Uses RC4 with a 128-bit but adds a TKIP
* Changes key constantly
* Some theoretical attacks exists such as injection attacks

### Wi-Fi Protected Setup (WPS)
* WPS allows quick setup of deviced
* Two methods of establishing connection
    * Pressing button on device
    * Use 8-digit WPS PIN
* Flaws in WPS make it trivial to guess the WPS PIN

### Propogation Attacks
* Jamming and Interference attacks: denial of service on wireless devices
* War Driving:
    * attackers will cruise neighborhoods and commercial areas to capture information about Wi-Fi networks
    
### Rogue Access Points
* An access point that is not part of the authorized network topology
* Can interfere with legitimate wireless traffic

### Evil Twin Attacks
* When a rogue access point has the same SSID as a legitimate access point
* Can be automated with the Karma Toolkit

### Disassociation Attacks
* 802.11 standard has a deauthentication frame which will disconnect a client from a wireless network
* Deauth frames can be spoofed by using the MAC address of the access point
* Attack can be repeated numerous times

### Near Field Communication (NFC) Attacks
* Used for very short ranges, commonly used in Bluetooth
* Bluejacking: attacker send Bluetooth spam to a user's device, essentially a spam/phishing attack
* Bluesnarfing: attacker forces pairing between devices, connection grants access to the device

### RFID Security
* Businesses want strong authentication and encryption to protect integrity of RFID systems
* Consumers want privacy safeguards to protect personal information