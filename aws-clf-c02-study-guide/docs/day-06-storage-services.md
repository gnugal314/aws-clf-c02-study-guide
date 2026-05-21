# DAY 6 — Storage Services Deep Dive

Source Reference: *Overview of Amazon Web Services AWS Whitepaper*

---

# Study Focus

This day focuses on AWS storage services and how organizations store, retrieve, archive, and protect data in the cloud.

Focus areas:
- Amazon S3
- EBS
- EFS
- Glacier
- Storage Gateway
- AWS Backup
- Storage classes
- Lifecycle policies
- Durability vs availability
- Object vs block vs file storage

---

# Why This Matters for the Exam

Storage is one of the most frequently tested CLF-C02 domains.

AWS commonly tests:
- storage selection
- cost optimization
- durability
- archival strategies
- shared storage
- EC2-attached storage

Questions are often framed like:

> “A company needs scalable durable object storage for backups and media files.”

You must identify:
- S3
- object storage
- scalable durable storage

---

# Exam Keyword Triggers

| Scenario Keyword | Think |
|---|---|
| Object storage | S3 |
| EC2 disk storage | EBS |
| Shared Linux filesystem | EFS |
| Long-term archive | Glacier |
| Hybrid storage | Storage Gateway |
| Lifecycle management | S3 lifecycle policies |
| Durable storage | S3 |

---

# Quick Cram Guide

## Amazon S3

Simple Storage Service.

Object storage platform.

Best for:
- backups
- media
- logs
- static websites
- data lakes

Benefits:
- virtually unlimited scalability
- high durability
- lifecycle management

---

## Amazon EBS

Elastic Block Store.

Persistent block storage attached to EC2 instances.

Best for:
- databases
- boot volumes
- transactional applications

---

## Amazon EFS

Elastic File System.

Managed shared Linux filesystem.

Best for:
- shared application storage
- multiple EC2 instances
- Linux workloads

---

## Amazon S3 Glacier

Low-cost archival storage.

Best for:
- long-term retention
- compliance archives
- infrequently accessed data

---

## AWS Storage Gateway

Hybrid storage integration between:
- on-premises infrastructure
- AWS cloud storage

---

## AWS Backup

Centralized backup management across AWS services.

---

# Storage Type Comparison

| Storage Type | AWS Service | Best Use Case |
|---|---|---|
| Object Storage | S3 | Files, backups, media |
| Block Storage | EBS | EC2 disks/databases |
| File Storage | EFS | Shared Linux storage |
| Archive Storage | Glacier | Long-term retention |

---

# Durability vs Availability

## Durability

Measures:
- likelihood data remains intact

S3 durability:
# 99.999999999%

(11 nines)

---

## Availability

Measures:
- ability to access data when needed

---

# S3 Storage Classes

| Storage Class | Use Case |
|---|---|
| Standard | Frequently accessed data |
| Standard-IA | Infrequent access |
| One Zone-IA | Lower-cost infrequent access |
| Glacier Instant Retrieval | Archive with faster access |
| Glacier Flexible Retrieval | Long-term archive |
| Glacier Deep Archive | Lowest-cost archival |

---

# Lifecycle Policies

Automatically move data between storage tiers.

Example:

```text
Day 0 → S3 Standard
Day 30 → S3 Standard-IA
Day 90 → Glacier
```

Purpose:
- cost optimization
- automated storage management

---

# Architecture Patterns

S3-Based Storage Pattern:

```text
Applications
  ↓
Amazon S3
  ↓
Lifecycle Policies
  ↓
Glacier Archive
```

---

Shared File Storage Pattern:

```text
EC2 Instance A
        ↓
      EFS
        ↑
EC2 Instance B
```

---

# Operational Benefits

## S3

Benefits:
- massive scalability
- durability
- serverless storage

---

## EBS

Benefits:
- low latency
- persistent storage
- EC2 integration

---

## EFS

Benefits:
- shared access
- elastic scaling
- managed filesystem

---

## Glacier

Benefits:
- low-cost retention
- compliance support

Tradeoff:
- slower retrieval times

---

# Business Scenario Mapping

| Business Problem | AWS Solution |
|---|---|
| Store files/backups | S3 |
| EC2 persistent storage | EBS |
| Shared Linux filesystem | EFS |
| Compliance archives | Glacier |
| Hybrid storage integration | Storage Gateway |

---

# Scenario-Based Questions

## 1.
A company needs highly durable scalable storage for images and backups.

### Which AWS service should be used?

Answer:
Amazon S3.

---

## 2.
An EC2 instance requires persistent block storage.

### Which AWS service applies?

Answer:
Amazon EBS.

---

## 3.
Multiple Linux servers need access to the same shared filesystem.

### Which AWS service should be used?

Answer:
Amazon EFS.

---

## 4.
A company wants low-cost long-term archival storage.

### Which AWS service applies?

Answer:
Amazon S3 Glacier.

---

## 5.
A company wants to automatically move old files into cheaper storage tiers.

### Which AWS capability applies?

Answer:
S3 Lifecycle Policies.

---

# Hands-On Activities

## Lab 1 — Create S3 Bucket

Tasks:
1. Create bucket
2. Upload files
3. Configure permissions

Goal:
Understand object storage basics.

---

## Lab 2 — Configure Lifecycle Policy

Tasks:
1. Create lifecycle rule
2. Transition objects to Glacier

Goal:
Understand storage optimization.

---

## Lab 3 — Explore EBS & EFS

Tasks:
1. Review EBS volume types
2. Compare EFS architecture
3. Identify use-case differences

Goal:
Understand storage selection.

---

# Common Exam Mistakes

## Mistake 1
Confusing S3 and EBS.

### Remember:
- S3 = object storage
- EBS = EC2 disk storage

---

## Mistake 2
Thinking EFS is Windows shared storage.

### Remember:
EFS is primarily Linux shared filesystem storage.

---

## Mistake 3
Using Glacier for frequently accessed data.

### Remember:
Glacier is archival storage.

---

# Final Cram Summary

Memorize:

- S3 = object storage
- EBS = EC2 block storage
- EFS = shared filesystem
- Glacier = archive storage
- Lifecycle Policies = automatic tiering
- Storage Gateway = hybrid storage

---

# High-Value Trigger Mapping

| Trigger Phrase | Likely Answer |
|---|---|
| Durable object storage | S3 |
| EC2 disk | EBS |
| Shared Linux storage | EFS |
| Long-term archive | Glacier |
| Automated storage optimization | Lifecycle Policies |
| Hybrid cloud storage | Storage Gateway |
