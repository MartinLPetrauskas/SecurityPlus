## Cloud Computing

### Virtualization
* Data centers leverage virtualization technology
* Host machines run on physical hardware
* Host machines provide services to several virtualized guest machines
* Hypervisor tricks each guest into thinking it is running on dedicated hardware
* Two different types of hypervisors
* Virtual machine isolation is critical
* Each server must have access to only its own memory and storage
* VM escape attacks attempt to break out of the guest environment
* VM sprawl: leads to unused and unmaintained servers

### Cloud Computing Models
* Cloud computing is the next logical advance in enterprise IT
* Cloud computing: delivery of computing resources as a service over a network
* Private Cloud: organization uses a dedicated cloud infrastructure
* Public Cloud: organizations uses a shared tenancy infrastructure
* Hybrid Cloud: organizations uses both private and public cloud
* No one cloud model is better than the others

### Public Cloud Tiers
* Software as a Service (SaaS):
    * Customter purchases an entire app, i.e. Google Drive
* Platform as a Service (PaaS):
    * Customer purchases app platform, i.e. AWS Lambda
* Infrastructure as a Service (IaaS):
    * Customer purchases server/storage, i.e. AWS, Google Computer, Microsoft Azure
* There are varying security responsibilites for the public cloud tiers

### Cloud Storage Security
* Encryption and access control are big security issue for the cloud

### Security Service Providers
* Managed Security Service Providers (MSSPs): provide security services for other organizations as a managed service
* MSSPs must be carefully monitored
* MSSP Service Examples:
    * Manage an entire security infrastructure
    * Monitor system logs
    * Monitor firewalls or networks
    * Perform identity and access management
* MSSPs may also be referred to as Security as a Service (SECaaS)
* Cloud Access Security Brokers (CASBs): add a third-party security layer to the interactions that users have with other cloud services
    * Network-Based CASB: broker intercepts traffic between the user and the cloud service, monitoring for security issues, broker can block requests
    * API-Based CASB: broker queries the cloud service via API, broker may not be able to block requests depending on API capabilities

### Desktop and Application Virtualization
* Virtual Desktop Infrastructure: provide network-based access to a desktop computing environment
* Application virtualization allows users to "stream" application to their desktop
* Containerization: runs multiple apps on the same operating system with restricted resource access
* Application cells refer to containers