## Public Key Infrastructure (PKI)

### Trust Models
* Requirements for Key Exchange
    * The two parties must be confident that they are really communicating with each other and neither one is an imposter
    * The two parties must be confident that nobody is eavesdropping on the key exchange
* Asymmetric Cryptography
    * Users don't need to share their private keys
    * Users can and should share their public keys freely
    * Eavesdropping protection isn't needed during the key exchange
    * We still need to prevent imposters
* Trust Knowledge
    * Personal Knowledge
    * Web of Trust (WOT): relies on indirect relationships, participants digitally sign the public keys of people they know personally
    * Public Key Infrastructure (PKI)
    
### PKI & Digital Certificates
* PKI depends upon trusted certificate authorities (CAs)
* Certificate Authorities: trusted third party organizations who verify the identity of individuals or organizations and then issue digital ertificates containing both identity information and a copy of the subject's public key
* Digital certificates are the identity cards of the digital world
* After authenticated identity, the CA provides a digital certificate containing the public key
* Anyone trying to use your digital certificate illegitmately won't have your private key

### Hash Functions
* Hash Function: one-way function that transforms a variable length input into a unique fixed-length output
* One-way functions can't be reversed
* The output of a hash function will always be the same length, regardless of the input size
* No two inputs to a hash function should produce the same output
* Hash functions may fail:
    * If they are reversible
    * if they are not collision resistant
* Message Digest 5 (MD5):
    * Ron Rivest created MD5 in 1991
    * MD5 is the fifth in a series of hash functions
    * Message digest is another term for hash
    * MD5 produces 128-bit hashes
    * MD5 is no longer secure
* NIST created the Secure Hash Algorithm (SHA) family as a government standard
* SHA-1
    * Produces a 160-bit hash value
    * Contains flaws that render is insecure
* SHA-2
    * Consists of a family of six hash functions
    * Produces output of 224, 256, 384, and 512 bits
    * Uses a mathematically similar approach to SHA-1 and MD5
* SHA-3
    * Designed as an eventual replacement for SHA-2
    * Uses a completely different hash generation approach than SHA-2
    * Produces hashes of user-selected fixed length
* RIPEMD:
    * Created as an alternative to government-sponsored hash functions
    * Produces 128, 160, 256, and 320 bit hashes
    * Contains flaws in the 128 bit hash
* HMAC:
    * Hash-Based Message Authentication Code
    * Combines symmetric cryptography and hashing
    * Provides authentication and integrity
    * Create and verify message authentication code by using a secret key in conjunction with a hash function
* Hash functions are used with asymmetric cryptography for digital signatures and digital certificates

### Digital Signatures
* Digital Signatures use asymmetric cryptography to achieve integrity, authentication, and non-repudiation
* What Signed Message Recipients Know
    * The owner of the public key is the person who signed the message
    * The message was not altered after being signed
    * The recipient can prove these facts to a third party
* What Digital Signatures Depend On
    * Collision-resistant hash functions
    * Asymmetric cryptography
* Use private keys to create digital signatures
* Digitally signing messages does not provide confidentiality

### Digital Signature Standard
* Approved DSS Algorithms
    * Digital Signature Algorithm (DSA)
    * Rivest, Shamir, Adelman (RSA)
    * Elliptic Curve Digital Signature Algorithm (ECDSA)
    
### Create a Digital Certificate
* Digital certificates use the X.509 standard
* Uses a Cetificate Signing Request (CSR) to request a certificate from a CA

### Revoking Digital Certificates
* Certificate Revocation List (CRL): CAs provide a list of the serial numbers of revoked certificates
* Online Certificate Status Protocol (OCSP): CAs provide a real time service that allows users to verify that a certificate is not revoked
* Most modern browsers implement OCSP

### Certificate Stapling
* OCSP places a significant burden on the OCSP server operated by certificate authorities
* Certificate Stapling: reduces the CAs burden

### Certificate Authorities
* You must pay a fee to the CA to obtain a trusted certificate
* Self-Signed Certificates: issues by an internal CA
* Certificate chaining allows the use of intermediate CAs
* Offline CAs: protect sensitive root keys

### Certificate Subjects
* Certificate subject: owner of the public key
* Certificate Object Identifiers (OID)
* Certificate Subjects
    * Servers (web, SSH, file, etc.)
    * Devices (SAN, routers, switches, etc.)
    * Individuals (Names, email addresses)
* Certificate Pinning: ties a certificate to a subject for a period of time

### Certificate Types
* Root Certificates: protect CA private keys
* Wildcard Certificates: match an entire domain
    * Commonly used for load balancers
* CAs issuing certificates are vouching for the certificate sender's identity
* Domain Validation (DV): verify domain ownership
* Organizational Validation (OV): verify business name
* Extended Validation (EV): require extensive investigation 

### Certificate Formats
* Distinguished Encoding Rules (DER):
    * Binary Format
    * Use .DER, .CRT, and .CER file extensions
* PEM Certificates
    * Name comes from outdates Privacy Enhanced Mail (PEM) standard
    * ASCII text equivlanet of DER
    * Convert with opensll
    * Use .PEM and .CRT extensions
* .CRT files may either either DER binary certificates or PEM text certificates
* Personal Information Exchange (PFX):
    * Binary format
    * Commonly used by Windows systems
    * Use .PFX or .P12
* P7B Format
    * ASCII text equiavlent of PFX certificates
    * Commonly used on Windows systems
    * Use >P&B file extension