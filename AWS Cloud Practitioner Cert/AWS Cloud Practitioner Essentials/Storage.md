## Block Storage
- Data divided into pieces called blocks
	- Data updated block by block -> whole file doesn't have to be changed
- Direct data access without file system layers
- Best for applications/databases needing fast, frequent updates
- Like physical hard-drive
- Can be encrypted, backed up, and modified without disruption

#### EC2 Instance Store
- Unmanaged
- high-performance block storage directly attached to EC2 instance for temp data
- No data-persistence

#### Elastic Block Store (EBS)
- Managed service
- Provided persistent block storage volumes for EC2 Instances
- Price measured in Input/output per second (IOPs)
- Snapshots can be restored in different regions
- Automatic replication in same availability zone

- Users are responsible for scheduling and managing regular EBS snapshots
	- Ensure that data within snapshots are encrypted
	- integrity
	- test restoration procedures

- Snapshots
	- Dealt via increments
	- Initial snapshot contains everything
	- Every snapshot after contains only things that have changed
###### Data Lifecycle Manager
- Can be used to automate EBS snapshots
- Schedule automatic snapshot creation
- Set retention policies
- Manage snapshot lifecycle
- Apply consistent backup policies
## Object Storage
- Object = data + unique ID + metadata
- Full rewrite rewrite requited to update and object
- Organized using buckets
- Best for large or infrequently changed files
- unlimited scalability

#### S3
- Fully managed scalable object storage service for storing and retrieving any amount of data from anywhere
- Stores data as objects
- Objects store in buckets
- Max object size = 5TB
- Unlimited bucket size
- Version objects
- Automatically redundant by AWS

###### S3 Security
- Everything private by default
- Bucket policies
- Presigned URLs
- S3 Access Points
- S3 audit logs

###### S3 Storage Classes
- Designed for different storage needs
- Mix and match classes

S3 Standard
 - general purpose storage
 - Default selection
 - Used for cloud apps, dynamic websites, content distro, mobile/gaming apps, big data analytics

S3 Intelligent-Tiering
- Useful if data has unknown or changing access patterns
- Stores objects in 3 tiers: frequent access, infrequent access, archive instant access
- Monitors access patterns of data and automatically moved data to most cost-effective tier

S3 Standard Infrequent Access (Standard-IA)
- Data that is access less frequently but require rapid access when needed
- High durability, throughput, low latency
- Low per-GiB storage and retrieval fee
- Store long-term backups, disaster recovery files, etc
- Uses 3 AZs

One Zone Infrequent Access (One Zone-IA)
- Stores data in single AZ
- For those seeking affordable storage for infrequently accessed data without high availability
- Storing secondary backups or easily recreatable data

Express One Zone
- Deliver consistent single-digit millisecond data access for most frequently accessed data and latency-sensitive apps
- High speed access up to 10x faster and requests costs up to 80% lower than standard

Glacier Instant Retrieval
- Archiving data that is rarely accessed and requires millisecond retrieval
- Cost savings up to 68% compared to Standard-IA
- Same latency and throughput performance as Standard-IA

Glacier Flexible Retrieval
- low-cost storage for archived data that's access 1-2 times/year
- Access data in as little as 1-5min using expedited retrieval
- Request bulk retrieval up to 5-12 hours at no additional cost
- For backups, disaster recovery, offsite data storage, when data occasionally retrieved in min

Glacier Deep Archive
- lowest-cost storage class
- Long term retention and digital preservation for data access 1-2 times/year
- Default retrieval time of 12hrs
- Retain data sets for 7-10 years or longer
- Highly regulated industries: financial services, healthcare, public sectors
###### S3 Lifecycle Configurations
 - Used to automate managing object storage tier configs
 - 2 types of actions
	 - Transition - Define when objects should transition to another storage class
	 - Expiration - Define wen objects expire and should be permanently deleted

## File Storage
- Cloud-based access through shared file systems
- Straightforward implementation without code changes
- Best for applications needing shared file access
	- CMS for example
- Accessible over networks so multiple users and apps can access the same data simutaneously

#### Elastic File System (EFS)
- Fully managed
- NFS file system for use with AWS and on-prem resources
- Multiple instances can read and write to EFS at the same time
- Linux file system
- Regional resource
- Scales automatically

###### Storage classes
Standard and Standard-IA
- Offer Multi-AZ resilience
- Higher costs

One Zone Classes
- Saves data in single zone

Archive Classes
- Data only access a few times a year or less
- Does not need sub-millisecond latencies
- 50% lower costs

###### EFS Data Lifecycle
- Create lifecycle policies that determine when and how files are transitioned
#### FSx
- Fully managed
- File storage services for popular file systems like windows, lustre, netapp ontap

## Other Categories

#### Storage Gateway
- fully managed
- Hybrid-cloud storage service
- Provides on-prem access to virtually unlimited cloud storage
- 3 types
	- S3 File Gateway
	- Volume Gateway
	- Tape Gateway

#### Elastic Disaster Recovery
- Fully managed
- Streamlines recovery of physical, virtual, and cloud servers

