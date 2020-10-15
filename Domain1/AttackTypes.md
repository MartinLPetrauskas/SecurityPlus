## Attack Types

### Denial of Service (DOS) Attacks
* disrupts the normal use of computing resources
* sends a huge number of requests to a server so it cannot accept legitimate traffic
* requires a large amount of bandwidth
* easy to block IP based attacks
* Distributed Denial of Service (DDOS)
    * leverages botnets to execute the attack

### Smurf Attack:
* Utilizes "ping" command
* Attacker forges the source address in an echo request and all the replies focus on one victim
* Amplified DDoS attack: small requests, but the replies are large in comparison
* Amplification Factor: Reply Size / Request Size

### Eavesdropping Attacks
* rely on a compromised communications path
* Man-in-the-Middle
    * attacker is in-between the user and the server
    * Man-in-the-Browser: exploits a flaw in the browser or its plugin
* Replay Attack:
    * Utilizes previously captured packets/information and sends them again to the server
    * can be prevented with token, timestamps, etc.
    
### Network Attacks
* Christmas Tree Attack:
    * all flags are set in a packet
    * response can be used to fingerprint the OS

### DNS Poisoning
* attacker inserts incorrect DNS entries into the DNS servers

### ARP Poisoning
* attacker insert incorrect ARP entries onto the local area network
* Attacker needs to be on the local network to execute the attack

### Typosquatting (URL Hijacking)
* Attacker registers domains with typos and victims can end up visiting the fake sites

### Domain Hijacking
* Attacker attempts to steal or alter DNS registration records

### MAC Spoofing Attack
* Alters the hardware address of a device

### IP Spoofing
* Alters IP addresses
* Mainly used in Denial of Service attacks

### Preventing spoofing attacks
* Ingress Filtering: blocks incoming traffic from external network bearing an internal source address
* Egress Filtering: blocks outbound traffic for source IP addresses that you don't control

### Password Attacks
* Linux Systems store password hashes in the /etc/shadow file
* Passwords are usually hashed
* Types of Password Attacks:
    * Brute Force Attacks
    * Dictionary Attacks
    * Hybrid Attacks
    * Rainbow Table Attacks

### Hashing
* mathematical function which takes a variable length input and transforms it into a fixed-length output
* must be collision resistant

### Birthday Problem
* Collisions become common with large samples
* Birthday paradox

### Brute Force Attacks
* simplest attack against a cryptographic system
* repeatedly guess the key
* also called known-ciphertext attacks
* Keyspace: the set of all possible encryption keys usable with an algorithm
* modern algorithms aren't susceptible to brute-force attacks
* Flawed algorithms may be vulnerable to brute-force attacks

### Advanced Cryptographic Attacks
* Frequency Analysis: detect patterns in ciphertext, takes advantage of language information, such as the most common letters in the alphabet
* Known-Plaintext Attack: attacker has access to the unencrypted message
* Chosen-Plaintext Attack: attacker can create an encrypted message of their choice
* Downgrade Attacks: attacker forces two systems to use weak cryptographic protocols (i.e. POODLE attack)

### Watering Hole Attacks
* websites spread malware effectively
* Web browsers have add-ons which can be vulnerable
* Client-side attacks
* Uses commonly visited websites without the knowledge of the website owner