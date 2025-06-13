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
- Unlimited storage capacity
- Organized into buckets (groups)
- Use Cases
	- Hosting static website
	- Data Storage

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

RDS

DynamoDB

Aurora

Redshift

IAM

CloudTrail

GuardDuty

CloudWatch