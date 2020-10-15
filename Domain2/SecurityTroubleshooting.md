## Security Troubleshooting

### Troubleshooting Authentication and Authorization
* the use of unencrypted credentials is a serious security issue
* replace unencrypted protocols
* VPNs and SSH tunnels add security to insecure protocols
* permission issues require careful troubleshooting

### Troubleshooting Digital Certificates
* don't ignore certificate errors
* expired certificates: requires renewal
* mismatched names: indicates a serious issue and it may be using an incorrect certificate
* untrusted CAs: only trust certificates from well known certificate authorities
* revoked certificates: should not be trusted, the certificate was probably compromised
* cryptographic errors: usually related to which protocols are being used

### Troubleshooting Device Configuration
* patch devices regularly
* avoid weak cryptography
    * avoid DES, RC4
    * avoid MD4, MD5, SHA-1
* disable default accounts

### Change and Configuration Management
* change is good, but it must be controlled
* change management ensures that organizations follows a standardized process for requesting, reviewing, approving, and implementing changes to information systems
* Request For Change (RFC)
* baselines: provides a configuration snapshot

### Physical Asset Management
* build an asset inventory: integrate it with other processes
* data updates are critical
* media managagement tracks highly sensitive data