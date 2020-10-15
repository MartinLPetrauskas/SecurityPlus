## Symmetric Cryptography

### Data Encryption Standard (DES)
* Designed by IBM in the 1970s
* Intended to serve as federal encryption standard
* Replaced untested algorithms used by agencies
* Enhanced interoperability of communications
* DES uses an encryption operation called the Feistel function for 16 rounds of encryption
* DES is no longer considered secure
* Ket Facts about DES:
    * Symmetric encryption algorithm
    * Block cipher operating on 64-bit blocks
    * Key length of 56 bits
    * Now considered insecure

### 3DES - Triple DES
* Applies DES to plaintext three times
* Triple DES applies DES three times with three keys: K1, K2, and K3
* DES Keying Options
    * K1 != K2 != K3
    * K1 = K3, K1 != K2, K2 != K3
    * K1 = K2 = K3
* Double DES is no more secure than standard DES due to the meet-in-the-middle-attack
* Key Facts about 3DES:
    * Symmetric encryption algorithm
    * Block cipher operating on 64-bit blocks
    * Effective key length of 112 bits

### AES, Blowfish, & Twofish
* The Rijndael algorithm won a competition to become the Advanced Encryption Standard (AES)
* AES uses subsitution and transposition
* Key Facts about AES:
    * Symmetric encryption algorithm
    * Block cipher operating on 128-bit blocks
    * Key lengths of 128, 192, or 256
    * Considered secure
* Blowfish
    * is a public domain algorithm
    * designed as a DES replacement
    * Uses a Feistel network
    * Combines substitution and transposition
* Key Facts about Blowfish:
    * Symmetric encryption algorithm
    * Block cipher operating on 64-bit blocks
    * Key length anywhere between 32 and 448 bits
    * Not considered secure
* Twofish:
    * Designed as a DES replacement
    * Placed into the public domain
    * Uses a Feistel network
    * Combines substitution and transposition
* Key Facts about Twofish:
    * Symmetric encryption algorithm
    * Block cipher operating on 128-bit blocks
    * Key lengths of 128, 192, or 256
    * Considered secure

### RC4
* RC4 was a trade secret from its invention in 1987 until its public disclourse in 1994
* RC4 and Network Encryption
    * Wired Equivalent Privacy (WEP)
    * Wi-Fi Protected Access (WPA)
    * Secure Sockets Layer (SSL)
    * Transport Layer Security (TLS)
* RC4 uses a pseudorandom keystream
* RC4 is no longer considered secure
* Key Facts about RC4:
    * Symmetric encryption algorithm
    * Stream cipher
    * Variable length key between 40 and 2048 bits
    * Not considered secure
    
### Cipher Modes
* Cipher mode: describes how an algorithm encrypts and decrypts data
* Electronic Codebook (ECB): encrypting the same block with the same key in ECB mode results in identical cipher text blocks
* Cipher Block Chaining (CBC):
* Counter Mode (CTR): 
* Galois/Counter Mode (GCM) adds authentication capability

### Steganography
* Steganography: hides data in large files
* Steganography often uses innocent looking high resolution images
* Images with embedded text may be posted in plain sight
    