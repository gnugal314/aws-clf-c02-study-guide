# AWS CLF-C02 Fast Recall Service Mapping

## Business Problem → Service Category → AWS Service

This reference guide focuses on AWS services that are commonly confused on the AWS Certified Cloud Practitioner (CLF-C02) exam.

---

## Service Mapping Table

| Business Problem                                                  | Service Category                     | Service         |
| ----------------------------------------------------------------- | ------------------------------------ | --------------- |
| Connect on-premises storage systems to AWS storage services       | Hybrid Storage                       | Storage Gateway |
| Run SQL queries directly against files stored in Amazon S3        | Analytics                            | Athena          |
| Build, train, and deploy machine learning models                  | AI / ML                              | SageMaker       |
| Build generative AI applications using foundation models          | AI / ML                              | Bedrock         |
| Deliver content globally with low latency                         | Networking / Content Delivery        | CloudFront      |
| Create, publish, secure, and manage APIs                          | Networking / Application Integration | API Gateway     |
| Connect multiple VPCs and networks through a centralized hub      | Networking                           | Transit Gateway |
| Manage user sign-up, sign-in, and authentication                  | Security / Identity                  | Cognito         |
| Monitor AWS resources, logs, metrics, and alarms                  | Monitoring                           | CloudWatch      |
| Audit AWS account activity and API calls                          | Governance / Auditing                | CloudTrail      |
| Establish and govern a multi-account AWS environment              | Governance                           | Control Tower   |
| Build event-driven architectures and route events between systems | Messaging & Integration              | EventBridge     |
| Coordinate multi-step workflows and business processes            | Messaging & Integration              | Step Functions  |
| Extract, transform, and load (ETL) data                           | Analytics                            | Glue            |
| Extract text, forms, and tables from documents                    | AI / ML                              | Textract        |
| Analyze text for sentiment, entities, and language insights       | AI / ML                              | Comprehend      |
| Convert speech recordings into text                               | AI / ML                              | Transcribe      |
| Convert text into lifelike speech                                 | AI / ML                              | Polly           |
| Build dashboards and business intelligence reports                | Analytics                            | QuickSight      |
| Process large-scale Hadoop and Spark workloads                    | Analytics / Big Data                 | EMR             |
| Process streaming data in real time                               | Analytics / Streaming                | Kinesis         |
| Search, analyze, and visualize logs and operational data          | Analytics / Search                   | OpenSearch      |
| Analyze images and videos using computer vision                   | AI / ML                              | Rekognition     |

---

## Exam Trigger Word Cheat Sheet

| Trigger Words                   | Think Service   |
| ------------------------------- | --------------- |
| Hybrid storage                  | Storage Gateway |
| On-premises storage integration | Storage Gateway |
| SQL on S3                       | Athena          |
| Serverless analytics            | Athena          |
| Machine learning models         | SageMaker       |
| Model training                  | SageMaker       |
| Generative AI                   | Bedrock         |
| Foundation models               | Bedrock         |
| LLMs                            | Bedrock         |
| CDN                             | CloudFront      |
| Edge locations                  | CloudFront      |
| Low latency content delivery    | CloudFront      |
| REST API                        | API Gateway     |
| HTTP API                        | API Gateway     |
| Multiple VPCs                   | Transit Gateway |
| Centralized networking          | Transit Gateway |
| User authentication             | Cognito         |
| User sign-in                    | Cognito         |
| Metrics                         | CloudWatch      |
| CPU utilization                 | CloudWatch      |
| Monitoring                      | CloudWatch      |
| API activity                    | CloudTrail      |
| Audit logs                      | CloudTrail      |
| Governance                      | CloudTrail      |
| Landing zone                    | Control Tower   |
| Multi-account setup             | Control Tower   |
| Event bus                       | EventBridge     |
| Event-driven architecture       | EventBridge     |
| Workflow orchestration          | Step Functions  |
| State machine                   | Step Functions  |
| ETL                             | Glue            |
| Data catalog                    | Glue            |
| OCR                             | Textract        |
| Document extraction             | Textract        |
| Sentiment analysis              | Comprehend      |
| NLP                             | Comprehend      |
| Speech-to-text                  | Transcribe      |
| Audio transcription             | Transcribe      |
| Text-to-speech                  | Polly           |
| Voice synthesis                 | Polly           |
| Dashboards                      | QuickSight      |
| BI reporting                    | QuickSight      |
| Hadoop                          | EMR             |
| Spark                           | EMR             |
| Big data                        | EMR             |
| Streaming analytics             | Kinesis         |
| Real-time ingestion             | Kinesis         |
| Search engine                   | OpenSearch      |
| Log analytics                   | OpenSearch      |
| Image recognition               | Rekognition     |
| Video analysis                  | Rekognition     |

---

## One-Line Memory Anchors

| Service         | Memory Anchor           |
| --------------- | ----------------------- |
| Storage Gateway | On-Prem Storage ↔ AWS   |
| Athena          | SQL on S3               |
| SageMaker       | Build ML Models         |
| Bedrock         | Build GenAI Apps        |
| CloudFront      | Global CDN              |
| API Gateway     | Front Door for APIs     |
| Transit Gateway | Router for VPCs         |
| Cognito         | User Login Service      |
| CloudWatch      | Watch Metrics           |
| CloudTrail      | Trail of API Actions    |
| Control Tower   | Govern AWS Accounts     |
| EventBridge     | Event Router            |
| Step Functions  | Workflow Coordinator    |
| Glue            | ETL Service             |
| Textract        | Read Documents          |
| Comprehend      | Understand Text         |
| Transcribe      | Audio → Text            |
| Polly           | Text → Audio            |
| QuickSight      | BI Dashboards           |
| EMR             | Hadoop / Spark          |
| Kinesis         | Streaming Data          |
| OpenSearch      | Search Logs             |
| Rekognition     | Analyze Images & Videos |

---

## Category Grouping for Fast Recall

| Category                | Services                                                                 |
| ----------------------- | ------------------------------------------------------------------------ |
| Hybrid Storage          | Storage Gateway                                                          |
| Analytics               | Athena, Glue, QuickSight, EMR, Kinesis, OpenSearch                       |
| AI / ML                 | SageMaker, Bedrock, Textract, Comprehend, Transcribe, Polly, Rekognition |
| Networking              | CloudFront, API Gateway, Transit Gateway                                 |
| Security / Identity     | Cognito                                                                  |
| Monitoring / Governance | CloudWatch, CloudTrail, Control Tower                                    |
| Messaging & Integration | EventBridge, Step Functions                                              |

---

## CLF-C02 Exam Strategy

When you encounter a scenario question:

1. Identify the business problem.
2. Determine the service category.
3. Look for trigger words.
4. Match the trigger words to the AWS service.
5. Eliminate similar services that solve a different problem.

**Business Problem → Service Category → Service**
