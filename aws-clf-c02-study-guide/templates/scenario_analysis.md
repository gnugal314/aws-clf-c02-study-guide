# AWS CLF-C02 Scenario Analysis

## Business Problem → Service Category → Service Framework

---

# Question 1

## Question

Your colleague wants to create certain Amazon EC2 and Amazon S3 resources in an automated fashion using AWS CloudFormation. However, they reached out to you asking for help to understand pricing. Which option will provide them with the information they need?

**A.** AWS will charge for Amazon EC2 and Amazon S3. There is no charge for AWS CloudFormation.

**B.** You will be priced for Amazon EC2 and Amazon S3 only. The Amazon EC2 pricing will not vary depending on the region.

**C.** You will be charged for AWS CloudFormation, Amazon EC2 and Amazon S3. The Amazon EC2 pricing will not vary depending on the region.

**D.** You will be charged for AWS CloudFormation, Amazon EC2 and Amazon S3. The Amazon EC2 pricing will vary depending on the region.

---

# Correct Answer

## ✅ A. AWS will charge for Amazon EC2 and Amazon S3. There is no charge for AWS CloudFormation.

---

# CLF-C02 Exam Strategy

## Business Problem

Understand AWS pricing when provisioning infrastructure using Infrastructure as Code (IaC).

## Service Category

Billing & Cost Optimization

## Service

AWS CloudFormation

---

# Trigger Words

| Trigger Words           | Think                       |
| ----------------------- | --------------------------- |
| CloudFormation          | Infrastructure as Code      |
| Automated deployment    | CloudFormation              |
| Provision AWS resources | CloudFormation              |
| Pricing                 | Billing & Cost Optimization |

---

# Why This Is Correct

AWS CloudFormation itself is **free**.

CloudFormation is an orchestration service that creates and manages AWS resources.

You are charged only for the resources created by CloudFormation.

Examples include:

* Amazon EC2
* Amazon S3
* Amazon RDS
* AWS Lambda
* Elastic Load Balancers

### Architecture Concept

```text
CloudFormation Template
          ↓
Creates Resources
          ↓
EC2, S3, RDS, Lambda
          ↓
Charges Apply To Resources
```

CloudFormation acts as the deployment engine.

The deployed resources generate the charges.

---

# Why Option B Is Incorrect

### Statement

> You will be priced for Amazon EC2 and Amazon S3 only. The Amazon EC2 pricing will not vary depending on the region.

### Analysis

The first statement is correct.

The second statement is incorrect.

Amazon EC2 pricing varies by AWS Region.

### Example

| Region                | Pricing   |
| --------------------- | --------- |
| US East (N. Virginia) | Lower     |
| Europe (Frankfurt)    | Different |
| Asia Pacific (Tokyo)  | Different |

---

# Why Option C Is Incorrect

### Statement

> You will be charged for AWS CloudFormation, Amazon EC2 and Amazon S3.

### Analysis

CloudFormation is free.

Because this statement incorrectly charges for CloudFormation, the answer is incorrect.

---

# Why Option D Is Incorrect

### Statement

> You will be charged for AWS CloudFormation, Amazon EC2 and Amazon S3. The Amazon EC2 pricing will vary depending on the region.

### Analysis

The region pricing statement is true.

However, CloudFormation is still free.

Since the answer incorrectly states CloudFormation incurs charges, the answer is incorrect.

---

# Similar Services To Eliminate

| Service             | Why Eliminate                                                 |
| ------------------- | ------------------------------------------------------------- |
| Cost Explorer       | Analyzes existing AWS spend                                   |
| AWS Budgets         | Creates spending alerts                                       |
| Cost & Usage Report | Historical billing details                                    |
| Pricing Calculator  | Estimates future costs but is not the answer to this question |

---

# Key CLF-C02 Exam Concepts

## Infrastructure as Code (IaC)

CloudFormation allows you to define infrastructure using code templates.

## AWS Managed Service Pricing

Many AWS management services are free.

Examples:

| Service        | Charged? |
| -------------- | -------- |
| CloudFormation | No       |
| IAM            | No       |
| VPC            | No       |
| Organizations  | No       |
| EC2            | Yes      |
| S3             | Yes      |
| RDS            | Yes      |

---

# Fast Recall Memory Aid

## Question Pattern

> "I am using CloudFormation. What am I paying for?"

### Correct Response

You pay for:

* EC2
* S3
* RDS
* Lambda
* Other provisioned resources

You do NOT pay for:

* CloudFormation itself

---

# Exam Takeaway

When you see:

**CloudFormation**

Ask yourself:

> "Am I paying for CloudFormation or the resources it creates?"

### Correct Answer

You pay for the resources.

CloudFormation itself is free.

**Final Answer: A**


---

# Question 2

## Question

During a recent outage a number of static file uploads were lost and irretrievable. Your manager has tasked you with finding a more durable solution. Which service could be used with the least operational overhead?

### Business Problem

Durable file storage.

### Service Category

Storage

### Service

Amazon S3

### Trigger Words

* static files
* durability
* lost uploads
* minimal operational overhead

### Why This Is Correct

Amazon S3 provides 99.999999999% durability and is fully managed.

### Eliminate Similar Services

| Service        | Why Eliminate     |
| -------------- | ----------------- |
| EBS            | Attached to EC2   |
| EFS            | Shared filesystem |
| Instance Store | Temporary storage |

---

# Question 3

## Question

Your company wants you to focus on running and monitoring your cloud applications in a way that drives continuous improvement to procedures and processes. Which AWS Well-Architected pillar will help you identify the responsibilities in this scenario?

### Business Problem

Improve operational processes.

### Service Category

Well-Architected Framework

### Service

Operational Excellence Pillar

### Trigger Words

* continuous improvement
* monitoring
* operations
* procedures

### Why This Is Correct

Operational Excellence focuses on monitoring, automation, and continual improvement.

### Eliminate Similar Pillars

| Pillar            | Why Eliminate      |
| ----------------- | ------------------ |
| Reliability       | Availability focus |
| Security          | Protection focus   |
| Cost Optimization | Cost focus         |

---

# Question 4

## Question

Your company is deploying a web application in AWS running on several Amazon EC2 instances. What is the responsibility of AWS under the shared responsibility model?

### Business Problem

Determine AWS responsibilities.

### Service Category

Security

### Service

Security OF the Cloud

### Trigger Words

* shared responsibility
* EC2
* AWS responsibility

### Why This Is Correct

AWS manages:

* hardware
* networking infrastructure
* data centers
* physical security

### Eliminate Customer Responsibilities

| Responsibility  | Owner    |
| --------------- | -------- |
| OS patching     | Customer |
| Security groups | Customer |
| IAM permissions | Customer |

---

# Question 5

## Question

Your company's finance team wants to use their own business intelligence tool to visualize cost and usage. They want detailed billing line items for the last three years automatically available in a persistent store for their business intelligence tool without writing any scripts.

### Business Problem

Detailed billing exports.

### Service Category

Billing & Cost Optimization

### Service

Cost & Usage Report (CUR)

### Trigger Words

* detailed billing
* line items
* BI tool
* historical costs

### Why This Is Correct

CUR provides the most detailed billing and usage information.

### Eliminate Similar Services

| Service            | Why Eliminate      |
| ------------------ | ------------------ |
| Cost Explorer      | Visualization only |
| AWS Budgets        | Alerts only        |
| Pricing Calculator | Future estimates   |

---

# Question 6

## Question

A customer would like to design and build a new workload on the AWS Cloud but does not have the AWS expertise to get started.

### Business Problem

AWS implementation assistance.

### Service Category

Cloud Adoption

### Service

AWS Professional Services

### Trigger Words

* lacks expertise
* design workload
* build workload

### Why This Is Correct

AWS Professional Services helps customers architect and implement solutions.

### Eliminate Similar Services

| Service         | Why Eliminate                      |
| --------------- | ---------------------------------- |
| Trusted Advisor | Recommendations only               |
| Support Plans   | Support, not architecture services |

---

# Question 7

## Question

Your company is migrating to the AWS Cloud. As the network administrator, you are responsible for managing the physical network in the datacenter. What cloud role might you transition to?

### Business Problem

Cloud networking career alignment.

### Service Category

Networking

### Service

Cloud Network Engineer

### Trigger Words

* network administrator
* networking
* migration

### Why This Is Correct

Networking skills directly transfer to:

* VPC
* Route Tables
* Transit Gateway
* Direct Connect

---

# Question 8

## Question

A company wants to migrate their on-premises database to Amazon EC2. This database holds data that needs to be accessed quickly and requires high performance.

### Business Problem

High-performance database hosting.

### Service Category

Compute

### Service

Memory Optimized EC2 Instance

### Trigger Words

* database
* high performance
* low latency

### Why This Is Correct

Memory Optimized instances are designed for large in-memory databases.

### Eliminate Similar Services

| Instance Type     | Why Eliminate            |
| ----------------- | ------------------------ |
| General Purpose   | Balanced workloads       |
| Compute Optimized | CPU intensive            |
| Storage Optimized | Storage throughput focus |

---

# Question 9

## Question

Your customer wants to know how security and compliance is shared between AWS and the customer.

### Business Problem

Shared Responsibility Model.

### Service Category

Security

### Service

Shared Controls

### Trigger Words

* shared controls
* compliance
* shared responsibility

### Why This Is Correct

Both AWS and customer participate in:

* patch management
* configuration management
* awareness training

---

# Question 10

## Question

A startup company wants to minimize the cost of running Amazon EC2.

### Business Problem

Lowest-cost compute.

### Service Category

Billing & Cost Optimization

### Service

Spot Instances

### Trigger Words

* minimize cost
* lowest cost
* EC2

### Why This Is Correct

Spot Instances provide the lowest-cost EC2 pricing.

### Eliminate Similar Services

| Service            | Why Eliminate       |
| ------------------ | ------------------- |
| On-Demand          | Higher cost         |
| Reserved Instances | Commitment required |
| Savings Plans      | Commitment required |

---

# Question 11

## Question

An e-commerce company wants to modernize their infrastructure and move it to the AWS Cloud.

### Business Problem

Cloud adoption and modernization.

### Service Category

Cloud Benefits

### Service

Agility and Elasticity

### Trigger Words

* modernize
* cloud migration
* transformation

### Why This Is Correct

AWS enables faster innovation, scalability, and operational agility.

---

# Question 12

## Question

Your application is running on Amazon EC2 instances. Which component of the AWS global infrastructure will you use to make your application resilient and highly available?

### Business Problem

High availability.

### Service Category

Global Infrastructure

### Service

Availability Zones

### Trigger Words

* resilient
* highly available
* fault tolerance

### Why This Is Correct

Availability Zones provide isolation from failures.

### Eliminate Similar Services

| Service       | Why Eliminate         |
| ------------- | --------------------- |
| Region        | Too broad             |
| Edge Location | Content delivery only |

---

# Question 13

## Question

A batch job runs twice a week for 30 minutes and is tolerant to interruptions.

### Business Problem

Lowest-cost interruptible workload.

### Service Category

Billing & Cost Optimization

### Service

Spot Instances

### Trigger Words

* batch job
* tolerant to interruptions
* cost effective

### Why This Is Correct

Spot Instances are ideal for interruptible workloads.

---

# Question 14

## Question

A company is migrating to cloud-native services.

### Business Problem

Application modernization.

### Service Category

Migration Strategies

### Service

Refactor / Re-Architect

### Trigger Words

* cloud native
* modernization
* redesign

### Why This Is Correct

Refactoring modifies applications to use cloud-native services.

### Eliminate Similar Strategies

| Strategy | Why Eliminate   |
| -------- | --------------- |
| Rehost   | Lift-and-shift  |
| Relocate | Hypervisor move |
| Retain   | No migration    |

---

# Question 15

## Question

A highly regulated company needs operational, risk, and compliance auditing.

### Business Problem

Compliance auditing.

### Service Category

Governance

### Service

AWS Config

### Trigger Words

* compliance
* auditing
* resource tracking

### Why This Is Correct

AWS Config tracks resource configurations and compliance.

### Eliminate Similar Services

| Service    | Why Eliminate     |
| ---------- | ----------------- |
| CloudWatch | Monitoring        |
| CloudTrail | API activity only |

---

# Question 16

## Question

You want global low-latency access using CloudFront.

### Business Problem

Global content delivery.

### Service Category

Networking

### Service

Edge Locations

### Trigger Words

* CloudFront
* low latency
* global users

### Why This Is Correct

CloudFront uses Edge Locations for caching.

### Eliminate Similar Components

| Component         | Why Eliminate   |
| ----------------- | --------------- |
| Region            | Hosts resources |
| Availability Zone | Fault isolation |

---

# Question 17

## Question

How does AWS maintain the security and privacy of customer data?

### Business Problem

Cloud security.

### Service Category

Security

### Service

Shared Responsibility Model

### Trigger Words

* security
* privacy
* customer data

### Why This Is Correct

AWS secures infrastructure while customers secure data and access.

---

# Question 18

## Question

AWS bill has unexpectedly increased.

### Business Problem

Control AWS costs.

### Service Category

Billing & Cost Optimization

### Service

AWS Budgets

### Trigger Words

* cost spike
* overspending
* cost control

### Why This Is Correct

AWS Budgets proactively alerts on spending thresholds.

### Eliminate Similar Services

| Service       | Why Eliminate  |
| ------------- | -------------- |
| Cost Explorer | Analysis only  |
| CUR           | Reporting only |

---

# Question 19

## Question

Application servers in private subnets need internet access.

### Business Problem

Outbound internet access from private subnet.

### Service Category

Networking

### Service

NAT Gateway

### Trigger Words

* private subnet
* outbound internet
* initiate requests

### Why This Is Correct

NAT Gateway allows private subnet resources to access the internet without accepting inbound internet traffic.

### Eliminate Similar Services

| Service          | Why Eliminate          |
| ---------------- | ---------------------- |
| Internet Gateway | Requires public subnet |
| NAT Instance     | Legacy approach        |
| Route 53         | DNS only               |

### Memory Aid

```text
Public Subnet → Internet Gateway
Private Subnet → NAT Gateway
```
