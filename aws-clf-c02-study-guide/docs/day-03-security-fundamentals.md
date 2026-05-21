# DAY 3 — Security Fundamentals & Shared Responsibility Deep Dive

Source Reference: *Overview of Amazon Web Services AWS Whitepaper*

---

# Study Focus

This day focuses on AWS security fundamentals and identity/access management.

Focus areas:
- Shared Responsibility Model
- IAM users
- IAM groups
- IAM roles
- IAM policies
- Least privilege
- MFA
- Encryption
- Compliance
- Security best practices

---

# Why This Matters for the Exam

Security is one of the highest-weighted CLF-C02 domains.

AWS frequently tests:
- who secures what
- permission management
- IAM roles vs users
- encryption services
- security best practices

Questions are often framed like:

> “A company wants EC2 instances to securely access S3 without storing credentials.”

You must identify:
- IAM Roles
- least privilege
- temporary credentials

---

# Exam Keyword Triggers

| Scenario Keyword | Think |
|---|---|
| Permissions | IAM |
| Temporary credentials | IAM Role |
| Multiple users with same access | IAM Group |
| Permission document | IAM Policy |
| Encryption keys | KMS |
| Extra authentication layer | MFA |
| Principle of minimal access | Least Privilege |

---

# Quick Cram Guide

## Shared Responsibility Model

AWS secures:
# OF the cloud

Customers secure:
# IN the cloud

---

## AWS Secures

- physical datacenters
- networking infrastructure
- hardware
- hypervisor layer

---

## Customers Secure

- IAM permissions
- applications
- operating systems
- data
- encryption configurations

---

## IAM User

Permanent identity for:
- employees
- administrators
- applications

Uses:
- username/password
- access keys

---

## IAM Group

Collection of IAM users sharing common permissions.

Purpose:
- simplified permission management

---

## IAM Role

Temporary identity assumed by:
- AWS services
- applications
- federated users

Best practice:
# Use roles instead of hardcoded credentials

---

## IAM Policy

JSON document defining:
- allowed actions
- denied actions
- AWS resource access

---

## MFA

Multi-Factor Authentication.

Adds:
- second authentication factor
- improved account protection

---

## Least Privilege

Grant ONLY the permissions required to perform a task.

---

# Security Architecture Pattern

Traditional Credentials Pattern:

```text
Application
  ↓
Hardcoded Access Keys
```

Risk:
- credential exposure

---

Recommended AWS Pattern:

```text
Application
  ↓
IAM Role
  ↓
Temporary Credentials
```

Benefit:
- improved security
- credential rotation
- reduced exposure

---

# Encryption Concepts

## Encryption at Rest

Protects stored data.

Examples:
- S3 encryption
- EBS encryption
- RDS encryption

---

## Encryption in Transit

Protects data moving across networks.

Examples:
- HTTPS
- TLS

---

## AWS KMS

Managed encryption key service.

Purpose:
- centralized key management
- encryption governance

---

# Business Scenario Mapping

| Business Problem | AWS Solution |
|---|---|
| Secure user access | IAM |
| Shared team permissions | IAM Groups |
| Secure EC2 access to S3 | IAM Roles |
| Data encryption | KMS |
| Extra login security | MFA |

---

# Scenario-Based Questions

## 1.
A company wants developers to share the same AWS permissions.

### Which IAM feature should be used?

Answer:
IAM Groups.

---

## 2.
An EC2 instance needs access to S3 without storing credentials locally.

### Which AWS feature should be used?

Answer:
IAM Role.

---

## 3.
A security team wants centralized encryption key management.

### Which AWS service should they use?

Answer:
AWS KMS.

---

## 4.
A company wants additional protection for administrator accounts.

### Which AWS security feature should be enabled?

Answer:
MFA.

---

## 5.
A company wants users to have only the permissions required for their job responsibilities.

### Which security principle applies?

Answer:
Least privilege.

---

# Hands-On Activities

## Lab 1 — Create IAM Users & Groups

Tasks:
1. Create IAM user
2. Create IAM group
3. Attach permissions

Goal:
Understand identity management.

---

## Lab 2 — Configure MFA

Tasks:
1. Enable MFA on root account
2. Enable MFA for IAM user

Goal:
Understand account protection.

---

## Lab 3 — Explore IAM Roles

Tasks:
1. Create IAM Role
2. Assign role to EC2

Goal:
Understand temporary credentials.

---

# Common Exam Mistakes

## Mistake 1
Confusing IAM Users and IAM Roles.

### Remember:
- User = permanent identity
- Role = temporary assumed identity

---

## Mistake 2
Thinking AWS manages customer IAM permissions automatically.

### Remember:
Customers manage:
- permissions
- access control
- security configurations

---

## Mistake 3
Using overly broad permissions.

### Remember:
Always apply least privilege.

---

# Final Cram Summary

Memorize:

- IAM = permissions management
- Users = permanent identities
- Groups = shared permissions
- Roles = temporary credentials
- Policies = permission rules
- MFA = extra authentication layer
- KMS = encryption key management
- AWS secures OF the cloud
- Customers secure IN the cloud

---

# High-Value Trigger Mapping

| Trigger Phrase | Likely Answer |
|---|---|
| Temporary AWS access | IAM Role |
| Shared permissions | IAM Group |
| Permission document | IAM Policy |
| Encryption keys | KMS |
| Extra login protection | MFA |
| Minimal permissions | Least Privilege |
