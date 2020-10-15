## Software Development Security

### Development Methodologies
* Begin with business requirements and translate them into a design
* Quality software requires a quality design
* Waterfall Model
    * process is very rigid
* Spiral Model
    * Iterative process with four phases
* Agile Approach:
    * popular approach that is commonly used today
    
### Maturity Models
* Software Capability Maturity Model assesses an organizations software development practice

### Operations, Maintenance, and Change Management
* Software development is never finished
* Change Management
    * Request Control: manages, evaluates, and prioritizes inbound requests from customers
    * Change Control: grants permission for developers to make changes to application code
    * Release Control: moves the code from development environment into production
    
### DevOps
* Merging Development and Operations
* Build collaborative relationships
* Embraces automation
* Facilitates rapid release of code
* Provide a stable operating environment
* Infrastructure as Code: scripts the creation of resources

### Code Repositories
* Store software source code files
* Coordinate changes among multiple developers
* Perform version control
* Code repositories help avoid dead code

### Third-Party Code
* Libraries contain shared software code
* Software Development Kits (SDKs): provides programming resources
* Application Programming Interfaces: allow interaction with remote services
* Shared code creates shared security vulnerabilities

### Code Signing
* Digital signatures provide nonrepudiation
* Code signing: applies digital signatures to software
* Signing Code
    * Developer obtains a digital certificate
    * Developer creates a digital signatures for the code using the private key associated with the certificate
* Verifying Code Signatures
    * User downloads software
    * Operating system uses the certificates public key to validate the signature
    * OS verifies the signatures hash matches the code
    * OS verifies that the developer is trusted
    
### Database Security
* First Normal Form (1NF)
    * Create separate tables for different sets of related data
    * Provide a primary key for every table
    * Records may not have multivalued fields
    * Records in a table must have the same number of fields
* Second Normal Form (2NF)
    * Table must be in 1NF
    * Every non-key field must be a fact about the entire key
* Third Normal Form (3NF)
    * The table must be in 2NF
    * No non-key field may be a fact about another non-key field
* Use ecnryption to protect senesitve data stores in a database
* Obfuscation and camouflage hide the locations of sensitive information
* Stored Procedures protect against SQL injection

### Software Testing
* Verification and Validation
    * Software Model validation: are we building the right software?
    * Software verification: are we building the software right?
* Stress Testing
    * Uses automated script to verify system capacity
    * May be run internally or through a vendor
    * Verifies the system can handle the maximum expected load
    * Determines the maximum capacity of the system
* User Acceptance Testing (UAT): ensures software will work for users
* Regression Testing: checks for unexpected side effects

### Code Reviews
* Code review: use peer analysis to asses code
* Fagan inspections follows a formalized six-step code review process
* Most organizations use a less formal review process

### Code Tests
* Use technology to inspect software
* Static Tests: use automated techniques to analyze code for error and security flaws without executing it
* Dynamic Tests: Execute code to verify that it is functioning correctly and doesn't have security flaws

### Fuzzing
* Software testing techniques that feeds software many different input values in an attempt to cause an unpredictable state or unauthorized access
* Input source:
    * developer supplied input
    * developer supplied script
    * generation fuzzing
    * mutation fuzzing
    
### Code execution
* Interpreted code: computer executes the source code instructions as written by developer
* Compiled code: developer runs a compiler to covert source code into an executable file written in machine language
