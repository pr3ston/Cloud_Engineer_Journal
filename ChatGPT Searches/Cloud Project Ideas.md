That’s a smart move, Preston — building cloud projects **while studying for the AWS Solutions Architect – Associate** (SAA-C03) helps reinforce concepts **and** gives you tangible experience to showcase on your resume.

Here are **resume-worthy AWS cloud projects** (with suggested architecture components) that align directly with the exam topics:

---

## 🔧 1. **Deploy a Scalable Web Application**

**What It Shows**: High availability, scalability, VPC, load balancing, autoscaling

### 🧱 Stack:

- Frontend: HTML/CSS or React
    
- Backend: Node.js or Python (Flask)
    
- Database: RDS (MySQL/PostgreSQL)
    
- Infrastructure: EC2, ALB, Auto Scaling Group, custom VPC
    

### 🔐 Features:

- Use Security Groups and NACLs
    
- Place app in private subnets; use NAT Gateway
    
- Deploy infrastructure using **CloudFormation** or **Terraform**
    

---

## ☁️ 2. **Serverless File Upload and Processing App**

**What It Shows**: Serverless, event-driven architecture, IAM, S3, Lambda, cost-efficiency

### 🧱 Stack:

- S3 bucket for file upload (e.g., images or PDFs)
    
- Lambda function to process uploaded files
    
- Store metadata in DynamoDB
    
- Notify user via SNS or email
    

### 🧠 Bonus:

- Restrict file types
    
- Add CloudWatch logging and metrics
    

---

## 🔐 3. **IAM Policy Analyzer App (Small CLI or Web App)**

**What It Shows**: IAM best practices, least privilege, role-based access

### 🧱 Stack:

- Python CLI tool or web app using Flask
    
- Takes IAM policies, analyzes for overly permissive access (e.g., `s3:*`)
    
- Uses AWS SDK (`boto3`) to fetch and audit policies
    

---

## 🌐 4. **Static Website Hosting on S3 with CloudFront and Route 53**

**What It Shows**: Global content delivery, DNS, storage, cost-efficient architecture

### 🧱 Stack:

- Website hosted on S3 with static assets
    
- CloudFront distribution in front
    
- Custom domain using Route 53
    
- Add SSL/TLS with ACM (free certificate)
    

---

## 🔄 5. **Disaster Recovery Simulation**

**What It Shows**: Resilience, RTO/RPO understanding, cross-region architecture

### 🧱 Stack:

- Deploy a workload in **us-east-1**
    
- Replicate S3 to **us-west-2**
    
- Use Route 53 failover policy
    
- Document RTO/RPO for each component
    

---

## 📈 6. **Real-Time Log Monitoring System**

**What It Shows**: Monitoring, observability, decoupling

### 🧱 Stack:

- CloudWatch Logs from Lambda or EC2
    
- Kinesis Data Firehose → S3
    
- Use Athena or QuickSight to query logs
    
- Optional alerting with CloudWatch Alarms + SNS
    

---

## 🧪 7. **CI/CD Pipeline on AWS**

**What It Shows**: DevOps integration, automation, infrastructure as code

### 🧱 Stack:

- CodeCommit → CodeBuild → CodeDeploy → EC2 or Lambda
    
- Pipeline triggers on push to `main` branch
    
- Include IAM roles, least privilege policies
    
- Optional: Terraform to deploy the pipeline
    

---

## 🧰 Tools to Consider Using:

- **Terraform or AWS CloudFormation** for IaC
    
- **boto3** (Python SDK) or **AWS CLI**
    
- **GitHub Actions** for deployment automation
    
- **CloudWatch** for metrics and alerting
    

---

## ✅ Resume Tip Format (for each project):

```
Project Name – AWS Cloud Project
• Designed and deployed a scalable 3-tier web application using EC2, ALB, Auto Scaling Groups, and RDS in a custom VPC
• Implemented cost optimization and monitoring with CloudWatch and AWS Budgets
• Defined infrastructure as code using Terraform with modular reusable components
```

---

Would you like help writing up one of your existing projects in bullet points for your resume? Or I can guide you step-by-step to build one of these from scratch.