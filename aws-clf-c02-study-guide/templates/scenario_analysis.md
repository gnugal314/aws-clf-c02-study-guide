# AWS CLF-C02 Scenario Analysis

## Business Problem → Service Category → Service Framework

---

# Question 1

## Original Question

Your colleague wants to create certain Amazon EC2 and Amazon S3 resources in an automated fashion using AWS CloudFormation. However, they reached out to you asking for help to understand pricing. Which option will provide them with the information they need?

### Correct Answer

**A. AWS will charge for Amazon EC2 and Amazon S3. There is no charge for AWS CloudFormation.**

### Business Problem

Understand AWS pricing for infrastructure deployed using Infrastructure as Code (IaC).

### Service Category

Billing & Cost Optimization

### Service

AWS CloudFormation

### Trigger Words

* CloudFormation
* pricing
* EC2
* S3
* automated provisioning

### Why This Is Correct

CloudFormation is free. Customers pay only for the AWS resources created by CloudFormation.

### Similar Services to Eliminate

| Service             | Why Eliminate           |
| ------------------- | ----------------------- |
| Cost Explorer       | Analyzes existing spend |
| AWS Budgets         | Creates spending alerts |
| Cost & Usage Report | Historical billing data |

---

# Question 2

## Original Question

During a recent outage a number of static file uploads were lost and irretrievable. Your manager has tasked you with finding a more durable solution. Which service could be used with the least operational overhead?

### Correct Answer

**Amazon S3**

### Business Problem

Highly durable file storage.

### Service Category

Storage

### Service

Amazon S3

### Trigger Words

* static files
* durability
* lost uploads
* operational overhead

### Why This Is Correct

S3 provides 11 nines of durability and is fully managed.

### Similar Services to Eliminate

| Service        | Why Eliminate     |
| -------------- | ----------------- |
| EBS            | Attached to EC2   |
| EFS            | Shared filesystem |
| Instance Store | Temporary storage |

---

# Question 3

## Original Question

Your company wants you to focus on running and monitoring your cloud applications in a way that drives continuous improvement to procedures and processes. Which AWS Well-Architected pillar will help you identify the responsibilities in this scenario?

### Correct Answer

**Operational Excellence**

### Business Problem

Continuous operational improvement.

### Service Category

AWS Well-Architected Framework

### Service

Operational Excellence Pillar

### Trigger Words

* continuous improvement
* monitoring
* procedures
* operations

### Why This Is Correct

The Operational Excellence pillar focuses on monitoring, automation, and process improvement.

### Similar Services to Eliminate

| Pillar            | Why Eliminate      |
| ----------------- | ------------------ |
| Reliability       | Availability focus |
| Security          | Protection focus   |
| Cost Optimization | Cost focus         |

---

# Question 4

## Original Question

Your company is deploying a web application in AWS running on several Amazon EC2 instances. What is the responsibility of AWS under the shared responsibility model?

### Correct Answer

**Physical infrastructure, hardware, networking, and facilities security**

### Business Problem

Understand AWS responsibilities.

### Service Category

Security

### Service

Shared Responsibility Model

### Trigger Words

* EC2
* responsibility
* shared responsibility

### Why This Is Correct

AWS secures the infrastructure that runs AWS services.

### Similar Services to Eliminate

| Responsibility  | Owner    |
| --------------- | -------- |
| OS patching     | Customer |
| Security Groups | Customer |
| IAM permissions | Customer |

---

# Question 5

## Original Question

Your company's finance team wants to use their own business intelligence tool to visualize cost and usage. They want detailed billing line items for the last three years automatically available in a persistent store for their business intelligence tool without writing any scripts. Which AWS tool meets their requirements?

### Correct Answer

**AWS Cost & Usage Report (CUR)**

### Business Problem

Detailed billing and usage exports.

### Service Category

Billing & Cost Optimization

### Service

Cost & Usage Report

### Trigger Words

* detailed billing
* line items
* three years
* BI tool

### Why This Is Correct

CUR provides the most detailed billing and usage data available.

### Similar Services to Eliminate

| Service       | Why Eliminate      |
| ------------- | ------------------ |
| Cost Explorer | Visualization only |
| AWS Budgets   | Alerts only        |

---

# Question 6

## Original Question

A customer would like to design and build a new workload on the AWS Cloud but does not have the AWS expertise to get started. Which AWS program can a customer take advantage of to achieve that outcome?

### Correct Answer

**AWS Professional Services**

### Business Problem

Need AWS implementation expertise.

### Service Category

Cloud Adoption

### Service

AWS Professional Services

### Trigger Words

* lacks expertise
* design workload
* build workload

### Why This Is Correct

AWS Professional Services assists customers with architecture and implementation.

---

# Question 7

## Original Question

Your company is migrating to the AWS Cloud. As the network administrator, you are responsible for managing the physical network in the datacenter. What cloud role might you transition to that would be the closest fit to your current role?

### Correct Answer

**Cloud Network Engineer**

### Business Problem

Networking career transition.

### Service Category

Networking

### Service

VPC, Route Tables, Direct Connect, Transit Gateway

### Trigger Words

* network administrator
* networking
* migration

### Why This Is Correct

Traditional networking skills translate directly to AWS networking services.

---

# Question 8

## Original Question

A company wants to migrate their on-premises database to Amazon EC2. This database holds data that needs to be accessed quickly and requires high performance. Which EC2 instance type would be BEST suited for this scenario?

### Correct Answer

**Memory Optimized Instance**

### Business Problem

High-performance database hosting.

### Service Category

Compute

### Service

Memory Optimized EC2

### Trigger Words

* database
* high performance
* low latency

### Why This Is Correct

Memory optimized instances are designed for large in-memory databases.

---

# Question 9

## Original Question

Your customer wants to know how security and compliance is shared between AWS and the customer. Under the AWS Shared Responsibility Model, what are your suggested shared controls between the customer and AWS?

### Correct Answer

**Patch Management, Configuration Management, Awareness & Training**

### Business Problem

Understand shared controls.

### Service Category

Security

### Service

Shared Responsibility Model

### Trigger Words

* shared controls
* compliance
* responsibility

### Why This Is Correct

Certain controls require participation from both AWS and customers.

---

# Question 10

## Original Question

A small startup company wants to deploy a new web application in the cloud. The company's IT team is familiar with AWS and has decided to use Amazon EC2 for the deployment. The budget is limited and they want to minimize the cost of running the application. Which of the following options should the company choose to minimize the cost of running the application on Amazon EC2?

**(Select TWO)**

* A. On-Demand Instances
* B. Reserved Instances
* C. Spot Instances
* D. Auto Scaling Groups
* E. Dedicated Instances

---

# Correct Answers

## ✅ B. Reserved Instances

## ✅ D. Auto Scaling Groups

---

# CLF-C02 Exam Strategy

## Business Problem

Deploy a production web application on Amazon EC2 while minimizing infrastructure costs.

## Service Category

Billing & Cost Optimization

## Services

* Reserved Instances
* Auto Scaling Groups

---

# Trigger Words

| Trigger Words        | Think              |
| -------------------- | ------------------ |
| Web Application      | EC2                |
| Limited Budget       | Cost Optimization  |
| Minimize Cost        | Reserved Instances |
| Reduce Waste         | Auto Scaling       |
| Predictable Workload | Reserved Instances |
| Variable Demand      | Auto Scaling       |

---

# Why B. Reserved Instances Is Correct

Reserved Instances provide significant discounts compared to On-Demand pricing when a workload is predictable and expected to run continuously.

### Benefits

* Lower hourly cost
* Predictable pricing
* Ideal for long-running workloads
* 1-year or 3-year commitment options

### Business Outcome

```text
Predictable Web Application
            ↓
Reserved Instances
            ↓
Lower Compute Cost
```

---

# Why D. Auto Scaling Groups Is Correct

Auto Scaling automatically adjusts the number of EC2 instances based on application demand.

### Benefits

* Eliminates overprovisioning
* Reduces idle infrastructure
* Improves cost efficiency
* Supports dynamic workloads

### Business Outcome

```text
Low Traffic
      ↓
2 Instances

High Traffic
      ↓
10 Instances

Result:
Only Pay For What You Need
```

---

# Why A. On-Demand Instances Is Incorrect

On-Demand pricing provides maximum flexibility but does not provide cost discounts.

### When To Use

* Short-term workloads
* Testing environments
* Unpredictable workloads

### Why Eliminate

The question specifically asks:

> "Minimize cost"

On-Demand is usually the most expensive pricing model.

---

# Why C. Spot Instances Is Incorrect

Spot Instances provide the lowest-cost compute capacity but may be interrupted by AWS with little notice.

### When To Use

* Batch processing
* Fault-tolerant workloads
* Data analytics
* Background jobs

### Why Eliminate

This scenario involves a production web application.

```text
Customer Traffic
       ↓
Spot Instance Interrupted
       ↓
Potential Application Outage
```

AWS generally expects Spot Instances to be used for interruptible workloads, not as the primary hosting mechanism for a startup's production web application.

---

# Why E. Dedicated Instances Is Incorrect

Dedicated Instances run on hardware dedicated to a single customer.

### Benefits

* Hardware isolation
* Compliance requirements
* Regulatory requirements

### Why Eliminate

Dedicated Instances increase infrastructure costs.

The scenario specifically states:

> "The budget is limited."

Dedicated Instances are typically among the most expensive deployment options.

---

# Similar Service Differentiation Table

| Service             | Cost Impact                 | Best Use Case           |
| ------------------- | --------------------------- | ----------------------- |
| On-Demand Instances | Highest Cost                | Short-Term Workloads    |
| Reserved Instances  | Lower Cost                  | Predictable Workloads   |
| Spot Instances      | Lowest Cost                 | Interruptible Workloads |
| Auto Scaling Groups | Reduces Waste               | Variable Demand         |
| Dedicated Instances | Highest Infrastructure Cost | Compliance / Isolation  |

---

# Exam Memory Aid

```text
Predictable Workload
        ↓
Reserved Instances

Variable Demand
        ↓
Auto Scaling

Interruptible Workload
        ↓
Spot Instances

Compliance / Isolation
        ↓
Dedicated Instances
```

---

# CLF-C02 Takeaway

This question tests two major AWS cost optimization concepts:

1. Reserved Instances reduce the cost of predictable EC2 workloads.
2. Auto Scaling reduces waste by dynamically adjusting capacity based on demand.

### Final Answers

✅ B. Reserved Instances

✅ D. Auto Scaling Groups


# Question 11

## Original Question

An e-commerce company wants to modernize their infrastructure and move it to the AWS Cloud. Which option can BEST assist the company to realize these goals?

**A. AWS App Runner**

**B. AWS Partner Network (APN)**

**C. AWS Artifact**

**D. Amazon EC2**

---

# Correct Answer

## ✅ B. AWS Partner Network (APN)

---

# Business Problem

The company wants assistance modernizing infrastructure and migrating workloads to AWS but may not have the expertise required to perform the transformation independently.

---

# Service Category

Cloud Adoption & Migration

---

# Service

AWS Partner Network (APN)

---

# Trigger Words

| Trigger Words            | Think                   |
| ------------------------ | ----------------------- |
| Modernize Infrastructure | Cloud Adoption          |
| Move to AWS              | Migration               |
| Assistance               | AWS Partner Network     |
| AWS Expertise            | AWS Partner Network     |
| Transformation           | AWS Consulting Partners |
| Guidance                 | AWS Partner Network     |

---

# Why This Is Correct

The AWS Partner Network (APN) is a global network of AWS Partners that help customers:

* Design cloud architectures
* Migrate applications
* Modernize infrastructure
* Implement cloud-native solutions
* Accelerate cloud adoption

The question asks:

> "Which option can BEST assist the company?"

The key phrase is:

**BEST assist**

This points to a program that provides expertise and guidance rather than a technical AWS service.

---

# Business Problem → Service Category → Service

```text
Need Help Modernizing Infrastructure
                ↓
Cloud Adoption & Migration
                ↓
AWS Partner Network (APN)
```

---

# Why A. AWS App Runner Is Incorrect

### What It Does

AWS App Runner is a fully managed service used to deploy web applications and APIs.

### Why Eliminate

The question is not asking:

> "How do I run an application?"

It is asking:

> "How do I get assistance modernizing my environment?"

App Runner is a deployment service, not a modernization consulting service.

---

# Why C. AWS Artifact Is Incorrect

### What It Does

AWS Artifact provides:

* Compliance reports
* Security certifications
* Audit documentation

### Why Eliminate

Artifact supports governance and compliance.

It does not help customers modernize or migrate workloads.

---

# Why D. Amazon EC2 Is Incorrect

### What It Does

Amazon EC2 provides virtual servers in the cloud.

### Why Eliminate

EC2 is a compute service.

The question asks for assistance with modernization, not compute infrastructure.

---

# Similar Services to Eliminate

| Service                   | Purpose                                | Why Not Correct                      |
| ------------------------- | -------------------------------------- | ------------------------------------ |
| AWS App Runner            | Managed application hosting            | Does not provide migration expertise |
| AWS Artifact              | Compliance documentation               | Compliance-focused service           |
| Amazon EC2                | Virtual servers                        | Compute service only                 |
| AWS Partner Network (APN) | Migration and modernization assistance | ✅ Correct Answer                     |

---

# Exam Memory Aid

```text
Need AWS Expertise
        ↓
AWS Partner Network (APN)

Need Compliance Reports
        ↓
AWS Artifact

Need Virtual Servers
        ↓
Amazon EC2

Need Managed Web App Hosting
        ↓
AWS App Runner
```

---

# CLF-C02 Takeaway

When the question asks:

* Who can help migrate workloads?
* Who can help modernize infrastructure?
* Who can provide AWS expertise?
* Who can assist with cloud transformation?

Think:

## ✅ AWS Partner Network (APN)

This is a common CLF-C02 pattern where the correct answer is an AWS program or ecosystem resource rather than a technical service.


---

# Question 12

## Original Question

Your application is running on Amazon EC2 instances. Which component of the AWS global infrastructure will you use to make your application resilient and highly available?

### Correct Answer

**Availability Zones**

### Business Problem

High availability.

### Service Category

Global Infrastructure

### Service

Availability Zones

### Trigger Words

* resilient
* highly available
* fault tolerant

### Why This Is Correct

Availability Zones isolate failures within a Region.

---

# Question 13

## Original Question

Your company has a batch job that runs twice a week for 30 minutes to catalog certain items and is tolerant to interruptions. Which pricing model would meet the requirements and be the most cost effective?

### Correct Answer

**Spot Instances**

### Business Problem

Interruptible batch processing.

### Service Category

Billing & Cost Optimization

### Service

Spot Instances

### Trigger Words

* batch job
* interruptions
* cost effective

### Why This Is Correct

Spot Instances are ideal for interruptible workloads.

---

# Question 14

## Original Question

A company has an on-premises application that runs on virtual machines and uses a relational database in the backend. As the company migrates to the cloud, it is planning to leverage cloud native services. Which migration strategy is the company adopting in this scenario?

### Correct Answer

**Refactor / Re-Architect**

### Business Problem

Application modernization.

### Service Category

Migration Strategies

### Service

Refactor

### Trigger Words

* cloud native
* modernization
* redesign

### Why This Is Correct

Refactoring modifies applications to take advantage of cloud-native services.

---

# Question 15

## Original Question

You are employed at a company that is highly regulated. You are tasked with monitoring operational and risk auditing as well as compliance of your AWS account. Which AWS service can help you meet these audit requirements?

### Correct Answer

**AWS Config**

### Business Problem

Compliance monitoring.

### Service Category

Governance

### Service

AWS Config

### Trigger Words

* compliance
* auditing
* monitoring

### Why This Is Correct

AWS Config continuously evaluates resource compliance.

---

# Question 16

## Original Question

Your application has a global reach and you would like to provide low latency access to your application globally by using Amazon CloudFront. What component of the AWS Global Infrastructure does Amazon CloudFront use?

### Correct Answer

**Edge Locations**

### Business Problem

Global content delivery.

### Service Category

Networking

### Service

CloudFront

### Trigger Words

* low latency
* global users
* CloudFront

### Why This Is Correct

CloudFront caches content in Edge Locations close to users.

---

# Question 17

## Original Question

An enterprise is heavily dependent on their on-premises data center and are considering a potential migration to the cloud. One of the major concerns is security. How does AWS maintain the security and privacy of customer data?

### Correct Answer

**Through the Shared Responsibility Model and security controls built into AWS infrastructure**

### Business Problem

Data security and privacy.

### Service Category

Security

### Service

Shared Responsibility Model

### Trigger Words

* security
* privacy
* migration

### Why This Is Correct

AWS secures the cloud infrastructure while customers secure their data and configurations.

---

# Question 18

## Original Question

You are working in a start-up company, which uses various AWS services. They have recently noticed a spike in the monthly AWS bill. The CTO is concerned about the cost and wants to act to reduce it. Which AWS service would be most effective on controlling AWS costs in this scenario?

### Correct Answer

**AWS Budgets**

### Business Problem

Control spending.

### Service Category

Billing & Cost Optimization

### Service

AWS Budgets

### Trigger Words

* cost spike
* spending control
* budget

### Why This Is Correct

AWS Budgets provides proactive alerts and controls.

---

# Question 19

## Original Question

A company has its application servers deployed in an AWS region in Amazon VPCs with private and public subnets. The application servers are placed in private subnets and often initiate requests to the internet. Which solution would BEST accomplish this task?

### Correct Answer

**NAT Gateway**

### Business Problem

Outbound internet access from private subnets.

### Service Category

Networking

### Service

NAT Gateway

### Trigger Words

* private subnet
* internet access
* outbound requests

### Why This Is Correct

A NAT Gateway allows private subnet resources to access the internet while remaining private.

### Similar Services to Eliminate

| Service          | Why Eliminate          |
| ---------------- | ---------------------- |
| Internet Gateway | Used by public subnets |
| Route 53         | DNS service            |
| Load Balancer    | Traffic distribution   |
