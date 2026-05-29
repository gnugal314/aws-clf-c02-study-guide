# AWS CLF-C02 Cost Optimization Differentiation Table

## Purpose

This reference guide focuses specifically on AWS billing, pricing models, cost optimization tools, and architectural decisions that impact AWS spend. These concepts are frequently tested on the AWS Certified Cloud Practitioner (CLF-C02) exam.

---

| Billing & Cost Optimization Services                | Key Differences                                                                                                               |
| --------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| AWS Budgets vs Cost Explorer                        | Budgets sends alerts when spending thresholds are exceeded; Cost Explorer analyzes and visualizes historical spending trends  |
| Cost Explorer vs Cost & Usage Report (CUR)          | Cost Explorer provides dashboards/charts; CUR provides detailed raw billing and usage data exports                            |
| Reserved Instances vs Savings Plans                 | Reserved Instances are tied more closely to instance configurations; Savings Plans provide more flexible compute discounts    |
| Spot Instances vs On-Demand                         | Spot provides the lowest-cost interruptible compute; On-Demand provides flexible stable compute with no interruption risk     |
| Savings Plans vs On-Demand                          | Savings Plans require long-term usage commitments for discounts; On-Demand has no commitment                                  |
| On-Demand vs Reserved Instances                     | On-Demand is flexible with no upfront commitment; Reserved Instances reduce cost for predictable workloads                    |
| AWS Budgets vs Trusted Advisor                      | Budgets focuses on spending alerts; Trusted Advisor provides optimization recommendations including cost savings              |
| Cost Allocation Tags vs AWS Budgets                 | Tags organize and categorize costs; Budgets monitors and alerts on spending                                                   |
| Compute Savings Plans vs EC2 Instance Savings Plans | Compute Savings Plans are more flexible across compute services; EC2 Instance Savings Plans are more instance-family specific |
| S3 Standard vs S3 Glacier                           | S3 Standard is optimized for frequent access; Glacier is optimized for low-cost archival storage                              |
| Single-AZ vs Multi-AZ Deployments                   | Single-AZ is lower cost with less resiliency; Multi-AZ increases availability but costs more                                  |
| Auto Scaling vs Fixed Capacity                      | Auto Scaling reduces waste by scaling dynamically; Fixed capacity risks overprovisioning or underutilization                  |
| Data Transfer In vs Data Transfer Out               | Inbound data transfer is generally free; outbound internet traffic is typically charged                                       |
| Free Tier vs Paid AWS Usage                         | Free Tier provides limited no-cost service usage; Paid usage begins after limits are exceeded                                 |
| Dedicated Hosts vs Shared Tenancy                   | Dedicated Hosts provide isolated hardware at higher cost; Shared tenancy is lower cost and multi-tenant                       |
| AWS Organizations vs Separate Accounts              | Organizations enables centralized billing and consolidated cost management across accounts                                    |
| AWS Marketplace vs Native AWS Services              | Marketplace may include third-party licensing costs; Native AWS services use AWS pricing models                               |
| Provisioned Capacity vs Serverless Pricing          | Provisioned capacity charges for allocated resources; Serverless pricing charges based on actual usage                        |
| EC2 vs Lambda Cost Model                            | EC2 charges while instances run; Lambda charges per execution and runtime duration                                            |
| Reserved Capacity vs Elasticity                     | Reserved capacity lowers predictable long-term costs; Elasticity reduces waste during fluctuating demand                      |

---

# High-Value Cost Optimization Trigger Words

| Trigger Words               | Likely Answer       |
| --------------------------- | ------------------- |
| Lowest-cost compute         | Spot Instances      |
| Predictable workload        | Reserved Instances  |
| Flexible long-term discount | Savings Plans       |
| No commitment               | On-Demand           |
| Spending alert              | AWS Budgets         |
| Analyze spending            | Cost Explorer       |
| Detailed billing data       | Cost & Usage Report |
| Archive storage             | S3 Glacier          |
| Cost recommendations        | Trusted Advisor     |
| Scale with demand           | Auto Scaling        |
| Reduce idle resources       | Auto Scaling        |
| Pay only for usage          | Serverless Pricing  |
| Consolidated billing        | AWS Organizations   |

---

# Cost Optimization Decision Guide

| Business Requirement                       | Recommended AWS Service/Approach |
| ------------------------------------------ | -------------------------------- |
| Receive notifications before overspending  | AWS Budgets                      |
| Understand where AWS spend is occurring    | Cost Explorer                    |
| Export detailed billing records            | Cost & Usage Report              |
| Reduce EC2 costs for predictable workloads | Reserved Instances               |
| Reduce compute costs with flexibility      | Savings Plans                    |
| Achieve the lowest compute cost            | Spot Instances                   |
| Reduce storage costs for archival data     | S3 Glacier                       |
| Automatically adjust capacity to demand    | Auto Scaling                     |
| Eliminate idle server costs                | Lambda or Serverless Services    |
| Centralize cost management across accounts | AWS Organizations                |

---

# Most Tested CLF-C02 Cost Concepts

1. AWS Budgets = Cost Alerts
2. Cost Explorer = Cost Analysis
3. Cost & Usage Report = Detailed Billing Data
4. Spot Instances = Lowest Cost Compute
5. Savings Plans = Flexible Commitment Discounts
6. Reserved Instances = Predictable Workload Discounts
7. Auto Scaling = Cost Efficiency Through Elasticity
8. S3 Glacier = Low-Cost Archival Storage
9. Trusted Advisor = Cost Optimization Recommendations
10. AWS Organizations = Consolidated Billing

---

# Exam Memory Aids

| If You See...                       | Think...            |
| ----------------------------------- | ------------------- |
| "Alert me when spending exceeds..." | AWS Budgets         |
| "Analyze historical AWS costs..."   | Cost Explorer       |
| "Lowest-cost EC2 option..."         | Spot Instances      |
| "Predictable workload..."           | Reserved Instances  |
| "Flexible compute discount..."      | Savings Plans       |
| "Archive data for years..."         | S3 Glacier          |
| "Automatically adjust capacity..."  | Auto Scaling        |
| "Pay only when code runs..."        | AWS Lambda          |
| "Centralized billing..."            | AWS Organizations   |
| "Detailed billing export..."        | Cost & Usage Report |
