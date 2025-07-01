## Unmanaged and Managed Services
- Unmanaged (EC2)
	- AWS takes care of underlying physical infrastructure
	- User responsible for setting up, securing, maintaining OS, network config, apps
- Managed Services
	- Reduce amount of infrastructure you need to manage
	- You still need to perform some provisioning and config based on service
- Fully-managed (Lambda)
	- Eliminates the need to provision or manage any servers
	- Infrastructure fully managed my AWS
![[Pasted image 20250630155618.png]]
## AWS Lambda
- Serverless, FaaS (Function as a Service)
- AWS takes care of scaling, updates, patches, etc
- You only need to put in your code
- Maximum Duration of Lambda Function is 15min
- Supports different Programming Languages
- Charged by compute time

## Containers and Orchestration
- Amazon Elastic Container Service (ECS)
	- Streamlined and integrated
	- Define some params
	- Fully Managed Service
- Amazon Elastic Kubernetes Service (EKS)
	- Fully managed service for running Kubernetes
	- Open Source
	- Manages containers
	- Automates container deployment, scaling, management
- Amazon Elastic Container Registry (ECR)
	- Like Docker Hub
	- Stores container images
	- Fully managed Docker registry
- AWS Fargate 
	- Can be used to run containers
	- Serverless
	- Only need to manage containers

## Additional Compute Services

#### Elastic Beanstalk
- Fully Managed service
- Streamlines deployment, management, scaling of web apps
- Upload code -> beanstalk handles provisioning of infrastructure, scaling, load balancing, app health monitoring
- Supports various programming languages and frameworks
- Good for
	- APIs, mobile backend, web apps, microservices

#### AWS Batch
- Fully managed
- Used to run batch computing workloads
- Automatically schedules, manages, scales compute resources for batch jobs
- Good for:
	- processing large-scale, parallel workloads for scientific computing, risk analysis, media transcoding, big data processing, machine learning, genomic research

#### Amazon Lightsail
- Offers Virtual Private Servers (VPS), storage, databases, networking
- Ideal for small businesses, basic workloads, developers seeking straightforward AWS expereince without complexity of full AWS management console 
- Good for:
	- Basic web apps, low-traffic websites, dev and testing envs, blogs, learning cloud services

#### AWS Outposts
- AWS gives you a server that has the AWS software on it
- You host the server on-prem, but are still able to use AWS
