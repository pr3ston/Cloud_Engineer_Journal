## Relational Database Services

#### RDS
- Managed service
- Multi-AZ deployment and automated backups
- Automated patching
- Backups
- Redundancy
- Failover
- Disaster Recovery
- supports:
	- Aurora, MySQL, PostgreSQL, Microsoft SQL Server, MariaDB, Oracle DB
- Used for webapps, enterprise workloads, product inventories

Security:
- network isolation
- encryption in transit and rest

#### Aurora
- fully managed
- Reduces unnecessary I/O operations
- Supports:
	- PostgreSQL
	- MySQL
	- DSQL
- Up to 15 replicas across AZs
- Supports AWS Backup
- Used for gaming apps, media/content management, real-time analytics
- Scales automatically


## NoSQL DB Services

#### DynamoDB
- Fully managed serverless
- Non-relational
- Data = items = set of attributes
	- Attribute = name + value
- Scales automatically
- Built in security features
- Can be used for globally distributed apps = **DynamoDB Global Tables**
- Ideal for high performance and seamless scaling

## Caching
- Temporarily stores frequently accessed data in RAM

#### ElastiCache
- Fully managed
- Reduces complexity of administering in-memory caching systems
- Automatically detects and replaces failed nodes

## Other Services

#### DocumentDB
- Fully managed
- Handle semistructured data
	- information that doesn't conform to rigid relational schemas
	- MondoDB compatible
- For apps requiring frequent schema changes and document-oriented data
- Quickly iterate without relying on predefined schemas
- Uses JSON
- Automatically scales
- Up to 15 replicas

#### AWS Backup
- provides single dashboard for monitoring and managing backups
- eliminates complexity of managing multiple backup strategies
- Supports
	- EBS
	- EFS
	- Others
- Centralizes and automates data protection processes

#### Neptune
- fully managed
- graph db
- Understands complex relationships
- auto scales