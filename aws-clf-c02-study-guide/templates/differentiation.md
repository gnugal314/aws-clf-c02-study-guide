# AWS CLF-C02 Master Service Differentiation Table

| Similar Services                     | Key Differences                                                                                                                |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ |
| EC2 vs Lambda                        | EC2 provides full server/OS control; Lambda is serverless and event-driven with no server management                           |
| ECS vs EKS                           | ECS is AWS-native container orchestration; EKS is managed Kubernetes                                                           |
| ECS/EKS vs Fargate                   | ECS/EKS manage containers; Fargate removes server management for containers                                                    |
| S3 vs EBS vs EFS                     | S3 = object storage; EBS = block storage for EC2; EFS = shared file storage                                                    |
| Glacier vs S3 Standard               | Glacier is low-cost archival storage; S3 Standard is active-access object storage                                              |
| RDS vs DynamoDB                      | RDS is relational SQL; DynamoDB is NoSQL key-value                                                                             |
| RDS vs Aurora                        | Aurora is AWS-optimized high-performance relational database; RDS supports multiple standard engines                           |
| Redshift vs RDS                      | Redshift is analytics/data warehousing; RDS is transactional relational database                                               |
| CloudWatch vs CloudTrail             | CloudWatch monitors metrics/logs; CloudTrail tracks API activity and auditing                                                  |
| CloudTrail vs Config                 | CloudTrail tracks user/API actions; Config tracks resource configuration changes                                               |
| Security Groups vs Network ACLs      | Security Groups are stateful instance-level firewalls; NACLs are stateless subnet-level firewalls                              |
| IAM Users vs IAM Roles               | Users are permanent identities; Roles provide temporary assumed permissions                                                    |
| IAM Groups vs IAM Roles              | Groups organize users with shared permissions; Roles delegate temporary access                                                 |
| Shield vs WAF                        | Shield protects from DDoS attacks; WAF filters malicious web traffic                                                           |
| SNS vs SQS                           | SNS pushes notifications/pub-sub; SQS stores queued messages for asynchronous processing                                       |
| EventBridge vs SNS                   | EventBridge routes application/system events; SNS distributes notifications/messages                                           |
| Route 53 vs CloudFront               | Route 53 provides DNS routing; CloudFront provides CDN caching and global delivery                                             |
| VPC vs Subnet                        | VPC is the overall private network; Subnet is a segmented network range inside a VPC                                           |
| Internet Gateway vs NAT Gateway      | Internet Gateway allows inbound/outbound internet access; NAT Gateway allows outbound-only internet access for private subnets |
| Reserved Instances vs Spot Instances | Reserved = long-term discounted predictable usage; Spot = cheapest interruptible compute                                       |
| Savings Plans vs Reserved Instances  | Savings Plans provide flexible compute discounts; Reserved Instances are more instance-specific                                |
| Cost Explorer vs AWS Budgets         | Cost Explorer analyzes spending trends; AWS Budgets sends spending alerts                                                      |
| Athena vs Redshift                   | Athena queries S3 directly serverlessly; Redshift is a dedicated analytics warehouse                                           |
| Glue vs Athena                       | Glue performs ETL/data integration; Athena performs SQL querying                                                               |
| SageMaker vs Bedrock                 | SageMaker builds/trains ML models; Bedrock provides foundation models for generative AI                                        |
| Direct Connect vs VPN                | Direct Connect is a dedicated private network connection; VPN uses encrypted internet connectivity                             |
| ELB vs Auto Scaling                  | ELB distributes traffic; Auto Scaling adjusts resource capacity                                                                |
| API Gateway vs Load Balancer         | API Gateway manages APIs; ELB distributes general application/network traffic                                                  |
| Cognito vs IAM                       | Cognito manages application user authentication; IAM manages AWS account/service permissions                                   |
| EBS vs Instance Store                | EBS is persistent block storage; Instance Store is temporary ephemeral storage                                                 |
| Trusted Advisor vs Compute Optimizer | Trusted Advisor provides broad AWS recommendations; Compute Optimizer focuses on rightsizing resources                         |
| Organizations vs Control Tower       | Organizations manages multiple AWS accounts; Control Tower automates governed multi-account setup                              |
| CloudFormation vs Elastic Beanstalk  | CloudFormation provisions infrastructure as code; Elastic Beanstalk deploys applications with managed infrastructure           |
| Step Functions vs SQS                | Step Functions orchestrates workflows; SQS queues messages asynchronously                                                      |
| Inspector vs GuardDuty               | Inspector scans for vulnerabilities; GuardDuty detects threats and suspicious activity                                         |
| Macie vs GuardDuty                   | Macie identifies sensitive data; GuardDuty identifies threats and anomalies                                                    |
| EC2 Auto Scaling vs Lambda Scaling   | Auto Scaling adjusts EC2 instance count; Lambda scales automatically per request                                               |
| Public Subnet vs Private Subnet      | Public subnets allow direct internet access; Private subnets restrict inbound internet access                                  |
| Stateful vs Stateless Firewalls      | Security Groups are stateful; Network ACLs are stateless                                                                       |
| Multi-AZ vs Multi-Region             | Multi-AZ improves availability within a Region; Multi-Region improves geographic disaster recovery                             |
| On-Demand vs Reserved Pricing        | On-Demand has no commitment; Reserved provides discounts for long-term commitments                                             |
| Hybrid Cloud vs Multi-Cloud          | Hybrid combines cloud + on-premises; Multi-cloud uses multiple cloud providers                                                 |
