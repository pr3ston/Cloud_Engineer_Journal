## AWS VPC
- Isolated section of AWS where you can launch AWS resources
- Subnet - Used to organize resources into public or private zones
	- Chunks of IP addresses in your VPC to group resources together

## Internet Gateway
- Doorway open to the public
- Allows traffic to leave and enter the Public Subnet

## Virtual Private Gateway
- Only allows traffic from an approved external network to access the resources

## AWS Dedicated Connect
- Completely private direct connection via fiber from your DC to AWS
- Different from VPN as with VPN you would still need to traverse internet
- Uses direct connect partner

## Connecting to AWS Cloud
- AWS Client VPN
	- Used to connect remote workers and on-prem networks to the cloud
	- Fully Managed, Elastic
	- Don't need to install or manage hardware
	- Quick and easy access
- AWS Site-to-Site VPN
	- Creates secure connection from on-prem DC or branch offices to AWS
	- Secure and encrypted
	- App migration or secure communication between remote locations
- AWS PrivateLink
	- Allows you to privately connect your VPC to other cloud provider's resources
	- Don't need to use internet gateway, NA, public IP, direct connect, nor VPN
	- Control specific API endpoints, sites, services, resources
	- Connecting client VPC resources, other VPC, and endpoints
- AWS Direct Connect
	- Established dedicated private connection between your DC and VPC
- AWS Transit Gateway
	- Used to connect VPC and on-prem networks via central hub
- NAT Gateway
	- Allows private subnet to connect to outside services but external services can't initiate a connection to those in the private subnet
- AWS API Gateway
	- Used for creating, publishing, maintaining, monitoring, and security APIs to any scale

## Security Groups
- Instance level security
- Doesn't allow any traffic into instance by default
- Only allow rules
- Stateful

## Network Access Control Lists (NACLs)
- Checks if packets have rights to enter or leave the subnet
- Both allow and deny rules
- Only controls subnet traffic
- Stateless

## AWS Global Accelerator
- Uses intelligent traffic routing and fast failover
- Routes traffic over AWS infrastructure instead of internet