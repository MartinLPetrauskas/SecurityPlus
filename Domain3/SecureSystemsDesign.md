## Secure Systems Design

### Workstation OS
* Power laptop and desktop computers
* Typically Windows or macOS

### Server OS
* Designed for special purpose computer that provides services to others
* Windows Server OS
* Linux

### Mobile OS
* Designed for smartphones and tablets
* iOS
* Andriod
* Windows Mobile

### Kiosk Computer
* Device placed inside a specialized furniture and with limited functionality
* Operating systems depends on the hardware

### Kiosk Security
* Kiosk devices require the same types of security controls that you would deploy for their fully functioning counterparts
* You must also verify that the technology limiting kiosk functionality works properly

### Appliances
* Bundle together hardware and software to achieve a function
* Often run full operating systems
* Require vendor support for updates

### Network devices
* Run special purpose network operating systems
* Cisco IOS
* Juniper Junos OS

### Data Encryption
* Encryption protects data using algorithms and secrete keys
* Full disk encryption protects an entire hard drive
* Database encryption protects the contents of databases from attack
* Hardware encryption is more efficient than software encryption
* Hardware Security modules use dedicated hardware for encryption, decryption, and key management
* Trusted Platform Module (TPM) being hard encryption to typical computers

### Hardware & Fireware Security
* Operating systems must be loaded from disk during the boot process
* Basic Input/Output System (BIOS): lightweight operating system stored in firmware
* BIOS attacks may give malicious individual full control of a device
* Unified Extensible Firmware Interface (UEFI): replaces BIOS with a flexible alternative
* Secure Boot:
    * Read the boot loader from disk
    * Computers the hash of the boot loader
    * Decrypt the boot loader's digital signature
    * Verify that the signature is accurate
* Hardware Root of Trust
    * verifies firmware integrity
* Electromagnetic Interference (EMI): electromagnetic waves can cause disruption to nearby electronic equipment

### Peripheral Security
* Many wireless devices use the same Wi-Fi and Bluetooth protocols user by other computer systems, and they must be secure in the same way
* Removable storage devices create the risk of data theft by trust insiders
* Some storage cards create their own wireless networks
* Printer Security Practices:
    * Patch the operating systems
    * Secure the printer's webserver
    * Encrypt the print traffic
    * Securely wipe printer hard drives
    
### IT Automation
* Automation uses scripts to create servers treating infrastructure as code
* Typically start with a master image, but they can be customized with templates and script commands
* Benefits of Automating Server Builds
    * Consistency: Remove the human element
    * Elasticity: facilitate adding additional servers
    * Load Balancing: add and remove servers as needed
    * Scability: modify server configuration easily
    * Resiliency: rebuild servers from original script
* Distributive allocation also means load balancing

### Nonpersistence
* Nonpersistence: designed for failure
* Nonpersistent technologies:
    * Automated server builds
    * System snapshots
    * Reversion to a known state