# AWS CLF-C02 Business Problem → Service Category → Service Mapping

## Purpose

The AWS Certified Cloud Practitioner (CLF-C02) exam is primarily a service recognition exam. Most questions describe a business problem and require you to identify the correct AWS service.

Use this table to train yourself to think:

**Business Problem → Service Category → Common AWS Services**

---

| Business Problem                                                   | Service Category            | Common Services                 |
| ------------------------------------------------------------------ | --------------------------- | ------------------------------- |
| Run virtual servers in the cloud                                   | Compute                     | EC2, Auto Scaling               |
| Run code without managing servers                                  | Compute                     | Lambda                          |
| Run containerized applications                                     | Compute / Containers        | ECS, EKS, Fargate               |
| Deploy applications quickly with minimal infrastructure management | Compute                     | Elastic Beanstalk               |
| Host a simple website or small application                         | Compute                     | Lightsail                       |
| Process large batch workloads                                      | Compute                     | AWS Batch                       |
| Store files, backups, images, and documents                        | Storage                     | S3                              |
| Attach persistent storage to an EC2 instance                       | Storage                     | EBS                             |
| Share storage across multiple Linux servers                        | Storage                     | EFS                             |
| Archive data for years at low cost                                 | Storage                     | Glacier                         |
| Connect on-premises storage to AWS                                 | Storage                     | Storage Gateway                 |
| Run a managed SQL database                                         | Database                    | RDS                             |
| Run a high-performance relational database                         | Database                    | Aurora                          |
| Run a serverless NoSQL database                                    | Database                    | DynamoDB                        |
| Build a cloud data warehouse                                       | Database / Analytics        | Redshift                        |
| Cache frequently accessed data                                     | Database                    | ElastiCache                     |
| Analyze graph relationships                                        | Database                    | Neptune                         |
| Create an isolated private cloud network                           | Networking                  | VPC                             |
| Route internet traffic to applications                             | Networking                  | Route 53                        |
| Deliver content globally with low latency                          | Networking                  | CloudFront                      |
| Distribute traffic across multiple servers                         | Networking                  | Elastic Load Balancer           |
| Connect an on-premises network to AWS privately                    | Networking                  | Direct Connect                  |
| Securely expose APIs                                               | Networking / Integration    | API Gateway                     |
| Connect multiple VPCs centrally                                    | Networking                  | Transit Gateway                 |
| Manage AWS users and permissions                                   | Security                    | IAM                             |
| Manage encryption keys                                             | Security                    | KMS                             |
| Protect against DDoS attacks                                       | Security                    | Shield                          |
| Protect web applications from attacks                              | Security                    | WAF                             |
| Detect suspicious activity                                         | Security                    | GuardDuty                       |
| Manage application user sign-in/sign-up                            | Security                    | Cognito                         |
| Store passwords and secrets securely                               | Security                    | Secrets Manager                 |
| Monitor infrastructure metrics and logs                            | Monitoring                  | CloudWatch                      |
| Track AWS API activity                                             | Monitoring / Governance     | CloudTrail                      |
| Monitor configuration changes                                      | Governance                  | AWS Config                      |
| Receive architecture and cost recommendations                      | Governance                  | Trusted Advisor                 |
| Manage multiple AWS accounts                                       | Governance                  | AWS Organizations               |
| Establish a governed landing zone                                  | Governance                  | Control Tower                   |
| Receive alerts when costs exceed thresholds                        | Billing & Cost Optimization | AWS Budgets                     |
| Analyze historical AWS spending                                    | Billing & Cost Optimization | Cost Explorer                   |
| Export detailed billing data                                       | Billing & Cost Optimization | Cost & Usage Report             |
| Reduce costs for predictable workloads                             | Billing & Cost Optimization | Reserved Instances              |
| Reduce costs with flexible commitments                             | Billing & Cost Optimization | Savings Plans                   |
| Achieve the lowest compute cost                                    | Billing & Cost Optimization | Spot Instances                  |
| Send notifications to many subscribers                             | Messaging & Integration     | SNS                             |
| Queue messages between applications                                | Messaging & Integration     | SQS                             |
| Build event-driven architectures                                   | Messaging & Integration     | EventBridge                     |
| Coordinate multi-step workflows                                    | Messaging & Integration     | Step Functions                  |
| Support traditional message brokers                                | Messaging & Integration     | Amazon MQ                       |
| Query data stored in S3 using SQL                                  | Analytics                   | Athena                          |
| Perform ETL and data preparation                                   | Analytics                   | Glue                            |
| Create business dashboards and reports                             | Analytics                   | QuickSight                      |
| Process large-scale Hadoop/Spark workloads                         | Analytics                   | EMR                             |
| Process real-time streaming data                                   | Analytics                   | Kinesis                         |
| Search and analyze logs                                            | Analytics                   | OpenSearch                      |
| Build, train, and deploy ML models                                 | AI / ML                     | SageMaker                       |
| Build generative AI applications                                   | AI / ML                     | Bedrock                         |
| Analyze images and videos                                          | AI / ML                     | Rekognition                     |
| Extract text from forms and documents                              | AI / ML                     | Textract                        |
| Analyze text sentiment and entities                                | AI / ML                     | Comprehend                      |
| Convert speech to text                                             | AI / ML                     | Transcribe                      |
| Convert text into speech                                           | AI / ML                     | Polly                           |
| Improve application availability                                   | Architecture                | Multi-AZ                        |
| Improve disaster recovery across regions                           | Architecture                | Multi-Region                    |
| Scale automatically based on demand                                | Architecture / Compute      | Auto Scaling                    |
| Reduce overprovisioning costs                                      | Cost Optimization           | Auto Scaling                    |
| Implement least-privilege access                                   | Security                    | IAM                             |
| Encrypt sensitive data                                             | Security                    | KMS                             |
| Meet compliance requirements                                       | Security / Governance       | Config, CloudTrail, Artifact    |
| Improve cost visibility across departments                         | Cost Optimization           | Cost Allocation Tags            |
| Consolidate billing across multiple accounts                       | Cost Optimization           | AWS Organizations               |
| Host a globally distributed static website                         | Storage / Networking        | S3 + CloudFront + Route 53      |
| Build serverless applications                                      | Compute                     | Lambda + API Gateway            |
| Build highly available web applications                            | Networking / Compute        | ELB + Auto Scaling + EC2        |
| Implement hybrid cloud connectivity                                | Networking                  | Direct Connect, VPN             |
| Store infrequently accessed data at lower cost                     | Storage                     | S3 Intelligent-Tiering, Glacier |

---

# High-Value Exam Recognition Patterns

| If You See...            | Think...       |
| ------------------------ | -------------- |
| "Virtual Server"         | EC2            |
| "Serverless"             | Lambda         |
| "Object Storage"         | S3             |
| "Relational Database"    | RDS            |
| "NoSQL Database"         | DynamoDB       |
| "DNS"                    | Route 53       |
| "Content Delivery"       | CloudFront     |
| "Permissions"            | IAM            |
| "Encryption Keys"        | KMS            |
| "Monitor Metrics"        | CloudWatch     |
| "Audit API Calls"        | CloudTrail     |
| "Send Notifications"     | SNS            |
| "Queue Messages"         | SQS            |
| "Workflow Orchestration" | Step Functions |
| "SQL on S3"              | Athena         |
| "Machine Learning"       | SageMaker      |
| "Generative AI"          | Bedrock        |
| "Spending Alerts"        | AWS Budgets    |
| "Analyze AWS Costs"      | Cost Explorer  |
| "Lowest Cost Compute"    | Spot Instances |

---

# Exam Mindset

Always ask:

1. What business problem is being described?
2. What service category solves that problem?
3. Which AWS service is the best fit?

**Business Problem → Service Category → Service**

This framework alone can solve the majority of CLF-C02 scenario-based questions.
