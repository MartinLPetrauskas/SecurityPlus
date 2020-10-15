## Key Management

### Key Exchange
* symmetric cryptography required exchanging a shared secret key in advance
* Out-of-Band Key exchange: uses a different channel
* Out-of-band Options:
    * Face-to-face meeting
    * Physical mail
    * Telephone call
* Out-of-band key exchange is difficult and time consuming
* In-Band Key Exchange: securely exchange keys digitally

### Diffie-Hellman
* Ralph Merkle's work formed the basis of the Diffie-Hellman algorithm
* Whitfield Diffie and Martin Hellman created the Diffie-Hellman key exchange (DHE) algorithm
* Elliptic Curve Diffie Hellman (ECDHE): uses elliptic curve problem

### Key Escrow
* Encryption Key Escrow: allows government access to keys
* The Cipper Chip included technology that would allow government access to encrypted communications
* Privacy advocated and industry firms fought strongly against the Cliiper Chip
* Recovery Agents: allows internal access to lost keys

### Key Stretching
* Key Stretching: takes a relatively insecure value, and uses mathematical techniques to strengthen it, making it harder to crack
* Salting: adds a value to the encryption key to make it more complex
* Hashing: adds time to the verification process requiring more math
* Verifying one key is fast, but guessing millions of keys is slow
* PBKDF2: Passwrod-Based Key Derivation Function v2
    * Uses salting and hashing to stretch a key
    * Should be used at least 4,000 times
* bcrypt: key stretching with Blowfish

