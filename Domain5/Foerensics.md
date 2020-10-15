## Forensics

### Conducting Investigations
* Investigation Types:  
    * Operational investigations: look into technology issues
        * Seek to resolve technology issues
        * Restore normal operations as quickly as possible
        * Use very low standards of evidence
        * Involve root cause analysis
    * Criminal investigations: look into possible crimes
        * Involve the possibility of fines and jail time
        * Use the "beyond a reasonable doubt" standard of evidence
    * Civil investigations: resolve disputes between parties
        * Do not involve the possibility of fines or jail time
        * Use the "preponderance of the evidence" standard
    * Regulatory investigations: are conducted by the government
* Interviews are a valuable tool available to investigators
* Cybersecurity investigators should leave interrogations to law enforcement

### Evidence Types
* Evidence Types
    * Real evidence: consists of tangible objects
    * Documentary evidence: consists of written information
        * Authentication rule: documents must be authenticated by testimony
        * Best evidence rule: original documents are superior to copies
        * Parol evidence rule: written contracts are assumed to be the entire agreement
    * Testimonial evidence: consists of witness statements
        * Direct evidence: witness provides evidence based upon his or her own observations
        * Expert Opinion: expert witness draws conclusions based upon other evidence
        * Testimonial evidence may not consist of hearsay
        
### Intro to Forensics
* Digital Forensics: investigation techniques that collect, preserver, analyze, and interpret digital evidence
* Investigations must never alter evidence
* Volatility: the relative permanence of a piece of evidence: evidence that may not last long is more volatile than more permanent sources of evidence
* Order of Volatility:
    * Network Traffic
    * Memory contents
    * System and process data
    * Files
    * Logs
    * Archived records
* Time offsets help correlate records from different sources
* Alternate Evidence Sources
    * Video recordings
    * Witness statements
* Track your use of time and resources
* Recovery and preservation of evidence are the core tasks of digital forensics

### System & File Forensics
* Investigations must never alter evidence
* Images take the place of original physical media
* Write blockers, also known as forensics disk controllers, prevent accidental modifications of disks during images
* Hashes protect evidence: they provide a unique file signature
* Use hashes to demonstrate that a file hasn't been altered
* Other Forensics Sources:
    * Screenshots
    * Memory Contents
    * Process Table
    * Operating system configuration
* Never try to perform forensics yourself unless you've received approriate training

### Network Forensics
* Ethernet networks send electrical pulses over copper wire
* Fiber-optic networks send light pulses over strands of glass
* Wireless network send pulses over radio waves
* Network communications may be intercepted
* NetFlow summarizes traffic
* Routers and firewalls capture netflow data

### Software Forensics
* Intellectual Property: software forensics may be used to resolve intellectual property disputes between two parties
* Malware Origins: software forensics may be used to identify the author of malicious software found on a system

### Embedded Device Forensics
* embedded devices: special purpose computers found inside smart devices found in homes, businesses, and industrial settings
* Vehicles often contain many embedded devices with valuable forensic information

### Chain of Custody
* Chain of Custody: provides a paper trail for evidence
* Evidence should be labeled and stored in a sealed evidence container
* Evidence Log Events:
    * Initial collection
    * Transfer
    * Storage
    * Opening and resealing the container
* Envidence Log Entry Details:
    * Investigator name
    * Date & Time
    * Purpose
    * Nature of action
    
### Electronic Discovery
* Three major steps in electronic discovery
    * Preservation
    * Collection
    * Production
* litigation holds require the preservation of relevant electronic and paper records
* System administrators must suspend the automatic deletion of relevant logs
* Security teams often assist in collection efforts
* Source of Electronic Records:
    * File servers
    * Endpoint systems
    * Email messages
    * Enterprise systems and cloud services
* Electronic discovery management system coordinate collection efforts

