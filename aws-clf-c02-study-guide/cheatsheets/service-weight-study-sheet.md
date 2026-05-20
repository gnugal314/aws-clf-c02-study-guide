# AWS CLF-C02 Service Weight Study Sheet

Use this sheet to map high-value AWS services to business problems.

---

## VERY HIGH WEIGHT

### Amazon EC2

| Prompt | Your Answer |
|---|---|
| Business problem solved | Run scalable virtual servers and applications |
| Operational benefit | Full control over compute, OS, and installed software |
| Managed or unmanaged | Customer-managed compute on AWS-managed infrastructure |
| Serverless? | No |
| What category? | Compute |
| Common trigger words | virtual server, VM, operating system, lift-and-shift, full control |

### Amazon S3

| Prompt | Your Answer |
|---|---|
| Business problem solved | Durable scalable object storage for files, backups, logs, media |
| Operational benefit | No storage infrastructure to manage |
| Managed or unmanaged | Fully managed |
| Serverless? | Yes |
| What category? | Storage |
| Common trigger words | object storage, bucket, backup, archive, files, logs, static website |

### AWS Lambda

| Prompt | Your Answer |
|---|---|
| Business problem solved | Run code without managing servers |
| Operational benefit | Automatic scaling and low operational overhead |
| Managed or unmanaged | Fully managed |
| Serverless? | Yes |
| What category? | Compute |
| Common trigger words | serverless, event-driven, functions, no servers |

### AWS IAM

| Prompt | Your Answer |
|---|---|
| Business problem solved | Manage identity and access permissions |
| Operational benefit | Secure, fine-grained access control |
| Managed or unmanaged | Fully managed |
| Serverless? | Yes |
| What category? | Security |
| Common trigger words | users, groups, roles, policies, permissions, least privilege |

### Amazon VPC

| Prompt | Your Answer |
|---|---|
| Business problem solved | Build an isolated private network in AWS |
| Operational benefit | Custom network control, segmentation, routing, security boundaries |
| Managed or unmanaged | AWS-managed service, customer-configured network |
| Serverless? | No |
| What category? | Networking |
| Common trigger words | private network, CIDR, subnet, route table, security group |

### Amazon RDS

| Prompt | Your Answer |
|---|---|
| Business problem solved | Managed relational database hosting |
| Operational benefit | Automated patching, backups, maintenance |
| Managed or unmanaged | Fully managed |
| Serverless? | Some options are serverless |
| What category? | Database |
| Common trigger words | SQL, relational, MySQL, PostgreSQL, Oracle, managed database |

### Amazon DynamoDB

| Prompt | Your Answer |
|---|---|
| Business problem solved | Serverless NoSQL key-value data storage |
| Operational benefit | Low-latency, scalable database with minimal operations |
| Managed or unmanaged | Fully managed |
| Serverless? | Yes |
| What category? | Database |
| Common trigger words | NoSQL, key-value, serverless database, low latency |

### Amazon CloudWatch

| Prompt | Your Answer |
|---|---|
| Business problem solved | Monitor resources and applications |
| Operational benefit | Metrics, logs, alarms, observability |
| Managed or unmanaged | Fully managed |
| Serverless? | Yes |
| What category? | Monitoring |
| Common trigger words | metrics, monitoring, logs, alarms, observability |

### AWS CloudTrail

| Prompt | Your Answer |
|---|---|
| Business problem solved | Audit AWS API activity |
| Operational benefit | Governance, compliance, forensic investigation |
| Managed or unmanaged | Fully managed |
| Serverless? | Yes |
| What category? | Governance / Security |
| Common trigger words | API calls, audit trail, who did what, compliance |

---

## HIGH WEIGHT

### Amazon Route 53

| Prompt | Your Answer |
|---|---|
| Business problem solved | DNS routing and domain management |
| Operational benefit | Highly available DNS and routing policies |
| Managed or unmanaged | Fully managed |
| Serverless? | Yes |
| What category? | Networking |
| Common trigger words | DNS, domain, routing, hosted zone |

### Amazon CloudFront

| Prompt | Your Answer |
|---|---|
| Business problem solved | Deliver content globally with low latency |
| Operational benefit | Edge caching and performance improvement |
| Managed or unmanaged | Fully managed |
| Serverless? | Yes |
| What category? | Networking / Content Delivery |
| Common trigger words | CDN, edge location, cache, low latency, global content |

### Elastic Load Balancing

| Prompt | Your Answer |
|---|---|
| Business problem solved | Distribute traffic across targets |
| Operational benefit | Scalability and high availability |
| Managed or unmanaged | Fully managed |
| Serverless? | Yes |
| What category? | Networking |
| Common trigger words | load balancer, distribute traffic, high availability |

### AWS KMS

| Prompt | Your Answer |
|---|---|
| Business problem solved | Manage encryption keys |
| Operational benefit | Centralized encryption control |
| Managed or unmanaged | Fully managed |
| Serverless? | Yes |
| What category? | Security |
| Common trigger words | encryption keys, KMS, data protection |

### AWS WAF

| Prompt | Your Answer |
|---|---|
| Business problem solved | Protect web applications from malicious requests |
| Operational benefit | Layer 7 traffic filtering |
| Managed or unmanaged | Fully managed |
| Serverless? | Yes |
| What category? | Security |
| Common trigger words | web firewall, SQL injection, XSS, HTTP filtering |

### AWS Shield

| Prompt | Your Answer |
|---|---|
| Business problem solved | Protect from DDoS attacks |
| Operational benefit | Improves availability and attack resilience |
| Managed or unmanaged | Fully managed |
| Serverless? | Yes |
| What category? | Security |
| Common trigger words | DDoS, denial of service, attack protection |

### Amazon SQS

| Prompt | Your Answer |
|---|---|
| Business problem solved | Decouple services using queues |
| Operational benefit | Reliable asynchronous message buffering |
| Managed or unmanaged | Fully managed |
| Serverless? | Yes |
| What category? | Application Integration |
| Common trigger words | queue, decoupling, asynchronous, message buffering |

### Amazon SNS

| Prompt | Your Answer |
|---|---|
| Business problem solved | Publish notifications to many subscribers |
| Operational benefit | Fanout messaging and alert distribution |
| Managed or unmanaged | Fully managed |
| Serverless? | Yes |
| What category? | Application Integration |
| Common trigger words | pub/sub, notifications, fanout, email, SMS |
