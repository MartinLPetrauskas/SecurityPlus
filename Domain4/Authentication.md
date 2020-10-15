## Authentication

### Authentication Factors
* Three types of authentication factors
    * Something you know:
        * Normally a password
        * Strong passwords are long and complex
        * Passphrases are better than passwords
    * Something you are:
        * Biometric authentication
            * fingerprints
            * eye scans
            * facial recognition
            * voiceprints
    * Something you have:
        * Requires phyiscal possession of a device
            * smartphone with authentication app
            * Authentication key fob
* False Acceptance: system misidentifies an individual as an authorized user, measured by the false acceptance rate (FAR)
* False Rejection: system fails to recognize an authorized user, measured by the false rejection rate (FRR)
* Crossover Error Rate (CER): when FAR equals FRR

### Multifactor Authentication
* Combines authentication techniques from two or more of the authentication categories

### Something You Have
* OTP: one time passwords
    * HMAC-OTP: shared secret and incrementing counter
    * T-OTP: shared secret and based on the time of day
    
### Password Authentication Protocols
* Password Authentication Protocol (PAP): earliest version, both client and server know the password
* Challenge Handshake Authentication Protocol (CHAP): secure version of PAP
    * MS-CHAP and MS-CHAPv2 are insecure
    
### Single Sign-On and Federation
* Federated Identity Management
    * Individuals may have accounts across multiple systems
    * Federated identity management systems share identity information
    * This reduces the number of individual identities a user must have
* Single Sign-On (SSO): authentication system that shares a single authentication session across multiple systems avoiding asking users to log in multiple times
* One-Way Trust: Domain 1 trusts Domain 2 but Domain 2 does not trust Domain 1
* Two-Way Trust: Domains 1 and 2 trust each other
* Transitive Trust: trust relationships transfer across domains
* Non-Transitive Trust: trust relationships do not transfer between domains

### RADIUS and TACACS
* RADIUS: Remote Access Dial-In User Service, RADIUS client is usually an application server
* RADIUS Disadvantages:
    * Use unreliable UDP
    * Does not encrypt the entire authentication sequence
* TACACS: Terminal Access Controller Access Control System
    * TACACS+: current version that works today
        * Functions similarly to RADIUS
        * Uses TCP
        * Encrypts full authentication session
        
### Kerberos & LDAP
* Kerberos: ticket based authentication system that allows users to authentication to a centralized service and then use tickets to gain access to distributed services
* Lightweight Directory Access Protocol (LDAP): provides the means to query a centralized directory service, such as Microsoft Active Directory
* Kerberos uses port 88
* LDAP uses 389
* Secure LDAP uses 636
* NTLM Authentication: was widely used on Windows services for many years
    * Used weak encryption
    * Vulnerable to pass the hash attack

### SAML
* Security Assertion Markup Language (SAML): allows SSO within a web browswer across a variety of systems
* SAML Authentication:
    * End user is known as the principal
    * Identity Provider (IdP)
    * Service Provider
* SAML Benefits:
    * True SSO experience for end users
    * No credential access for service providers

### OAUTH and OpenID Connect
* OAUTH Providers
    * Linkedin
    * Facebook
    * Amazon
    * Etc.
* OUATH: authorization protcol designed to work across a variety of web services
* OpenID Connect: identification and authorization protocol design to work with OAuth

### Certificate Based Authentication
* Digital certificates contain a signed copy of a user's public key
* Key-Based Authentication:
    * Create a public/private keypair
    * Steps:
        * Connection Request
        * Random Challenge Message
        * Challenge Encrypted with Private Key
        * Connection Authenticated
* Key based authentication may be automated
* Certificate authorities create digital certificates for public keys used in authentication
