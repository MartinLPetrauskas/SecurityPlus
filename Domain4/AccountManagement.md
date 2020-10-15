## Account Management

### Understanding Account and Privilege Management
* Implement least privilege
* Implement separation of duties
* Implement job rotation
* Manage account life cycle
* Least Privilege: users should have only the minimum set of permissions necessary for their job function
* Separation of Duties: sensitive functions should require action by two separate users
* Job Rotation: regularly move people between jobs to prevent fraud
* Mandatory Vacation: enforce periods of time when employees have no access to systems

### Account Types
* User Accounts: have standard permissions and standard monitoring
* Privilege Accounts: have administrator rights and require strong controls
* Privileged accounts should not be used for routine activities
* Guest Accounts: have limited permissions and temporary lifetimes
* Shared Accounts: reduce accountability and should not be used
* Service Accounts: provide access for internal server processes

### Account Policies
* Group Policy Objects (GPO): apply configuration settings to users and computers

### Password Policies
* Prevent password guessing
    * password length: at least 8 characters
    * password complexity: include other characters like numbers, symbols, etc.
* Password expiration:
    * every X amount of days
* Password History and Reuse:
    * keeps track of previous passwords
* Account lockout after several incorrect password attempts
* Password recovery mechanisms

### Managing Roles
* Roles Group Permissions allow sharing of security settings
* Roles simplify account management
* Roles eliminates dangers of shared and generic accounts

### Account Monitoring
* Account Security Issues:
    * Inaccurate permissions
    * Illegitimate account use
* User Access Reviews:
    * Pull listing of user permissions
    * Review permissions with managers
    * mane an necessary adjustments
    * Focus on users who recently changed roles

### Provisioning and Deprovisioning of Accounts
* Provisioning: after onboarding, administrators create authentication credentials, and grant appropriate authorizations
* Deprovisioning: during the offboarding process, admins disable accounts and revoke authorizations
