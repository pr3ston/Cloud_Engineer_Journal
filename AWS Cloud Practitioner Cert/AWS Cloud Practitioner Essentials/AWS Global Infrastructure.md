## How to choose a Region/Set of Regions
Factors
- Compliance - Does data need to live in a specific region/country?
- Proximity - How close are the customers to the resources
- Feature availability - Not all regions have the same resources
- Pricing - Some locations are more cost efficient (Local tax, etc)

## Edge Locations
- Smaller footprint facilities
- Cache the most popular items:
	- images, videos, and other resources for quicker access

## IaC/CloudFormation
- Define infrastructure in a file
- Automate deployment
- Maintain consistency among different regions/edge locations

## Multi-AZ/Multi-Region
- High availability - operate without failing
- Agility - quickly adapt to changing requirements or market conditions
- Elasticity - ability to scale resources up or down automatically

## AWS Cloudfront
- Content delivery network
- Designed to serve content as close to users as possible
	- Images, data, videos, apps, api, etc
- Uses edge locations
	- Separate from regions

## Route 53
- AWS version of DNS