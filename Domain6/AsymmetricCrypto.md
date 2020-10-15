## Asymmetric Cryptography

### Rivest-Shamir-Adleman (RSA)
* Users create RSA key pairs using two large prime numbers
* User distributes the public key freely and keeps the private key secure
* RSA Keys:
    * Sender encrypts a message using the recipient's public key
    * Recipient decrypts a message using the recipient's private key
* RSA: transfer symmetric keys
* RSA: patent is now expired
* Key Facts about RSA
    * Asymmetric encryption algorithm
    * Variable length keys between 1024 and 4096 bits
    * Considered secure

### PGP and GnuPG
* Phil Zimmerman created Pretty Good Privacy in 1991
* PGP is widely available today through the open PGP standard
* PGP Function:
    * Use public and private keys
    * Combines both symmetric and asymmetric cryptography
* PGP relies upon other encryption algorithms

### ECC and Quantum Cryptography
* Asymmetric cryptography is based upon the difficulty of solving complex math problems
* Elliptic Curve cryptography: uses the EC discrete log problem, does not use prime factorization
* Quantum Computing: uses quantum mechanics principles
* Quantum cryptography may be stronger than any modern approach

### Tor and Perfect Forward Secrecy
* Tor: The Onion Router (TOR) is a software package that uses encryption and relay notes to facilitate anonymous Internet access
* Perfect Forward Secrecy: hides nodes identity from each other
* 