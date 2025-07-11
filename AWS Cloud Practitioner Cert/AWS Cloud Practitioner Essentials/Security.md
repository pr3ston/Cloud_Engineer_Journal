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
	- Attach policies to users