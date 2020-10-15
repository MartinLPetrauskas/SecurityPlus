## Host Security

### Operating System Security
* OS Security it critical
* compromised systems are a gateway attack
* Security settings
* Windows has group policy objects to control security settings
* Patch Management: operating systems should install updates promptly
* System hardening: locking down configurations
    * remove unnecessary software and operating system components
    * lock down the host firewall configuration
    * disable default accounts and passwords
    
### Malware Prevention
* Viruses: spread by human action
* Worm: spread by themselves
* Trojan Horses: disguise themselves
* Spyware: gathers information
* Antimalware software protects against many different threats
    * Signature detection: watches for known patterns of virus activity
    * Behavior detection: watches for deviations from normal patterns of activity
    * Sandboxing: executes suspicious code in a safe environment where is is monitored for malicious activity
    
### Application Management
* Application control: restricts software that may run on a system
    * Whitelisting: admins create a list of all the applications that can be run
    * Blacklisting: admins create a list that are prohibited applications

### Host-Based Network Security Controls
* Default Deny Principle
* Network Firewalls: hardware devices that regulate connections between two networks
* Host-Based Firewalls: software components of an operating system that limit connections to a server

### File Integrity Monitoring
* Defense in depth require the use of diverse, overlapping security controls
* watches for unexpected file modifications
* Hash functions are one-way functions that transform a variable length input into a unique fixed-length output
* File integrtiy monitoring systems periodically verify that the hash value of critical files have not changed

### Removable Media Control
* Limit the use of removable media
* Track the use of removable media, when it connects, disconnects, etc. 

### Data Execution Prevention (DEP
* Microsoft technology that enforeces specific restrictions on the acceptable locations for executable code
