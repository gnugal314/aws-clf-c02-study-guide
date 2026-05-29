# AWS CLF-C02 Pricing Differentiation Table

## Purpose

This reference guide helps differentiate AWS pricing models, billing tools, storage cost options, and cost optimization strategies commonly tested on the AWS Certified Cloud Practitioner (CLF-C02) exam.

---

| Pricing Options                                     | Key Differences                                                                                                                        |
| --------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| On-Demand vs Reserved Instances                     | On-Demand = no commitment/flexible; Reserved Instances = discounted pricing for long-term predictable workloads                        |
| Reserved Instances vs Savings Plans                 | Reserved Instances are more instance-specific; Savings Plans provide broader compute flexibility                                       |
| Spot Instances vs On-Demand                         | Spot = lowest-cost interruptible compute; On-Demand = stable non-interruptible compute                                                 |
| Spot Instances vs Reserved Instances                | Spot is cheapest but can be interrupted; Reserved provides predictable discounted capacity                                             |
| Savings Plans vs On-Demand                          | Savings Plans require usage commitment; On-Demand has no commitment                                                                    |
| AWS Budgets vs Cost Explorer                        | Budgets sends spending alerts; Cost Explorer analyzes historical cost trends                                                           |
| Cost Explorer vs Cost & Usage Report                | Cost Explorer provides visual dashboards; CUR provides detailed raw billing data                                                       |
| Free Tier vs Paid Usage                             | Free Tier offers limited free services; Paid usage begins after limits are exceeded                                                    |
| Compute Savings Plans vs EC2 Instance Savings Plans | Compute Savings Plans are more flexible across services; EC2 Instance Savings Plans are tied to specific instance families and Regions |
| Pay-As-You-Go vs Upfront Purchasing                 | Pay-as-you-go charges only for usage; Upfront purchasing requires capital investment                                                   |
| Dedicated Hosts vs Shared Tenancy                   | Dedicated Hosts provide isolated physical servers; Shared tenancy shares AWS infrastructure                                            |
| Data Transfer In vs Data Transfer Out               | Inbound AWS data transfer is usually free; outbound internet transfer is typically charged                                             |
| S3 Standard vs Glacier Pricing                      | S3 Standard costs more for active access; Glacier is cheaper for archival storage                                                      |
| Multi-AZ vs Single-AZ Costing                       | Multi-AZ improves availability but increases cost; Single-AZ is cheaper with lower resiliency                                          |
| Reserved Capacity vs Elastic Scaling                | Reserved capacity reduces cost for predictable workloads; Elastic Scaling adjusts dynamically for variable workloads                   |

---

# High-Value Exam Memory Aids

| Trigger Words                     | Likely Answer       |
| --------------------------------- | ------------------- |
| Lowest-cost compute               | Spot Instances      |
| Predictable workload              | Reserved Instances  |
| Flexible long-term savings        | Savings Plans       |
| No commitment                     | On-Demand           |
| Spending alerts                   | AWS Budgets         |
| Analyze AWS costs                 | Cost Explorer       |
| Detailed billing export           | Cost & Usage Report |
| Archive storage                   | Glacier             |
| Cost optimization recommendations | Trusted Advisor     |
| Variable demand                   | Auto Scaling        |

---

# AWS Pricing Model Cheat Sheet

| Pricing Model      | Best Used For                              |
| ------------------ | ------------------------------------------ |
| On-Demand          | New, unpredictable, short-term workloads   |
| Reserved Instances | Stable workloads running continuously      |
| Savings Plans      | Long-term compute usage with flexibility   |
| Spot Instances     | Fault-tolerant and interruptible workloads |
| Free Tier          | Learning, testing, and small workloads     |

---

# Most Tested Cost Optimization Concepts

1. AWS Budgets = Alerts
2. Cost Explorer = Cost Analysis
3. Spot Instances = Lowest Cost Compute
4. Savings Plans = Flexible Discounts
5. Reserved Instances = Predictable Workload Discounts
6. Auto Scaling = Reduce Overprovisioning
7. S3 Lifecycle Policies = Reduce Storage Costs
8. Glacier = Long-Term Archival Storage
9. Trusted Advisor = Cost Optimization Recommendations
10. Pay-As-You-Go = Cloud Financial Model
