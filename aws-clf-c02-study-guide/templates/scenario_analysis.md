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

## AWS Expertise and Workload Design Assistance

### Original Question

A customer would like to design and build a new workload on the AWS Cloud but does not have the AWS expertise to get started. Which AWS program can a customer take advantage of to achieve that outcome?

**A. AWS Partner Network (APN) Consulting Partners**

**B. AWS Technical Account Managers (TAMs)**

**C. AWS Support**

**D. AWS Marketplace**

---

# Correct Answer

## ✅ A. AWS Partner Network (APN) Consulting Partners

---

# Business Problem

The customer needs expertise, guidance, and implementation assistance to design and build a new workload on AWS.

---

# Service Category

Cloud Adoption & Migration

---

# Service

AWS Partner Network (APN) Consulting Partners

---

# Trigger Words

| Trigger Words       | Think                     |
| ------------------- | ------------------------- |
| Design a workload   | Architecture expertise    |
| Build a workload    | Implementation assistance |
| Lacks AWS expertise | Consulting Partner        |
| Get started on AWS  | APN Consulting Partner    |
| Cloud adoption      | AWS Partner Network       |

---

# Why This Is Correct

AWS Partner Network (APN) Consulting Partners are organizations that help customers:

* Design AWS architectures
* Build cloud-native solutions
* Migrate workloads
* Modernize applications
* Accelerate cloud adoption

The key phrase in the question is:

> "does not have the AWS expertise"

This immediately points to obtaining external AWS expertise.

### Business Outcome

```text
Customer Needs AWS Expertise
             ↓
Cloud Adoption & Migration
             ↓
APN Consulting Partner
             ↓
Design & Build AWS Workload
```

---

# Business Problem → Service Category → Service

```text
Need AWS Expertise
        ↓
Cloud Adoption & Migration
        ↓
AWS Partner Network (APN)
        ↓
Consulting Partners
```

---

# Why B. AWS Technical Account Managers (TAMs) Is Incorrect

### What It Does

A TAM provides:

* Operational guidance
* Best practices
* Support planning
* Trusted advisor services

### Why Eliminate

TAMs do not typically design and build workloads for customers.

They provide guidance but are not implementation resources.

### Trigger Words for TAM

| Trigger Words        |
| -------------------- |
| Operational guidance |
| Strategic advice     |
| Enterprise support   |

---

# Why C. AWS Support Is Incorrect

### What It Does

AWS Support assists with:

* Technical issues
* Service questions
* Troubleshooting

### Why Eliminate

Support helps resolve issues.

Support does not design and build customer workloads.

### Trigger Words for AWS Support

| Trigger Words   |
| --------------- |
| Troubleshooting |
| Technical issue |
| Service problem |

---

# Why D. AWS Marketplace Is Incorrect

### What It Does

AWS Marketplace provides:

* Third-party software
* SaaS solutions
* Commercial software products

### Why Eliminate

Marketplace helps customers purchase software.

It does not provide workload architecture expertise.

### Trigger Words for Marketplace

| Trigger Words        |
| -------------------- |
| Purchase software    |
| Third-party products |
| SaaS applications    |

---

# Similar Services to Eliminate

| Service                                       | Purpose                            | Why Not Correct           |
| --------------------------------------------- | ---------------------------------- | ------------------------- |
| AWS Partner Network (APN) Consulting Partners | Design and implement AWS solutions | ✅ Correct                 |
| AWS Technical Account Manager (TAM)           | Strategic and operational guidance | Does not build workloads  |
| AWS Support                                   | Technical assistance               | Troubleshooting focus     |
| AWS Marketplace                               | Software procurement               | No architecture expertise |

---

# Exam Memory Aid

```text
Need AWS Expertise
        ↓
APN Consulting Partner

Need Operational Guidance
        ↓
Technical Account Manager (TAM)

Need Technical Support
        ↓
AWS Support

Need Software
        ↓
AWS Marketplace
```

---

# CLF-C02 Takeaway

When you see:

* Customer lacks AWS expertise
* Design a workload
* Build a workload
* Migration assistance
* Cloud adoption help

Think:

## ✅ AWS Partner Network (APN) Consulting Partners

This is a common CLF-C02 pattern where AWS expects you to identify a program or partner ecosystem resource rather than a technical AWS service.


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

(Select TWO)

A. Physical and Environmental controls

B. Identity and access management

C. Data Encryption

D. Awareness and Training

E. Patch Management

# AWS CLF-C02 Scenario Analysis

## AWS Shared Responsibility Model – Shared Controls

---

# Correct Answers

## ✅ D. Awareness and Training

## ✅ E. Patch Management

---

# Business Problem

The customer wants to understand which security and compliance controls are jointly managed by both AWS and the customer.

---

# Service Category

Security

---

# Service

AWS Shared Responsibility Model

---

# Trigger Words

| Trigger Words               | Think                 |
| --------------------------- | --------------------- |
| Shared Responsibility Model | Shared Controls       |
| Shared controls             | AWS + Customer        |
| Security responsibilities   | Shared Responsibility |
| Compliance                  | Shared Controls       |
| Joint ownership             | Shared Controls       |

---

# Why These Answers Are Correct

AWS classifies security controls into:

* Inherited Controls
* Shared Controls
* Customer-Specific Controls

### Shared Controls

Shared controls require participation from both AWS and the customer.

Examples include:

* Patch Management
* Configuration Management
* Awareness and Training

---

## ✅ D. Awareness and Training

Both AWS and customers participate in security awareness and training.

### AWS Responsibilities

* AWS trains AWS employees
* AWS maintains security programs

### Customer Responsibilities

* Customer trains their users and administrators
* Customer develops security awareness programs

### Business Outcome

```text
Security Awareness
        ↓
AWS Training Programs
        +
Customer Training Programs
        ↓
Shared Control
```

---

## ✅ E. Patch Management

Patch management is considered a shared control because responsibility depends on the service model.

### AWS Responsibilities

AWS patches:

* Physical infrastructure
* Managed service infrastructure

### Customer Responsibilities

Customers patch:

* Operating systems on EC2
* Applications
* Middleware

### Business Outcome

```text
Infrastructure Patching
         ↓
AWS

Guest OS Patching
         ↓
Customer

Result
         ↓
Shared Control
```

---

# Business Problem → Service Category → Service

```text
Need To Understand Security Ownership
                  ↓
Security
                  ↓
Shared Responsibility Model
                  ↓
Shared Controls
                  ↓
Awareness & Training
Patch Management
```

---

# Why A. Physical and Environmental Controls Is Incorrect

### What It Is

Physical security includes:

* Data centers
* Physical access controls
* Environmental protections

### Why Eliminate

These are fully managed by AWS.

Customers have no responsibility for AWS data center operations.

### Ownership

```text
Physical Security
        ↓
AWS Only
```

---

# Why B. Identity and Access Management Is Incorrect

### What It Is

IAM controls:

* Users
* Roles
* Policies
* Permissions

### Why Eliminate

IAM is considered a customer responsibility.

Customers determine:

* Who gets access
* What permissions are granted
* How authentication is configured

### Ownership

```text
IAM
  ↓
Customer Responsibility
```

---

# Why C. Data Encryption Is Incorrect

### What It Is

Data protection through encryption.

### Why Eliminate

Customers are generally responsible for:

* Choosing encryption settings
* Managing encryption policies
* Managing encryption keys (when applicable)

Encryption is typically considered a customer control rather than a shared control.

### Ownership

```text
Data Encryption
        ↓
Customer Responsibility
```

---

# Similar Controls to Eliminate

| Control                           | Ownership | Why Not Correct   |
| --------------------------------- | --------- | ----------------- |
| Physical & Environmental Controls | AWS       | Inherited control |
| Identity & Access Management      | Customer  | Customer control  |
| Data Encryption                   | Customer  | Customer control  |
| Awareness & Training              | Shared    | ✅ Correct         |
| Patch Management                  | Shared    | ✅ Correct         |

---

# Shared Responsibility Quick Reference

| Responsibility       | AWS | Customer | Shared |
| -------------------- | --- | -------- | ------ |
| Physical Security    | ✅   | ❌        | ❌      |
| Data Centers         | ✅   | ❌        | ❌      |
| IAM                  | ❌   | ✅        | ❌      |
| Data Encryption      | ❌   | ✅        | ❌      |
| Awareness & Training | ❌   | ❌        | ✅      |
| Patch Management     | ❌   | ❌        | ✅      |

---

# Exam Memory Aid

```text
Security OF The Cloud
          ↓
AWS

Security IN The Cloud
          ↓
Customer

Shared Controls
          ↓
Patch Management
Awareness & Training
```

---

# CLF-C02 Takeaway

When you see:

* Shared Responsibility Model
* Shared controls
* Security ownership
* Compliance responsibilities

Think:

## ✅ Awareness and Training

## ✅ Patch Management

These are the two most commonly tested examples of shared controls because both AWS and the customer contribute to their successful implementation.


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

---

## Reducing Amazon EC2 Spend

### Original Question

A large enterprise organization with many affiliates has migrated all of their on-premises steady-state workloads to the AWS Cloud. They notice a significant increase in Amazon EC2 spend over the last several months. Which of the following should they purchase to reduce the EC2 spend?

**(Select TWO)**

**A. AWS Cost Explorer**

**B. Savings Plans**

**C. AWS Budgets**

**D. AWS Trusted Advisor**

**E. Reserved Instances**

---

# Correct Answers

## ✅ B. Savings Plans

## ✅ E. Reserved Instances

---

# Business Problem

The organization has predictable, steady-state workloads running continuously on Amazon EC2 and wants to reduce long-term compute costs.

---

# Service Category

Billing & Cost Optimization

---

# Services

* Savings Plans
* Reserved Instances

---

# Trigger Words

| Trigger Words            | Think                               |
| ------------------------ | ----------------------------------- |
| Steady-state workloads   | Predictable usage                   |
| Running for months       | Long-term commitment                |
| Reduce EC2 spend         | Savings Plans or Reserved Instances |
| Large enterprise         | Significant compute usage           |
| Purchase to reduce costs | Commitment-based discounts          |

---

# Why These Answers Are Correct

## ✅ B. Savings Plans

Savings Plans provide discounted pricing in exchange for a commitment to a consistent amount of compute usage.

### Benefits

* Lower compute costs
* Flexible across eligible compute services
* Easier management than Reserved Instances
* Ideal for long-running workloads

### Business Outcome

```text
Predictable Compute Usage
            ↓
Savings Plans
            ↓
Lower AWS Bill
```

---

## ✅ E. Reserved Instances

Reserved Instances provide discounted EC2 pricing for workloads that run continuously.

### Benefits

* Significant EC2 discounts
* Ideal for predictable workloads
* One-year or three-year commitment

### Business Outcome

```text
Steady-State EC2 Workloads
            ↓
Reserved Instances
            ↓
Reduced EC2 Spend
```

---

# Business Problem → Service Category → Service

```text
Need To Reduce Long-Term EC2 Costs
                ↓
Billing & Cost Optimization
                ↓
Savings Plans
                ↓
Reserved Instances
```

---

# Why A. AWS Cost Explorer Is Incorrect

### What It Does

Cost Explorer analyzes and visualizes AWS spending.

### Why Eliminate

Cost Explorer helps identify cost trends but does not directly reduce costs.

### Trigger Words

* analyze spending
* visualize costs
* cost reporting

---

# Why C. AWS Budgets Is Incorrect

### What It Does

AWS Budgets creates alerts when spending thresholds are exceeded.

### Why Eliminate

Budgets help monitor costs but do not provide discounts.

### Trigger Words

* spending alerts
* budget thresholds
* notifications

---

# Why D. AWS Trusted Advisor Is Incorrect

### What It Does

Trusted Advisor provides recommendations for:

* Cost optimization
* Security
* Performance
* Reliability

### Why Eliminate

Trusted Advisor can recommend cost-saving opportunities but does not itself provide discounted pricing.

### Trigger Words

* recommendations
* best practices
* optimization guidance

---

# Similar Services to Eliminate

| Service             | Purpose                        | Why Not Correct                |
| ------------------- | ------------------------------ | ------------------------------ |
| AWS Cost Explorer   | Cost analysis and reporting    | Does not reduce costs directly |
| AWS Budgets         | Spending alerts                | Does not reduce costs directly |
| AWS Trusted Advisor | Recommendations                | Does not provide discounts     |
| Savings Plans       | Flexible compute discounts     | ✅ Correct                      |
| Reserved Instances  | Predictable workload discounts | ✅ Correct                      |

---

# Cost Optimization Differentiation Table

| Service            | Primary Benefit                      |
| ------------------ | ------------------------------------ |
| Savings Plans      | Flexible long-term compute discounts |
| Reserved Instances | EC2-specific long-term discounts     |
| Cost Explorer      | Cost analysis                        |
| AWS Budgets        | Cost alerts                          |
| Trusted Advisor    | Cost recommendations                 |

---

# Exam Memory Aid

```text
Need To Reduce Costs
         ↓
Purchase Discounts
         ↓
Savings Plans
Reserved Instances

Need To Analyze Costs
         ↓
Cost Explorer

Need Cost Alerts
         ↓
AWS Budgets

Need Recommendations
         ↓
Trusted Advisor
```

---

# CLF-C02 Takeaway

When you see:

* Steady-state workloads
* Predictable usage
* Long-running EC2 instances
* Reduce EC2 spend
* Purchase something to lower costs

Think:

## ✅ Savings Plans

## ✅ Reserved Instances

These are the two primary AWS purchasing models designed specifically to reduce the cost of predictable compute workloads.


---

## Amazon EC2 Instance Purchasing Option

### Original Question

Your marketing team wants to run a one-day campaign to get some feedback on an upcoming product launch. You need to provision the application on an Amazon EC2 instance and it must function without interruption. Which type of instance can you use?

**A. Spot Instance**

**B. Dedicated Instance**

**C. Reserved Instance**

**D. On-Demand Instance**

---

# Correct Answer

## ✅ D. On-Demand Instance

---

# Business Problem

Deploy a short-term EC2 workload that must remain available for the duration of a one-day marketing campaign without interruption.

---

# Service Category

Billing & Cost Optimization

---

# Service

Amazon EC2 On-Demand Instance

---

# Trigger Words

| Trigger Words                      | Think               |
| ---------------------------------- | ------------------- |
| One-day campaign                   | Short-term workload |
| Temporary workload                 | On-Demand           |
| Must function without interruption | Stable capacity     |
| No long-term commitment            | On-Demand           |
| Immediate deployment               | On-Demand           |

---

# Why This Is Correct

On-Demand Instances are designed for:

* Short-term workloads
* Temporary projects
* Unpredictable usage patterns
* Immediate deployment
* No long-term commitment

The application must run:

* For only one day
* Without interruption

On-Demand provides guaranteed availability without requiring a commitment.

---

# Business Problem → Service Category → Service

```text
One-Day Marketing Campaign
            ↓
Short-Term Compute Need
            ↓
Billing & Cost Optimization
            ↓
On-Demand Instance
```

---

# Why A. Spot Instance Is Incorrect

### What It Does

Spot Instances provide the lowest-cost EC2 pricing by using unused AWS capacity.

### Why Eliminate

Spot Instances can be interrupted by AWS with little notice.

The question explicitly states:

> "must function without interruption"

This immediately eliminates Spot Instances.

### Trigger Words

| Trigger Words          | Think |
| ---------------------- | ----- |
| Lowest cost            | Spot  |
| Interruptible workload | Spot  |
| Batch processing       | Spot  |

---

# Why B. Dedicated Instance Is Incorrect

### What It Does

Dedicated Instances run on hardware dedicated to a single customer.

### Why Eliminate

Dedicated Instances are typically selected for:

* Compliance requirements
* Regulatory requirements
* Hardware isolation

Nothing in the scenario indicates a need for dedicated hardware.

Additionally, Dedicated Instances cost more than necessary.

---

# Why C. Reserved Instance Is Incorrect

### What It Does

Reserved Instances provide discounted pricing for predictable workloads through a one-year or three-year commitment.

### Why Eliminate

The workload only runs for:

> One day

Reserved Instances are intended for long-running workloads.

A one-day campaign does not justify a long-term commitment.

### Trigger Words

| Trigger Words            | Think             |
| ------------------------ | ----------------- |
| Predictable workload     | Reserved Instance |
| Long-running application | Reserved Instance |
| One-year commitment      | Reserved Instance |

---

# Similar Services to Eliminate

| Service            | Purpose                           | Why Not Correct           |
| ------------------ | --------------------------------- | ------------------------- |
| Spot Instance      | Lowest-cost interruptible compute | Can be interrupted        |
| Dedicated Instance | Single-tenant hardware            | Unnecessary and expensive |
| Reserved Instance  | Long-term discounted compute      | Requires commitment       |
| On-Demand Instance | Short-term reliable compute       | ✅ Correct                 |

---

# Pricing Model Differentiation Table

| Pricing Model      | Best Used For                     |
| ------------------ | --------------------------------- |
| On-Demand          | Short-term workloads              |
| Reserved Instance  | Predictable long-term workloads   |
| Spot Instance      | Interruptible workloads           |
| Dedicated Instance | Compliance and hardware isolation |

---

# Exam Memory Aid

```text
Short-Term Workload
        ↓
On-Demand

Long-Term Predictable Workload
        ↓
Reserved Instance

Interruptible Workload
        ↓
Spot Instance

Compliance Requirement
        ↓
Dedicated Instance
```

---

# CLF-C02 Takeaway

When you see:

* Temporary project
* One-time event
* Short-duration workload
* Immediate deployment
* Must not be interrupted

Think:

## ✅ On-Demand Instance

This is one of the most common CLF-C02 pricing questions and tests your ability to differentiate between EC2 purchasing options based on workload characteristics.


---

## Cloud Procurement Strategy

### Original Question

Your company is new to AWS and has started its cloud adoption journey. You are worried that the company will encounter challenges using traditional procurement strategies and will need to adapt. What are the characteristics of a cloud procurement strategy?

**(Select TWO)**

**A. Outcomes Prioritized**

**B. Risk-adverse**

**C. Pay as you go**

**D. Lengthy**

**E. Predictable payments**

---

# Correct Answers

## ✅ A. Outcomes Prioritized

## ✅ C. Pay as you go

---

# Business Problem

The company is transitioning from traditional IT procurement to cloud-based procurement and needs to understand how cloud purchasing differs from purchasing on-premises infrastructure.

---

# Service Category

Cloud Economics & Cloud Adoption

---

# Service

AWS Cloud Financial Model

---

# Trigger Words

| Trigger Words           | Think                     |
| ----------------------- | ------------------------- |
| Cloud adoption          | Cloud economics           |
| Procurement strategy    | Cloud financial model     |
| Traditional procurement | On-premises purchasing    |
| Outcomes                | Business value            |
| Pay as you go           | Consumption-based pricing |

---

# Why These Answers Are Correct

## ✅ A. Outcomes Prioritized

Cloud procurement focuses on:

* Business outcomes
* Speed to value
* Agility
* Innovation

Organizations shift away from purchasing infrastructure first and instead focus on:

> What business result needs to be achieved?

### Business Outcome

```text
Business Goal
      ↓
Desired Outcome
      ↓
Cloud Services
      ↓
Business Value
```

This outcome-based approach is a major cloud adoption principle.

---

## ✅ C. Pay as You Go

One of the most important AWS Cloud benefits is:

> Pay only for what you use.

Organizations no longer need to:

* Purchase servers upfront
* Overprovision infrastructure
* Make large capital investments

Instead:

```text
Use Resources
      ↓
Consume Services
      ↓
Pay For Actual Usage
```

This consumption-based model is fundamental to cloud computing.

---

# Business Problem → Service Category → Service

```text
Need Modern Procurement Model
            ↓
Cloud Economics
            ↓
Outcome-Based Purchasing
            ↓
Pay-As-You-Go Consumption
```

---

# Why B. Risk-Adverse Is Incorrect

### Why Eliminate

Cloud procurement is generally designed to:

* Increase agility
* Enable experimentation
* Reduce barriers to innovation

Traditional procurement is typically more risk-averse.

Cloud adoption encourages controlled experimentation.

---

# Why D. Lengthy Is Incorrect

### Why Eliminate

Cloud procurement is intended to be:

* Faster
* More agile
* More responsive

Traditional procurement processes are often lengthy.

Cloud procurement reduces procurement delays.

---

# Why E. Predictable Payments Is Incorrect

### Why Eliminate

AWS pricing is consumption-based.

While costs can be forecasted and managed:

* Usage may vary
* Monthly costs may fluctuate

The defining characteristic is:

> Pay as you go

Not:

> Fixed predictable payments

---

# Similar Concepts to Eliminate

| Concept                    | Why Not Correct                                   |
| -------------------------- | ------------------------------------------------- |
| Risk-Adverse               | More closely aligned with traditional procurement |
| Lengthy Procurement Cycles | Opposite of cloud agility                         |
| Predictable Fixed Payments | Not a core cloud procurement principle            |
| Outcomes Prioritized       | ✅ Correct                                         |
| Pay as You Go              | ✅ Correct                                         |

---

# Cloud Procurement vs Traditional Procurement

| Traditional Procurement      | Cloud Procurement               |
| ---------------------------- | ------------------------------- |
| Capital Expenditures (CapEx) | Operational Expenditures (OpEx) |
| Large Upfront Purchases      | Pay as You Go                   |
| Long Procurement Cycles      | Rapid Provisioning              |
| Infrastructure Focused       | Outcome Focused                 |
| Fixed Capacity               | Elastic Capacity                |

---

# Exam Memory Aid

```text
Traditional IT
      ↓
Buy Infrastructure
      ↓
Hope It Meets Needs

Cloud
      ↓
Focus On Outcomes
      ↓
Pay As You Go
      ↓
Scale As Needed
```

---

# CLF-C02 Takeaway

When you see:

* Cloud adoption
* Procurement strategy
* Cloud economics
* Financial model
* Traditional vs cloud purchasing

Think:

## ✅ Outcomes Prioritized

## ✅ Pay as You Go

These are two of the foundational principles that differentiate cloud procurement from traditional infrastructure procurement.


