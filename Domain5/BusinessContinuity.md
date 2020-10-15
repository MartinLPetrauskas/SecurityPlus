## Business Continuity

### Business Continuity Planning
* Business Continuity Planning: a set of controls designed to keep a business running in the face of adversity, whether natural or manmade
* Defining BCP Scope:
    * Business activities
    * Systems
    * Controls
* Business Impact Assessment (BIA): Identifies and prioritizes risks
* Risk Assessment Factors:
    * Impact on life and safety
    * Impact on property and finances
    * Impact on reputation
* Risk assessments should include environmental and man-made threats from internal and external sources

### Business Continuity Controls
* Redundancy protects against the failure of a single component
* Single Point of Failure Analysis: Identifies and removes SPOFs
* SPOF analysis continues until the cost of addressing risk outweighs the benefit
* Remember to perform succession planning for staff as well

### High Availability & Fault Tolerance
* High Availability (HA): uses multiple systems to protect against service failures
* Fault Tolerance (FT): makes a single system resilient against failing
* Load Balancing: spreads demand across systems, not exactly high availability
* Common Points of Failure:
    * Power supply
    * Storage media
* Redundant Array Of Inexpensive Disks (RAID):
    * RAID 1: disk mirroring, stores the same data on two different disks
    * RAID 5: disk striping with parity, uses three or more disks to store data and parity information
* Network Quality of Service (QoS): provides critical services with protected network capacity

### Disaster Recovery
* Disaster recovery capabilities are designed to restore a business to normal operations as quickly as possibly, subset of business continuity
* Initial Response:
    * Contain the damage
    * Recover whatever capabilities can be immediately restored
    * Include a variety of activities depending upon the nature of the disaster
* Employee responsibilities will changes dramatically during disaster recovery
* Disaster Communications:
    * Initial activation of the disaster recovery team
    * Regular status updates
    * Tatical communications
* After the danger passes, the team shifts to assessment mode
* Order of Restoration: should prioritize systems of critically
* Recovery Time Objective (RTO): maximum amount of time that it should take to recover a service after a disaster
* Recovery Point Objective (RPO): maximum time period from which data may be lost in the wake of a disaster

### Backups
* Backups provide a data "safety net"
* Backup Media:
    * Tape backups
    * Disk-to-disk backups
    * Cloud backups
* Backup Tyoes:
    * Full Backups: include a complete copy of all the data
    * Differential Backups: include all data modified since the last full backuo
    * Incremental Backups: include all the data modified since the last full or incremental backup
* Snapshots: capture system state at a moment in time

### Disaster Recovery Sites
* provide alternate data processing
* Disaster Recovery Facility Types
    * Hot site: fully operational data center, stocked with equipment and data, available at a moments notice
    * Cold site: Empty data centers, stocked with core equipment, network, and environmental controls, relatively inexpensive
    * Warm site: stocked with all necessary equipment and data, not maintained in parallel fashion
* Store backups at an offsite location
* Alternate business processes add flexibility in the wake of a disaster

### Geographic Considerations
* Backups serve as the last line of defense for data protection
* Backups should be stored in data centers unlikely to be affected by the same disaster as the primary facility
* Redundant data centers should also be geographically distant from primary facilities
* Data Sovereignty: data is subject to the law of the jurisdiction where it's stored

### Testing BC/DR Plans
* DR Testing Goals:
    * Validate that the plan functions correctly
    * Identify necessary plan updates
* DR Test Types:
    * Read-through: ask each member to review their role in the disaster recovery process and provide feedback
    * Walk-through: gather the team together for a formal review of the disaster recovery plan
    * Simulation: simulations use a practice scenario to test the disaster recovery plan
    * Parallel test: activate the disaster recovery facility but do not switch operations there
    * Full interruption test: switches primary operations to the alternate facility and can be disruptive to business

### After Action Reports
* after action reports create a formal record of disaster recovery (DR) or business continuity event
* Conduct after action reviewed after every BC or DR event, even those that are considered successful
* Provide enough background to allow the reader to understand the context
* Answer all the key factural questions around the event
* Include lessons learned during the response
* Conclude with clear next steps