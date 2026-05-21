# DAY 8 — Networking & Content Delivery Deep Dive

Source Reference: *Overview of Amazon Web Services AWS Whitepaper*

---

# Study Focus

This day focuses on AWS networking architecture and global content delivery.

Focus areas:
- Amazon VPC
- Route 53
- CloudFront
- Elastic Load Balancing
- Direct Connect
- VPN
- Security Groups
- Public vs Private Subnets
- Internet Gateway
- NAT Gateway
- Route Tables

---

# Why This Matters for the Exam

Networking concepts appear frequently on CLF-C02 because they connect:
- security
- compute
- scalability
- high availability

Questions are often framed like:

> “A company wants resources accessible from the internet while keeping databases private.”

You must identify:
- public subnets
- private subnets
- routing patterns
- networking security concepts

---

# Exam Keyword Triggers

| Scenario Keyword | Think |
|---|---|
| Private AWS network | VPC |
| Public internet access | Internet Gateway |
| Private outbound internet | NAT Gateway |
| DNS routing | Route 53 |
| Content delivery network | CloudFront |
| Traffic distribution | ELB |
| Dedicated AWS connection | Direct Connect |
| Instance firewall | Security Group |

---

# Quick Cram Guide

## Amazon VPC

Virtual Private Cloud.

Logically isolated AWS network.

Purpose:
- network segmentation
- IP range control
- routing management

---

## Route 53

Managed DNS service.

Purpose:
- domain management
- traffic routing
- health checks

---

## CloudFront

Global Content Delivery Network (CDN).

Purpose:
- reduce latency
- cache content globally
- improve performance

---

## Elastic Load Balancing (ELB)

Distributes traffic across resources.

Benefits:
- high availability
- fault tolerance
- scalability

---

## Internet Gateway

Allows public internet access from a VPC.

---

## NAT Gateway

Allows private subnet resources to access the internet outbound without allowing inbound internet access.

---

## Security Group

Stateful instance-level firewall.

---

# Public vs Private Subnets

## Public Subnet

Characteristics:
- route to Internet Gateway
- internet-accessible resources

Examples:
- web servers
- load balancers

---

## Private Subnet

Characteristics:
- no direct internet inbound access

Examples:
- databases
- internal applications

---

# Networking Architecture Pattern

```text
Internet
   ↓
Route 53
   ↓
CloudFront
   ↓
Load Balancer
   ↓
Public Subnet
   ↓
Private Subnet
```

---

# Networking Components Comparison

| Component | Purpose |
|---|---|
| VPC | Private AWS network |
| Route Table | Traffic routing |
| Internet Gateway | Public internet access |
| NAT Gateway | Private outbound internet |
| Security Group | Instance firewall |
| CloudFront | Global CDN |
| ELB | Traffic distribution |

---

# Operational Benefits

## VPC

Benefits:
- network isolation
- segmentation
- controlled routing

---

## CloudFront

Benefits:
- reduced latency
- faster content delivery
- caching

---

## Route 53

Benefits:
- scalable DNS
- routing policies
- failover routing

---

## ELB

Benefits:
- traffic balancing
- high availability
- automatic scaling support

---

# Business Scenario Mapping

| Business Problem | AWS Solution |
|---|---|
| Private cloud networking | VPC |
| Public web traffic | Internet Gateway |
| Private outbound internet | NAT Gateway |
| Global content acceleration | CloudFront |
| DNS routing | Route 53 |
| Traffic balancing | ELB |

---

# Scenario-Based Questions

## 1.
A company wants a logically isolated AWS network.

### Which AWS service applies?

Answer:
Amazon VPC.

---

## 2.
A web application needs global low-latency content delivery.

### Which AWS service should be used?

Answer:
Amazon CloudFront.

---

## 3.
A private application server needs outbound internet access without allowing inbound internet traffic.

### Which AWS component applies?

Answer:
NAT Gateway.

---

## 4.
A company wants to distribute traffic across multiple EC2 instances.

### Which AWS service should be used?

Answer:
Elastic Load Balancing.

---

## 5.
A company needs DNS routing for its applications.

### Which AWS service applies?

Answer:
Amazon Route 53.

---

# Hands-On Activities

## Lab 1 — Create Basic VPC

Tasks:
1. Create VPC
2. Configure subnet
3. Review route tables

Goal:
Understand private networking.

---

## Lab 2 — Explore CloudFront

Tasks:
1. Review edge locations
2. Compare CDN concepts
3. Explore caching behavior

Goal:
Understand global content delivery.

---

## Lab 3 — Compare Public vs Private Subnets

Tasks:
1. Draw architecture diagram
2. Identify internet routing
3. Compare subnet purposes

Goal:
Understand network segmentation.

---

# Common Exam Mistakes

## Mistake 1
Confusing Security Groups and Network ACLs.

### Remember:
- Security Groups = instance-level
- NACLs = subnet-level

---

## Mistake 2
Thinking NAT Gateway allows inbound public internet traffic.

### Remember:
NAT Gateway supports outbound-only internet access.

---

## Mistake 3
Confusing CloudFront and Route 53.

### Remember:
- Route 53 = DNS
- CloudFront = CDN

---

# Final Cram Summary

Memorize:

- VPC = private network
- Route 53 = DNS
- CloudFront = CDN
- ELB = traffic distribution
- Internet Gateway = public internet access
- NAT Gateway = private outbound internet
- Security Groups = instance firewall

---

# High-Value Trigger Mapping

| Trigger Phrase | Likely Answer |
|---|---|
| Private network | VPC |
| Global CDN | CloudFront |
| DNS routing | Route 53 |
| Traffic balancing | ELB |
| Public internet access | Internet Gateway |
| Private outbound internet | NAT Gateway |
