# DAY 12 — Analytics, AI/ML & Containers Deep Dive

Source Reference: *Overview of Amazon Web Services AWS Whitepaper*

---

# Study Focus

This day focuses on AWS analytics, AI/ML, and container services used for modern data-driven cloud architectures.

Focus areas:
- Amazon Athena
- AWS Glue
- Amazon QuickSight
- Amazon Redshift
- Amazon SageMaker
- Amazon Bedrock
- ECS
- EKS
- Fargate
- Event-driven architectures
- Analytics workflows

---

# Why This Matters for the Exam

AWS increasingly tests:
- analytics workflows
- AI/ML services
- serverless analytics
- container orchestration
- modern cloud architectures

Questions are often framed like:

> “A company wants to run SQL queries directly against data stored in S3 without managing infrastructure.”

You must identify:
- Athena
- serverless analytics
- S3 integration

---

# Exam Keyword Triggers

| Scenario Keyword | Think |
|---|---|
| SQL on S3 | Athena |
| ETL/data integration | Glue |
| BI dashboards | QuickSight |
| Machine learning platform | SageMaker |
| Generative AI | Bedrock |
| Containers | ECS |
| Kubernetes | EKS |
| Serverless containers | Fargate |

---

# Quick Cram Guide

## Amazon Athena

Serverless query service.

Purpose:
- run SQL directly against S3 data

Benefits:
- no infrastructure management
- ad hoc analytics

---

## AWS Glue

Managed ETL and data integration service.

Purpose:
- data preparation
- data transformation
- metadata cataloging

---

## Amazon QuickSight

Business intelligence dashboard platform.

Purpose:
- reporting
- visual analytics
- dashboards

---

## Amazon Redshift

Cloud data warehouse.

Purpose:
- large-scale analytics
- BI workloads
- SQL analytics

---

## Amazon SageMaker

Managed machine learning platform.

Purpose:
- build
- train
- deploy ML models

---

## Amazon Bedrock

Managed generative AI service.

Purpose:
- access foundation models
- build AI applications
- generative AI workflows

---

## ECS

AWS-native container orchestration platform.

---

## EKS

Managed Kubernetes platform.

---

## Fargate

Serverless compute for containers.

---

# Analytics Workflow Pattern

```text
Data Sources
     ↓
Amazon S3
     ↓
AWS Glue
     ↓
Athena / Redshift
     ↓
QuickSight Dashboards
```

---

# AI/ML Architecture Pattern

```text
Applications
     ↓
Bedrock / SageMaker
     ↓
AI/ML Models
```

---

# Container Architecture Pattern

```text
Users
   ↓
Load Balancer
   ↓
ECS / EKS
   ↓
Containers
```

---

# Analytics & AI Service Comparison

| Requirement | AWS Service |
|---|---|
| SQL on S3 | Athena |
| ETL pipelines | Glue |
| BI dashboards | QuickSight |
| Enterprise analytics | Redshift |
| Machine learning | SageMaker |
| Generative AI | Bedrock |

---

# Operational Benefits

## Athena

Benefits:
- serverless analytics
- SQL on S3
- low operational overhead

---

## Glue

Benefits:
- managed ETL
- metadata catalog
- simplified data integration

---

## QuickSight

Benefits:
- cloud BI dashboards
- scalable analytics
- visual reporting

---

## SageMaker

Benefits:
- managed ML workflows
- model deployment
- training infrastructure

---

## Bedrock

Benefits:
- managed generative AI
- foundation model access
- no model infrastructure management

---

## ECS/EKS/Fargate

Benefits:
- scalable containers
- application portability
- microservices architectures

---

# Business Scenario Mapping

| Business Problem | AWS Solution |
|---|---|
| Query S3 with SQL | Athena |
| ETL workflows | Glue |
| Executive dashboards | QuickSight |
| Large-scale analytics | Redshift |
| ML model deployment | SageMaker |
| Generative AI apps | Bedrock |
| Container orchestration | ECS/EKS |

---

# Scenario-Based Questions

## 1.
A company wants to run SQL queries directly against data stored in S3.

### Which AWS service applies?

Answer:
Amazon Athena.

---

## 2.
A data engineering team needs a managed ETL service.

### Which AWS service should they use?

Answer:
AWS Glue.

---

## 3.
Executives need visual dashboards for analytics reporting.

### Which AWS service applies?

Answer:
Amazon QuickSight.

---

## 4.
A company wants a managed platform for building machine learning models.

### Which AWS service should be used?

Answer:
Amazon SageMaker.

---

## 5.
A company wants access to foundation models for generative AI applications.

### Which AWS service applies?

Answer:
Amazon Bedrock.

---

## 6.
A company standardized on Kubernetes for container orchestration.

### Which AWS service should they use?

Answer:
Amazon EKS.

---

## 7.
A company wants containers without managing EC2 servers.

### Which AWS service applies?

Answer:
AWS Fargate.

---

# Hands-On Activities

## Lab 1 — Explore Athena

Tasks:
1. Review Athena query editor
2. Explore SQL-on-S3 concepts
3. Review serverless analytics workflows

Goal:
Understand ad hoc analytics.

---

## Lab 2 — Review AI/ML Services

Tasks:
1. Compare SageMaker vs Bedrock
2. Review AI use cases
3. Explore foundation model concepts

Goal:
Understand AWS AI offerings.

---

## Lab 3 — Compare ECS vs EKS vs Fargate

Tasks:
1. Compare orchestration models
2. Review Kubernetes concepts
3. Compare operational overhead

Goal:
Understand container platform selection.

---

# Common Exam Mistakes

## Mistake 1
Confusing Athena and Redshift.

### Remember:
- Athena = serverless SQL on S3
- Redshift = data warehouse

---

## Mistake 2
Thinking Bedrock trains ML models.

### Remember:
Bedrock provides managed access to foundation models.

---

## Mistake 3
Confusing ECS and EKS.

### Remember:
- ECS = AWS-native containers
- EKS = Kubernetes

---

# Final Cram Summary

Memorize:

- Athena = SQL on S3
- Glue = ETL/data integration
- QuickSight = dashboards
- Redshift = analytics warehouse
- SageMaker = machine learning
- Bedrock = generative AI
- ECS = AWS containers
- EKS = Kubernetes
- Fargate = serverless containers

---

# High-Value Trigger Mapping

| Trigger Phrase | Likely Answer |
|---|---|
| SQL on S3 | Athena |
| ETL workflows | Glue |
| BI dashboards | QuickSight |
| Machine learning | SageMaker |
| Generative AI | Bedrock |
| Kubernetes | EKS |
| Serverless containers | Fargate |
