## Activity Timeline
#### 6/9/25
- Today I have started my journey towards completing the AWS Cloud Practitioner Cert. I have signed up for the free `AWS Cloud Practitioner Essentials` course on the `AWS Skill Builder` website. I have also started to watch the `AWS Certified Cloud Practitioner Certification Course (CLF-C02) - Pass the Exam` video on Youtube by `freeCodeCamp.org`.
- Time Studying - 2hrs
	- 1:52:26 on the Youtube course (innovation Waves)
- Time Studying - 30min
	- 2:22 on the Youtube course (Fault Tolerance)

#### 6/11/25
- Continued watching the Youtube video and covered the following topics:
	- Fault Tolerance
	- AWS Global Network
	- Point of Presence (POP)
	- Tier 1
	- AWS POP
	- AWS Direct
	- Direct Locations
	- Local Zones
	- Wavelength Zones
	- Data Residency
	- GovCloud
	- AWS China
	- Sustainability
	- -----------------------
	- Ground Station
	- Outposts
	- Cloud Architecture Terminology
	- High Availability
	- Scalability
	- Elasticity
	- Fault Tolerance
	- Durability
	- Business Continuity Plan
	- -----------------------
- Time Studied - 50min
	- 2:56:47 on Youtube
- Time Studied - 1hr
	- Studied the main services on AWS

#### 6/13/25
- I started to watch a new Youtube video that explains the main services that AWS has to offer, as well as why to use them. Topics covered:
	- AWS networking
	- Route 53
- Time Studied - 30min
	- 12:30pm - 1pm
- Time Studied - 2hr 40min
	- 2:20pm - 5pm

#### 6/17/25
- It's been a while since I last studied but that's because I was preparing for an interview. The interview was for an internship at a local startup. The Sr. Security Engineer that I interviewed with also had a strong interest in the Cloud while also having 12 years of experience. In fact, he mentioned how he was the Sr. Cloud Architect at the startup. However, he still mentioned that he's more of a well-rounded security professional as in the job he is constantly working with other teams and on other projects besides the cloud. For example, he mentioned that he worked a lot with the SOC for incident response and also worked with the AppSec team for securing code. Overall, I think the interview went well and that we really clicked on the interest in cloud. The interview ended early, and I was able to ask him questions regarding the cloud. Highlights of what he mentioned
	- Cloud Engineers work a lot with devops. It is important to learn the following things:
		- Kubernetes
		- EKS
		- Containers (Docker)
		- Terraform (IaC)
	- It is good to get some certs, though he doesn't really believe in certs himself. Recommended that I continue to pursue the Cloud Practitioner cert. 
	- He mentioned the power of getting hands-on experience through projects. 
		- Also mentioned that it would be good to utilize the AWS online training/labs

#### 6/18/25
- Today I received a message on LinkedIn from a classmate of mines who is also going into the Cloud industry.

This was his message;

```
Physical infra is important to know but it's a dying practice in orgs. Home lab projects are still valuable for experience/resume, but any org planning to grow will be working on migrating if they aren’t already 100% cloud based like **This Company** is.  
  
To give some context of where my advice/opinions come from: my team is essentially labeled ‘platform engineers’. Its newer concept of a cloud engineer, essentially meant to act as the grease between our team of cloud engineers and principal architects who are making high level decisions, and developers who need to work without the obstructions that are sometimes caused by developing in a cloud environment. This is the white paper if you’re interested [https://tag-app-delivery.cncf.io/whitepapers/platforms/](https://tag-app-delivery.cncf.io/whitepapers/platforms/)  
'Developer enablement’ is pretty much the whole purpose of our team. We see the app developers as our ‘customers’, and we see ourselves as the solutions architects to them. It’s a blast btw. Very very fun and interesting.  
  
There’s obviously more than one way to break the entry barrier, but to be honest if I had to start over I would probably do the exact same thing as before. Here’s my suggested roadmap + insights:  
  
The best place to start is with the AWS certs. They have REALLY good learning resources for like $30 a month [https://skillbuilder.aws/](https://skillbuilder.aws/) There’s good 3rd party resources too, but I wouldn’t use those until after you’ve done all the AWS provided learning. Yes they also made a video game as a part of the learning course. It’s cheesy but worth it lol.  
  
1. Get the basic cloud practitioner cert, you can knock all of it out in about a month or less, including the test.  
  
2. Next step in my opinion is the Solutions Architect Associate cert. This one takes a bit longer. I ripped through it in about 2 months but that was a bad idea and I would recommend giving it at least 5-6 months to retain everything.  
  
I did use a 3rd party test bank for my exam study on this. Was very helpful since I sped run all the learning material.  
  
From here you can kinda decide what’s interesting to you. AI, Networking, etc, and pursue the next cert from there. My next certs will probably be: CKAD (not AWS) -> AWS DevOps Engineer -> AWS SA Professional  
  
3. After getting your SA you’re pretty close to being marketable, but you need to have projects. I think we were in OS together last Fall? I had my SA by that point so we (mostly me cause nobody else knew how lol) did our whole project on setting up a K8s cluster in AWS that hosted dockerized apps, and used cloud formation (IaC) for cluster portability. Not very hard tbh, but that project, along with having my SA, is what ultimately landed me the internship.  
  
Things to keep in mind:  
You’ll discover very quickly by doing the certs that AWS has done a great job of providing almost everything you’d need in an org IT environment. You’ll also discover by being in industry that there are a million things that don’t fit neatly into cloud infrastructure. For example Bamboo has a lot of specific use cases, special needs, and deployment strategies that don’t have 1:1 solutions in AWS. A lot of resources and expertise goes into creating solutions that are outside of AWS, but still work in tandem with our AWS accounts. Old hat 30 yr veteran developers are still VERY relevant in this sense, and It absolutely pays to have some development skills (which I inherently lack and need to get better at)  
  
This means that having a handle on other technologies is important. Outside of AWS, Bamboo uses:  
- Terraform (a lot)  
- Puppet  
- Github actions (for image building and CI/CD pipeline)  
- Humanitec (orchestrating platform)  
- Backstage  
- Score  
- k8s (we use EKS which is AWS managed, but the deployments are defined and applied via Terraform repos)  
- Docker (a lot)  
- And a ton of other stuff  
  
Since there’s so much going on, you’ve got to do some personal projects that showcase some similar things, and integrate them with AWS when possible.  
  
- Containerized apps  
	- Docker is the best  (seriously, you need to get good at docker [https://www.docker.com/trainings/)](https://www.docker.com/trainings/\))  
  
- Kubernetes  
	- K3d is a good way to do this easily (Use it to run and load balance dockerized apps)  
  
- IAC/State Management  
	- Ansible  
	- Terraform  
	- Puppet  
	- Cloud formation  
(try to do a different project with each of these. If you can terraform a k8s deployment with dockerized apps you’ll be golden)  
  
- Some form of AWS authentication  
	- AWS IAM  
	- AWS Identity Center  
  
If you’re trying to figure out what project(s) to do in the future or where to even get started just lmk and I’m happy to give ideas. 90% of the time this stuff is easier to set up than you’d expect. It gets complicated once you are trying to piece things together in custom ways to create a bespoke solution for ridiculously convoluted developer needs… So it’s good to get reps in when the use cases are simple and straightforward.  
  
  
Long story short I would just start with the certs, get some projects that you can showcase, start applying for positions while thinking about/working on your 3rd cert, but don’t forget to do some home lab stuff too.  
  
  
This is a huge dump and Idk where you’re at experience-wise, but feel free to ask anything about tech, industry, projects, whatever. Send any stupid questions my way, I'm happy to help with getting started. Hope this helps.
```

- A lot of great information to unpack. According to this message, my classmate recommends the following:
	- Cloud Practitioner Cert -> Solutions Architect Associate
	- Learning different tools
		- K8s
		- Docker
		- IaC
		- GitHub Actions (CI/CD pipeline)
- Today I will be starting to study using the AWS skill builder website. I will first start with the free modules in preparation for the Cloud Practitioner Cert. If needed, I'll then pay for the individual subscription. Today I'll be going through the AWS Cloud Quest: Cloud Practitioner module.
- Time Studied - 6.5hrs
	- 9:30am - 4pm
	- Topics covered:
		- EC2
			- EBS (Elastic Block Store) - Storage for EC2
		- S3
		- Networking
		- RDB
		- VPC
		- DynamoDB
- Time Studied - 30min
	- 4pm - 4:30pm
	- Topics covered:
		- Kubernetes

#### 6/21/25
- It's been a couple of days since I last studied, but today I have continued to study for the cert through the Youtube video same as before. I have also set up a computer with Ubuntu Desktop in preparation for using it as a Kubernetes node. Man that was such a pain. But I eventually got it. I have a lot of free time this upcoming week so I hope to be able to commit a lot of hours towards studying for the cert and at least be 90% done with the Youtube video and all of the content. Here is a list of all of my goals:
	- Watch 90% of the Youtube video by
 	 	- Suppliment with the AWS training
		- Will finish by 6/25 if watched about 3hrs/day for next 4 days
	- Start learning the basics of docker/containerization

#### 6/23/25
- Today I am continuing to study for the Cloud Practitioner exam via the Youtube video. I plan to go through at least 3 hours worth of video content.
- Topics Covered:
	- Disaster Recovery
	- AWS API
	- AWS Management Console
	- AWS CLI
	- ARN
	- Account ID
	- AWS SDK
	- AWS Cloudshell
	- -----------------
	- IaC
	- CloudFormation
	- CDK
- Time studied - 2hrs
	- 9:30am  - 12pm
		- 4:13:31 on Youtube Video
	- 3pm - 3:30pm
		- 4:41:39 on Youtube Video

#### 6/30/25
- Continued to study for the CP exam. I have switched to the `AWS Cloud Practitioner Essentials` course on the AWS website. Topics I covered:
	- What is the cloud
	- Cloud Shared Responsibilities
	- EC2
		- Instance types
		- Pricing
		- Scaling
		- Load Balancing
		- Messaging and Queuing
	- -----------
	- Lambda
	- Containers
		- EKS
		- ECS
		- Fargate
		- ECR
- Time Studied - 4hrs
	- 11:45am - 1:15am (1.5hrs)
	- 2:30pm - 5pm (2.5hrs)

#### 7/1/25
- It is a new month and I am about a third of the way done with the `AWS Cloud Practitioner Essentials` course. Today I plan on going through another 4 or 5 modules at least. Overall, I think that this course gives a foundation for what the exam would cover but not in that much detail. Because I am not sure, I will take a couple of practice tests after this, and if my knowledge isn't where it needs to be at, then I will continue with another source. Topics covered:
	- AWS Global Infrastructure
		- Connection types
	- Networking
		- NACLs
		- Security Groups
		- VPCs
		- Subnets
	- ------------------
- Time studied - 
	- 10:30am - 2pm (3.5hrs)

#### 7/10/25
- Continued the `Cloud Practitioner Essentials` course. Topics covered:
	- Storage
		- Block store
		- Object store
		- File store
	- Databases
- Time Studied - (6.5hrs)
	- 10:30am - 5pm

#### 7/11/25
- Topics covered
	- AI/ML and Data Analytics
	- Security
	- Monitoring, compliance and governance

#### 7/30/25
- I have officially passed the AWS Cloud Practitioner Exam with a score of around 835! Honestly the only resources that I have used is the `Cloud Practitioner Essentials` course, the Youtube video found below, and a set of 6 practice tests that I found on Udemy. Those practice tests were harder than the actual exam but I liked that as it overprepared me for the actual exam. Now onto the Solutions Architect Certification
## Resources
- AWS Cloud Practitioner Essentials | AWS Training and Certification Website
- AWS Cloud Quest: Cloud Practitioner | AWS Training and Certification Website
- AWS Certified Cloud Practitioner Certification Course (CLF-C02) - Pass the Exam | freeCodeCamp.org via Youtube
- AWS Cloud Engineer Full Course for Beginners | Tech With Soleyman via Youtube
- What is Kubernetes | Kubernetes explained in 15 mins | TechWorld with Nana via Youtube
- Kubernetes Explained in 15 Minutes | Hands On (2024 Edition) | Travis Media via Youtube
