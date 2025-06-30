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