## Authentication vs Authorization
Authentication - verifying the identity of a user through credentials
Authorization - grans users certain access rights and permissions

## Shared Responsibility Model
#### Customers: Security IN the Cloud
- Securing everything we create and mange
- Security of data, systems, apps
- Deciding what data and workloads to store/run
- Which AWS services to use
- Controlling access controls to env and resources

#### AWS: Security OF the Cloud
- Operates, manages, controls components at all layers of infrastructure
- Foundational software
- Virtualization layer
- Hardware and global infrastructure

![[Pasted image 20250711140003.png]]

#### AWS Security Controls
- AWS provides security mechanisms
- Prevent security incidents via proper permissions and access mgmt
- Protect networks, apps, data
- Detect and respond to security incidents

## User Permissions and Access

#### Root User
- Can perform any action and control any resource in the account
- Use strong password
- Turn on MFA
- Don't use for daily tasks

#### IAM
- Used to handle user creation and access management
- Handle who can access what
- Sort into groups w/ permissions
- Explicitly grant actions
- Least privilege
- IAM policy - JSON document that controls what the user can/cannot access
	- Attach policies to users, groups, roles
- Roles can be assumed for temp amount of time
	- Associated permissions

#### IAM Identity Center
- Centralizes identity and access management across AWS accounts and apps
- Connect to an existing identity source 
- Can allow SSO (Federated Identity Management)
	- FIM - system that allows users to access multiple apps, services, domain with single set of creds

#### Secrets Manager
- Secure way to manage, rotate, retrieve db creds, API keys, secrets

#### Systems Manager
- Centralized view of nodes across orgs accounts, regions, multi-cloud and hybrid envs
- Quickly access node information (ID, os, registry edits, user management, security patching)

## Network & Application Protection
- AWS automatically protects against low-level attacks

#### Security Groups
- Only allow proper request traffic
- Operates at network level -> DDoS goes through entire region (Not Effective at all)
- Runs at Region level

#### Elastic Load Balancing (ELB)
- Handles traffic first before going to server
	- server not overwhelmed
- Run at Region Level

#### AWS Regions
- Capacity of Regions makes it difficult to overwhelm.

#### AWS Shield
###### Shield Standard
 - Designed to automatically protect customers from most common DDoS attacks at no cost
 - Uses a variety of analysis techniques to detect, mitigate incoming malicious network traffic

###### Shield Advanced
- Paid service
- Provides detailed attack diagnostics and ability to detect, mitigate sophisticated DDoS attacks
- Integrates with other services:
	- CloudFront
	- Route 53
	- ELB

#### AWS WAF
- Monitors network requests
- Checks IP address against ACL

## Data Protection
- Built-in data protection
	- S3
		- Defaultly encrypted at rest
	- EBS
		- Volumes and snapshots are encrypted at rest
		- Includes both boot and data volumes of EC2 instance
	- DynamoDB
		- Server-side encryption at rest on all table data using keys

#### Key Management Service (KMS)
- Used to create and manage cryptographic keys
	- Used to encrypt and decrypt data
- Specify which IAM users, roles, groups, can manage keys
- Keys never leave KMS

#### Macie
- Monitor sensitive data at rest
- Uses ML and automation to discover sensitive data in S3
- Access security posture for compliance

#### AWS Certificate Manager (ACM)
- Manages your SSL/TLS certificates
	- Provides data encryption in transit

## Incident Detection and Response Services

#### Amazon Inspector
- Runs automated security assessments for EC2, containers lambda functions
- Checks for vulnerabilities and deviations from security best practices
- View via Inspector console
	- List of security findings prioritized by severity
	- Detailed description and recommendation on how to fix
	- Also found via API

#### GuardDuty
- Threat detection across resources
- Identifies threats by continuously monitoring streams of account metadata and network activity
- Uses known malicious IPs, anomaly detection, ML to identify threats
- View findings via Management Console
	- Steps for remediation
	- Can set up Lambda functions for automatic remediation

#### Detective
- Further investigate root cause of a threat
- Interactive visualizations contained in unified Management Console view
	- Include resource and user interactions over a timeline
	- Remediation steps

#### Security Hub
- Quickly see your security and compliance state in one view
- Aggregates security findings from AWS and partner services
	- Organizes them into actionable, meaningful groupings called insights