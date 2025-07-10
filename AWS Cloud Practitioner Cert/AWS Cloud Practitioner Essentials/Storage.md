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

#### Elastic Block Store (EBS)
- Managed service
- Provided persistent block storage volumes for EC2 Instances
- Price measured in Input/output per second (IOPs)

## Object Storage
- Object = data + unique ID + metadata
- Full rewrite rewrite requited to update and object
- Organized using buckets
- Best for large or infrequently changed files
- unlimited scalability

#### S3
- Fully managed scalable object storage service for storing and retrieving any amount of data from anywhere

## File Storage
- Cloud-based access through shared file systems
- Straightforward implementation without code changes
- Best for applications needing shared file access
	- CMS for example
- Accessible over networks so multiple users and apps can access the same data simutaneously

#### Elastic File System (EFS)
- Fully managed
- NFS file system for use with AWS and on-prem resources

#### FSx
- Fully managed
- File storage services for popular file systems like windows, lustre, netapp ontap

## Other Categories

#### Storage Gateway
- fully managed
- Hybrid-cloud storage service
- Provides on-prem access to virtually unlimited cloud storage

#### Elastic Disaster Recovery
- Fully managed
- Streamlines recovery of physical, virtual, and cloud servers

