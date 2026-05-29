# AWS CLF-C02 Master Service Differentiation Table

| Category                    | Service                     | Best Used For                         | Key Difference                                             | Trigger Words                                          |
| --------------------------- | --------------------------- | ------------------------------------- | ---------------------------------------------------------- | ------------------------------------------------------ |
| Compute Services            | EC2                         | Virtual servers and full OS control   | Customer manages operating system and server configuration | virtual server, lift-and-shift, compute capacity, VM   |
| Compute Services            | Lambda                      | Event-driven serverless applications  | No server management; pay per execution                    | serverless, event-driven, functions, automatic scaling |
| Compute Services            | ECS                         | AWS-native container orchestration    | Simpler AWS container management                           | containers, Docker, orchestration                      |
| Compute Services            | EKS                         | Kubernetes workloads                  | Managed Kubernetes control plane                           | Kubernetes, K8s, container platform                    |
| Compute Services            | Fargate                     | Serverless containers                 | Eliminates EC2 host management                             | serverless containers, no servers                      |
| Compute Services            | Elastic Beanstalk           | Rapid application deployment          | Platform-as-a-Service experience                           | deploy application, managed platform                   |
| Compute Services            | Auto Scaling                | Dynamic compute scaling               | Automatically adjusts capacity                             | elasticity, demand spikes, scale automatically         |
| Storage Services            | S3                          | Object storage                        | Stores files as objects in buckets                         | object storage, backups, files, media, buckets         |
| Storage Services            | EBS                         | Block storage for EC2                 | Attached storage for individual EC2 instances              | block storage, EC2 disk, volume                        |
| Storage Services            | EFS                         | Shared file storage                   | Multiple EC2 instances can access simultaneously           | shared filesystem, NFS, file share                     |
| Storage Services            | Glacier                     | Long-term archival storage            | Lowest-cost archive tier                                   | archive, retention, cold storage                       |
| Storage Services            | Storage Gateway             | Hybrid storage integration            | Connects on-premises storage to AWS                        | hybrid storage, on-prem integration                    |
| Database Services           | RDS                         | Relational databases                  | Managed SQL databases                                      | MySQL, PostgreSQL, relational database                 |
| Database Services           | Aurora                      | High-performance relational databases | AWS-optimized relational database                          | enterprise database, high performance                  |
| Database Services           | DynamoDB                    | NoSQL applications                    | Serverless key-value database                              | NoSQL, key-value, low latency                          |
| Database Services           | Redshift                    | Analytics and data warehousing        | Purpose-built for BI and analytics                         | data warehouse, analytics, reporting                   |
| Database Services           | ElastiCache                 | Application caching                   | In-memory acceleration layer                               | Redis, caching, performance                            |
| Database Services           | Neptune                     | Relationship analysis                 | Graph database service                                     | graph, relationships, connected data                   |
| Networking Services         | VPC                         | Private cloud networking              | Isolated AWS network                                       | private network, CIDR, subnets                         |
| Networking Services         | Route 53                    | DNS management                        | Highly available DNS service                               | DNS, domain routing                                    |
| Networking Services         | CloudFront                  | Global content delivery               | CDN using edge locations                                   | CDN, low latency, caching                              |
| Networking Services         | Elastic Load Balancer (ELB) | Traffic distribution                  | Balances traffic across resources                          | load balancing, distribute traffic                     |
| Networking Services         | Direct Connect              | Dedicated AWS connectivity            | Private physical connection to AWS                         | dedicated connection, hybrid networking                |
| Networking Services         | API Gateway                 | API management                        | Managed API hosting and security                           | REST API, HTTP endpoint                                |
| Networking Services         | Transit Gateway             | Multi-network routing                 | Centralized network connectivity                           | hub-and-spoke, network routing                         |
| Security Services           | IAM                         | Identity and permissions              | Controls access to AWS resources                           | users, groups, roles, permissions                      |
| Security Services           | KMS                         | Encryption key management             | Centralized key control                                    | encryption, keys, KMS                                  |
| Security Services           | Shield                      | DDoS protection                       | Protects against denial-of-service attacks                 | DDoS, attack protection                                |
| Security Services           | WAF                         | Web application protection            | Filters malicious HTTP traffic                             | SQL injection, XSS, web filtering                      |
| Security Services           | GuardDuty                   | Threat detection                      | Intelligent security monitoring                            | suspicious activity, threat detection                  |
| Security Services           | Cognito                     | User authentication                   | Sign-up and sign-in for applications                       | authentication, login, user management                 |
| Security Services           | Secrets Manager             | Secret storage                        | Manages credentials and API keys                           | secrets, passwords, credentials                        |
| Monitoring & Governance     | CloudWatch                  | Monitoring and observability          | Metrics, logs, alarms                                      | CPU utilization, metrics, monitoring                   |
| Monitoring & Governance     | CloudTrail                  | Auditing and compliance               | Tracks API activity                                        | API calls, auditing, governance                        |
| Monitoring & Governance     | AWS Config                  | Configuration compliance              | Tracks resource changes                                    | configuration tracking, compliance                     |
| Monitoring & Governance     | Trusted Advisor             | Best-practice recommendations         | Cost, security, performance guidance                       | optimization, recommendations                          |
| Monitoring & Governance     | Organizations               | Multi-account management              | Centralized account governance                             | consolidated billing, multi-account                    |
| Monitoring & Governance     | Control Tower               | Landing zone setup                    | Automated governance framework                             | landing zone, account setup                            |
| Billing & Cost Optimization | AWS Budgets                 | Spending alerts                       | Proactive budget monitoring                                | budget alerts, spending threshold                      |
| Billing & Cost Optimization | Cost Explorer               | Cost analysis                         | Visual spending analysis                                   | cost trends, spending reports                          |
| Billing & Cost Optimization | Cost & Usage Report         | Detailed billing exports              | Granular billing and usage data                            | billing export, usage report                           |
| Billing & Cost Optimization | Savings Plans               | Flexible long-term discounts          | Applies across compute services                            | savings, commitment discount                           |
| Billing & Cost Optimization | Reserved Instances          | Predictable workload discounts        | EC2-specific commitment savings                            | reserved capacity, predictable usage                   |
| Billing & Cost Optimization | Spot Instances              | Lowest-cost compute                   | Uses spare AWS capacity                                    | cheapest compute, interruptible                        |
| Messaging & Integration     | SNS                         | Notifications and pub/sub             | Push-based messaging                                       | notifications, fanout, email alerts                    |
| Messaging & Integration     | SQS                         | Application queues                    | Message buffering and decoupling                           | queue, asynchronous processing                         |
| Messaging & Integration     | EventBridge                 | Event-driven integration              | Event routing platform                                     | event bus, event-driven architecture                   |
| Messaging & Integration     | Step Functions              | Workflow orchestration                | Coordinates multi-step processes                           | workflow, orchestration                                |
| Messaging & Integration     | Amazon MQ                   | Managed message brokers               | ActiveMQ/RabbitMQ support                                  | message broker, legacy integration                     |
| Analytics Services          | Athena                      | SQL queries on S3                     | Serverless query engine                                    | SQL on S3, ad hoc analysis                             |
| Analytics Services          | Glue                        | ETL and data integration              | Managed data preparation                                   | ETL, data catalog                                      |
| Analytics Services          | QuickSight                  | Business intelligence                 | Dashboarding and visualization                             | dashboards, BI, reporting                              |
| Analytics Services          | EMR                         | Big data processing                   | Managed Hadoop and Spark                                   | big data, Spark, Hadoop                                |
| Analytics Services          | Kinesis                     | Real-time streaming                   | Stream ingestion and processing                            | streaming, real-time analytics                         |
| Analytics Services          | OpenSearch                  | Search and log analytics              | Search engine and log analysis                             | search, logs, indexing                                 |
| AI/ML Services              | SageMaker                   | Machine learning lifecycle            | Build, train, and deploy ML models                         | machine learning, model training                       |
| AI/ML Services              | Bedrock                     | Generative AI applications            | Foundation model access                                    | generative AI, LLM, foundation models                  |
| AI/ML Services              | Rekognition                 | Image and video analysis              | Computer vision service                                    | image recognition, video analysis                      |
| AI/ML Services              | Textract                    | Document processing                   | Extracts text and forms from documents                     | OCR, forms, document extraction                        |
| AI/ML Services              | Comprehend                  | Natural language processing           | Text analysis and sentiment detection                      | NLP, sentiment, entity recognition                     |
| AI/ML Services              | Transcribe                  | Speech-to-text                        | Converts audio to text                                     | transcription, speech recognition                      |
| AI/ML Services              | Polly                       | Text-to-speech                        | Converts text into lifelike speech                         | voice synthesis, speech generation                     |

# High-Value CLF-C02 Service Recognition Tips

| Trigger Words       | Likely Service |
| ------------------- | -------------- |
| Serverless          | Lambda         |
| Object Storage      | S3             |
| Relational Database | RDS            |
| NoSQL               | DynamoDB       |
| DNS                 | Route 53       |
| CDN                 | CloudFront     |
| User Permissions    | IAM            |
| Encryption Keys     | KMS            |
| Monitor CPU         | CloudWatch     |
| Audit API Calls     | CloudTrail     |
| Queue Messages      | SQS            |
| Send Notifications  | SNS            |
| SQL on S3           | Athena         |
| Machine Learning    | SageMaker      |
| Generative AI       | Bedrock        |
| Lowest-Cost Compute | Spot Instances |
| Spending Alerts     | AWS Budgets    |
| Cost Analysis       | Cost Explorer  |
