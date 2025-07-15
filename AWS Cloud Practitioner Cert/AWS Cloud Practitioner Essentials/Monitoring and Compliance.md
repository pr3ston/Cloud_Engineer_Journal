## Monitoring
Ideal Progression for effectively monitoring cloud:
- Securing systems
- Monitoring activities
- Conducting audits
- Ensuring compliance

Provides a way to continuously observe and analyze system activity, network traffic, and security events to detect potential threats or anomalies. Helps to ensure security, reliability, and performance.

#### CloudWatch
- Monitors AWS resources and apps in real-time
- Gain system-wide visibility in resource utilization, app performance, operational health
- Several features:
	- Metrics
	- Alarms
		- Send alerts or automatically makes changes
	- Dashboards
	- Logs

## Auditing
#### CloudTrail
- Tracks user activity and API usage in AWS Cloud, on-prem, and on other clouds
- Provides detailed history of API calls
	- Track changes and who made them and when
- Auditing, security monitoring, operational troubleshooting.
- Prove compliance and improve sec posture
- Features:
	- Events
		- Logs about API calls, console actions, etc.
		- Record of the past 90 days of management events
	- Logs
		- Creates logs based on events and activities
		- Stored in S3 bucket
	- Insights
		- Analyzes normal patterns of API call volume and API error rates
		- Generates insights events when those volumes and rates deviate
		- Can be enabled on trails or event stores to detect weird behavior/activity

## Compliance
#### AWS Artifact
- Provides no-cost, on-demand access to AWS security and compliance reports and select online agreements
- 2 types:
	- Agreements
		- review, accept and manage agreements for an individual account and all counts in AWS Organizations
		- Different types of agreements offered to address needs of customers who are subject to specific regulations. 
	- Reports
		- Provides compliance reports from third-arty auditors on AWS
			- Auditors test and verify AWS as compliant with global, regional, industry standards

#### AWS Compliance Portal
- Contains resources to help you

## Auditing Resources for Compliance
#### AWS Config
- Assess, audit and evaluate the configs of your AWS resources
- Continuously track changes
- Check configs against desired state, manage config changes, troubleshoot and remediate
- Create custom rules
- Generate compliance reports

#### AWS Audit Manager
- Assess your policies
- Manage reviews
- Build audit-ready reports
- Provides prebuilt frameworks
- Continually audits your AWS usage
- Helps to collect evidence and manage audit data
	- Automated evidence collection
	- Ensures audits are read-only

## AWS Organizations
- Manage/govern your env
- Scale your env via programmatically creating new AWS accounts for resources/teams
- 1 Primary account, all other accounts are "children" to it
- Can group accounts into different groups (Organization Units)
- Configure Service Control Policies (SCP) for groups to control max permissions for accounts in that group

## Governance
- A framework to manage IT goals with policies, processes, and structures to ensure adherence

#### AWS Control Tower
- Used to enforce and manage governance rules for security, ops, and compliance across your org
- Uses preconfigured controls and blueprints to quickly set up multi-account envs
- Automation with built-in governance
- Dashboard to see accounts and control policy enforcement and detect non-compliant resources
- Configure account templates that standardizes account provisioning

#### AWS Service Catalog
- Create, share, organize from curated catalog of AWS resources
- Deploy baseline networking resources and security tools for new AWS accounts
- Quickly find and deploy approved self-service resources
- Blueprints for AWS resources

#### AWS License Manager
- Manage software licenses
- Reduce risk of noncompliance with licenses
- Automate distribution and activation of software entitlements across AWS accounts

## AWS Health Dashboard
- View account-specific health info, and get health event updates
- You can interact with it with the AWS Health API (Available w/ AWS Premium Support)
- Give you timely/actionable guidance to remedy issues
- Manage service health

## Advisory
#### AWS Trusted Advisor
- Continuously evaluate AWS env using best practice checks across several categories
- All AWS support plans access dozens of checks
- Gives recommendations on what can be improved to optimize your env

#### IAM Access Analyzer
- Set, verify, refine permissions by analyzing external access and validating your policies match corporate security standards
- Refine permissions, validate IAM policies -> meet least privilige
- Automate IAM policy reviews