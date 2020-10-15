## Authorization

### Understanding Authorization
* Least Privilege: an individual should only have the minimum set of privileges necessary to carry out his or her job functions
    * Limits the potential damage from an insider attack
    * Restricts the ability of an external attacker to leverage a compromised account
* Separation of Duties: Performing any critical business function should require the involvement of two or more individuals
* Privelege Creep: this is a situation that occurs when a user accumulates excess permissions after shifting job responsibilites one or more times
* Account reviews limit privilege creep: automated and manual checks verify that users only have appropriate authorization levels

### Mandatory Access Controls
* Access control system where the operating system enforces security policies that users may not modify
* Security-Enhanced Linux (SELinux) uses mandatory access controls

### Discretionary Access Control
* Access control system where permissions may be set by the owners of files, computers, and other resources

### Access Control Lists
* Resource owners set DAC permissions through the use of access control lists
* NTFS Permissions:
    * Full control grants complete authority over a resource
    * Read allows the user to read the file
    * Read & Execute also allows the user to execute an application
    * Write allows the user to create files and modify their contents
    * Modify adds the ability to delete files and also includes Read & Execute permissions

### Advanced Authorization Concepts
* Implicit Deny Principle: any action which is not explicitly allowed must be denied
* Role-Based Access Control: permissions are grouped together into functional roles and users are assigned to those roles
* Attribute-Based Access Control (ABAC): allows administrators to make access control decisions based upon characteristics of the user, object, and environment
* Location-Based Controls: limit access based upon geographic location
* Time of Day Restrictions limit the use of resources during certain hours

### Database Access Control
* SQL Server Authentication:
    * uses local database user accounts
* Windows Authentication:
    * Uses underlying server user accounts
* Mixed Authentication:
    * Uses both SQL Server and Windows authentication
* Role-Based Authorization: manages permissions through roles that are assigned to users by administrators
* Account-Based Authorization: managers permissions by making explicit permissions grants to each account

