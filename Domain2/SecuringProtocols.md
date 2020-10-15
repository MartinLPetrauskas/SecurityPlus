## Securing Protocols

### TLS
* Transport Layer Security (TLS): encrypts network communications
* TLS depends upon pairings of encryption and hash functions known as cipher suites
* Session Keys are also known as ephemeral keys

### SSL
* Insecure predecessor to TLS

### Protocol Security Use Cases
* Voice and video communications should leverage TLS encryption whenever possible
* RTP-based VoIP services should use secure RTP (SRTP)
* Network Time Protocol (NTP): NTPSec is the more secure version of NTP
* Email Protocols:
    * POP: Unsecure 110, Secure 995
    * IMAP: Unsecure 143, Secure: 993
    * SMTP: Unsecure 25, Secure 465
* Encrypt email messages and attachments with S/MIME
* Networking Protocols:
    * Use SSH instead of Telnet
    * Use SNMPv3 instead of the older versions
* Use DNSSEC to add digitial signatures to DNS
* LDAPS offters a secure alternative to LDAP

### Securing Common Protocols
* Use HTTPS over HTTP, HTTPS adds TLS to web browsing
* Telnet uses insecure command-line access, SSH is a secure alternative
* FTP is insecure
    * FTP Secure (FTPS): adds TLS to FTP
    * SFTP transfers files over SSH
    * Secure SCP: uses SSH
    * TFTP is rarely used and is not secure

### Cryptographic Hardware
* SSL/TLS accelerator: provides dedicated hardware for SSL/TLS handshakes
* Encryption can make it difficult to perform intrusion detection and data loss prevention
* SSL/TLS decryption: performs a man-in-the-middle attack against local users
* Many firewalls perform SSL/TLS decryption
* Hardware Security Modules (HSM): manage encryption keys and perform cryptographic operations
    * HSMs are expensive, but are extremely effective