## Instance Types
- General Purpose
	- Used for diverse workloads, web services, code repos, workload perf. is uncertain
- Compute Optimized
	- Compute intensive tasks
	- Gaming, machine learning, scientific modeling
- Memory Optimized
	- Memory-intensive tasks
	- Data analytics, database processing
- Accelerated Computing
	- Use hardware accelerators like GPUs
	- Graphics processing, floating-point calc, machine learning
- Storage Optimized
	- Require high performance ofr locally stored data
	- large DBs, data warehousing, I/O intensive apps

## Pricing
- On Demand
	- Classic EC2 instance
	- Only pay what you use
	- Think VM on shared section on server
- Savings Plans
	- Discounts for On-Demand rates in exchange for commitments
- Reserved Instances
	- Similar to reserved instances
- Spot instances
	- Instances that are created from spare space on servers
	- May be taken back at anytime by AWS
- Dedicated Hosts
	- Entire physical server for your account
- Dedicated Instances
	- Hardware dedicated solely to your account
	- Single isolated section on server

## Scaling/Elasticity
- Scalability - Ability of a system to handle increased load by adding resources
- Elasticity - Ability to automatically scale resources up or down in response to real-time demand
- EC2 Auto-scaling Groups
	- Adds or removes resources based on usage
	- Minimum Capacity
		- Minimum number EC2 instances required
	- Desired Capacity
		- Ideal number of instances needed to hand current workload
		- If not specified, Group defaults to minimum capacity
	- Maximum Capacity
		- Upper limit on number of instances preventing over-scaling and controlling costs

## Load Balancing
- Distributes traffic between resources
- Can handle both internal and external traffic
- Serves as single point of contact for all web traffic to ASG
- Benefits
	- Efficient traffic distribution
	- Automatic Scaling
	- Simplified management
- Routing methods
	- Round Robin - Distributes traffic evenly across all available servers in a cyclic manner
	- Least Connections - Routes traffic to server with fewest active connections, balanced load
	- IP Hash - Uses client's IP to route traffic to same server
	- Least Response Time - Directs traffic to server with fastest response time

## Messaging and Queuing
- AWS Simple Queue Service (SQS)
	- Send, store, receive messages
	- Where messages are placed until processed
- AWS Simple Notification Service (SNS)
	- Channel for messages to be delivered
	- Need a response right away
	- `Publish-Subscribe` service
		- Send messages to subscribers through SNS topics
	- 
- Payload - Data contained in a message
- AWS EventBridge
	- Connects different parts of an application using events
	- You route events from sources (custom apps, AWS services, etc) to other apps
	- 