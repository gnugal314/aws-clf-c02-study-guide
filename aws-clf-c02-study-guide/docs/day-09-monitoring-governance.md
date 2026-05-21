# DAY 9 — Monitoring & Governance Deep Dive

Source Reference: *Overview of Amazon Web Services AWS Whitepaper*

---

# Study Focus

This day focuses on AWS monitoring, logging, governance, auditing, and operational visibility.

Focus areas:
- CloudWatch
- CloudTrail
- AWS Config
- Trusted Advisor
- AWS Organizations
- Control Tower
- Governance frameworks
- Logging
- Compliance
- Operational monitoring

---

# Why This Matters for the Exam

AWS frequently tests:
- operational visibility
- auditing
- compliance
- governance services
- logging distinctions

Questions are often framed like:

> “A company wants to track all AWS API activity for auditing purposes.”

You must identify:
- CloudTrail
- audit logging
- governance concepts

---

# Exam Keyword Triggers

| Scenario Keyword | Think |
|---|---|
| Metrics and monitoring | CloudWatch |
| API audit logging | CloudTrail |
| Resource configuration tracking | Config |
| Best-practice recommendations | Trusted Advisor |
| Multi-account management | AWS Organizations |
| Compliance visibility | Config |

---

# Quick Cram Guide

## CloudWatch

Monitoring and observability platform.

Purpose:
- metrics
- logs
- alarms
- dashboards

---

## CloudTrail

Records AWS API activity.

Purpose:
- auditing
- governance
- compliance
- forensic investigation

---

## AWS Config

Tracks AWS resource configurations over time.

Purpose:
- compliance visibility
- configuration tracking
- change monitoring

---

## Trusted Advisor

Provides AWS best-practice recommendations.

Categories:
- cost optimization
- security
- performance
- fault tolerance

---

## AWS Organizations

Centralized multi-account management.

Purpose:
- governance
- account organization
- policy management

---

# Monitoring vs Auditing

| Requirement | AWS Service |
|---|---|
| Infrastructure metrics | CloudWatch |
| API auditing | CloudTrail |
| Configuration tracking | Config |
| Optimization recommendations | Trusted Advisor |

---

# Architecture Pattern

```text
AWS Resources
     ↓
CloudWatch Metrics & Logs
     ↓
CloudTrail API Activity
     ↓
AWS Config Compliance Tracking
```

---

# Operational Benefits

## CloudWatch

Benefits:
- centralized monitoring
- alerting
- operational visibility

---

## CloudTrail

Benefits:
- audit trail
- governance support
- security investigations

---

## Config

Benefits:
- compliance tracking
- change history
- resource inventory

---

## Trusted Advisor

Benefits:
- optimization insights
- cost savings
- security recommendations

---

# Business Scenario Mapping

| Business Problem | AWS Solution |
|---|---|
| Monitor application health | CloudWatch |
| Audit AWS activity | CloudTrail |
| Track resource changes | Config |
| Improve AWS best practices | Trusted Advisor |
| Multi-account governance | Organizations |

---

# Scenario-Based Questions

## 1.
A company wants alerts when CPU utilization becomes too high.

### Which AWS service applies?

Answer:
Amazon CloudWatch.

---

## 2.
A security team wants to track all AWS API calls.

### Which AWS service should be used?

Answer:
AWS CloudTrail.

---

## 3.
A company wants to track AWS resource configuration changes over time.

### Which AWS service applies?

Answer:
AWS Config.

---

## 4.
A company wants recommendations for reducing AWS costs.

### Which AWS service should they use?

Answer:
AWS Trusted Advisor.

---

## 5.
A company wants centralized governance across multiple AWS accounts.

### Which AWS service applies?

Answer:
AWS Organizations.

---

# Hands-On Activities

## Lab 1 — Explore CloudWatch

Tasks:
1. Create CloudWatch alarm
2. Review metrics dashboard
3. Explore logs

Goal:
Understand AWS monitoring.

---

## Lab 2 — Review CloudTrail Logs

Tasks:
1. Explore API activity history
2. Review user actions
3. Identify audit records

Goal:
Understand AWS auditing.

---

## Lab 3 — Explore Trusted Advisor

Tasks:
1. Review recommendations
2. Identify security checks
3. Explore cost optimization suggestions

Goal:
Understand governance optimization.

---

# Common Exam Mistakes

## Mistake 1
Confusing CloudWatch and CloudTrail.

### Remember:
- CloudWatch = monitoring
- CloudTrail = API auditing

---

## Mistake 2
Thinking Config is a monitoring tool.

### Remember:
Config tracks resource configurations and compliance.

---

## Mistake 3
Confusing Trusted Advisor with CloudWatch.

### Remember:
Trusted Advisor gives recommendations, not operational monitoring.

---

# Final Cram Summary

Memorize:

- CloudWatch = metrics/logs/alarms
- CloudTrail = API auditing
- Config = configuration tracking
- Trusted Advisor = best-practice recommendations
- Organizations = multi-account governance

---

# High-Value Trigger Mapping

| Trigger Phrase | Likely Answer |
|---|---|
| Metrics monitoring | CloudWatch |
| API audit logs | CloudTrail |
| Compliance tracking | Config |
| AWS recommendations | Trusted Advisor |
| Multi-account governance | Organizations |
