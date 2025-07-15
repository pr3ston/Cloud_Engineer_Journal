## 3 Phases of Cloud Migration
1. Assess
	1. Build business case for migration and assess readiness
	2. AWS Migration Evaluator
2. Mobilize
	1. Prepare the org and mobilize resources needed for migration
	2. AWS Application discovery Service
	3. AWS Migration Hub
3. Migrate and Modernize
	1. Use your strategy, plan, best practices to migrate and modernize
	2. AWS Application Migration Service
	3. AWS Database Migration Service
	4. AWS DataSync, Transer Family, Snow Fmaily (Data Transfer)

## AWS Cloud Adoption Framework (CAF)
- Framework that brings AWS experience and best practices to companies that are preparing to migrate to cloud
- Reduce business risk and improve sustainability and corporate transparency
- AWS CAF Perspectives
	- Leadership/business
		- Business
			- Ensures IT aligns with business needs
			- IT investments link to business results
		- People 
			- Supports dev of org-wide change management strategy
			- Evaluate org structures and roles, assess new skills/process requirements, gaps
			- Prioritize training, staffing, org changes
			- HR, Staffing, People Managers
		- Governance
			- Focuses on skills and process to align IT strategy with business strategy
			- Maximize business value and minimize risks
			- How to update staff skills and processes necessary to maintain business gov in cloud
			- CIO, Program Mangers, Enterprise architects, Business analysts
	- Technical
		- Platform 
			- Principles and patters for implementing new solutions in cloud
			- Migrating workloads to cloud
			- Uses variety of architectural models to understand/communicate the strucutre of IT and their relationships
			- CTO, IT managers, Solutions architects
		- Security 
			- Ensure that org meets security objectives for visibility, auditability, control, agility
			- Use to structure the selection/implementation of security controls meet org needs
			- CISO, IT security analysts/managers
		- Operations
			- Enable, run, use, operate, recover IT workloads to level agreed upon by stakeholders
			- Define day-to-day business is conducted
			- Use to define current operating procedures/indentify process changes
			- IT operations managers

## 7 R's of Migration
#### Relocate
- Changing the hosting location to the cloud
- If using VMs or Containers, simply moving them to the cloud
#### Rehost ("Lift-and-shift")
- Involves moving apps without changes
- 1-1 moving
#### Replatform ("Lift-tinker-shift")
- Making few cloud optimizations
- Like Rehost
#### Refactor
- Re-architecting
- Reimaging how an app is architected and developed
- Adding features, scaling, improving performance that would otherwise be difficult without the cloud
#### Repurchase
- Moving from a traditional license to software-as-a-service model
- Choose to migrate from one software vendor to another
#### Retain
- Keeping apps that are business critical in the source env (on-prem)
- Apps that may require major refactoring
#### Retire
- Getting rid of process or apps that are no longer needed

## Migration Services
### Access Phase
#### Migration Evaluator
- Helps you create a business case for AWS migration
- Data driven approach
	- Analyzes current state, target state, developing a migration readiness plan with projected cloud costs
- Removes guesswork when migrating
- Shows cost-effective migration scenarios
- Gives insights on reusing existing software licensing
### Mobilize Phase
#### Application Discovery Service
- Discovers on-prem server inventory and connections
- Gathers config, performance, connection details from servers/databases to create detailed migration plan
- Receive a comprehensive snapshot of current inventory
- Integrate product with Migration Hub
#### Migration Hub
- Centralized hub for migration
- Provides tools, guidance, automated recommendations to collaborate with team and track migration
- No charge to use
### Migrate and Modernize Phase
#### Application Migration Service
- Used ot move and improve on-prem and cloud-based apps
- Streamline, expedite, reduce the cost of migrating and modernizing apps
- Support to migrate any source infra that runs on supported OS
- Makes it possible to modernize while migrating
- Maintain normal business operations

## Database Migration
#### AWS DMS
- Quickly and securely migrate DB and perform ongoing data replication tasks for live db and data warehouses
- Helps with planning, assessing, converting, migrating dbs
- Supports homogenous and heterogenous migrations
- Migrate TB sized dbs a low cost

#### AWS Schema Conversion Tool (AWS SCT)
- Converts database schemas and code objects from one db engine to another
- Can give estimates on how big of conversion it is -> planning
- Automates schema analysis, recommendations, conversion at scale
- Compatible with popular dbs and analytics services

## Transferring Data Online
#### AWS DataSync
- For bulk data transfers from other storage services to AWS and back 
- Designed for automating and accelerating data transfer
	- Running instances, encryption, network optimization
- Bandwidth throttling, migration scheduling, task filtering, task reporting
- Rapid data replication

#### AWS Transfer Family
- Smaller data transfers from a client to server and back
- Manage and share data with simple, secure, scalable file transfers
- Supports FTP, SFTP, FTPS, and others
- Transfers into and out of AWS storage like S3 and EFS

#### Direct Connect
- Dedicated private connection to VPC from on-prem through an AWS partner

## Transferring Data Offline
