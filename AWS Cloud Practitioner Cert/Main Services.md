EC2
- Elastic Compute Cloud
- Combination of processor and ram
- IaaS
- Can use any software version you need
- Use Cases
	- hosting apps/websites
	- Dev/test environments
	- Disaster recovery
	- Performance Computing
	- Data Analytics
	- In-memory DB
	- Machine Learning/AI
	- Graphics workloads and video rendering
- Config options
	- OS
	- CPU
	- RAM
	- Storage
	- Network
	- Firewall Rules; Security groups

S3 (Simple Storage Service)
- Inexpensive object storage
	- files
		- images, videos, documents, website code
- Unlimited storage capacity
- Organized into buckets (groups)
- Use Cases
	- Hosting static website
	- Data Storage

- Used to store any type of data, and retrieve any amount of data from anywhere
- Object - Any type of file, and any metadata for a file
- Buckets - Used to store objects

VPC (Virtual Private Cloud)
- Personal isolated section in the cloud

Route 53 (DNS)
- Operates as a DNS
- 

ELB (Elastic Load Balancer)
- 

Lambda
- Used for serverless compute
- Don't have to worry about spinning up server, automatically does this when function is running
- Pay based on calls and runtime
- Used with API gateway for websites

API Gateway
- Used to direct traffic and activate the correct lambda functions for websites

CloudFront
- Used to cache web content to edge locations around the world

ECS (Elastic Container Service
- automatically starts, stops, containers
- checks containers if running properly
- Automatically replace any that fail
- Can automatically create more containers to handle increased load
- Mix between Lambda and EC2
	- Don't have to manage infrastructure
	- able to customize environment

RDS (Relational Database Service)
- automatically handles backups, security patches, scaling, smooth operation

DynamoDB
- Built for speed and scale
- Handle a lot of data with low latency

Aurora

Redshift

IAM (Identity and Access Management)
- Ensures that every component only has the access that they need
	- no more, no less

CloudTrail
- Used for auditing
- records every single API call made in AWS account
- Any change is logged
	- what changed, when it was changed, who changed it

GuardDuty

CloudWatch
- Primary AWS Monitoring and Observability Service
- Gathers performance metrics, logs, events, from your services
- create dashboards and alerts
- Can trigger automated responses
	- Heavy load -> scaling
	- service failure -> recovery