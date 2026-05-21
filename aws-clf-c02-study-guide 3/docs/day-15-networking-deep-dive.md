# Day 15 Optional — AWS Networking, Access Control, and Network Provisioning Deep Dive

## Study Focus

This optional study day reinforces networking and access-control concepts that commonly confuse CLF-C02 learners.

## Key Concepts

- VPC
- Subnets
- CIDR blocks
- Route tables
- Internet Gateway
- NAT Gateway
- Security Groups
- Network ACLs
- Public vs private subnet
- Instance-level vs subnet-level controls
- IAM users, groups, roles, and policies

## Keyword Triggers

| Scenario Keyword | Think |
|---|---|
| Private network in AWS | Amazon VPC |
| Divide network into smaller ranges | Subnets |
| IP address range | CIDR |
| Public internet access | Internet Gateway |
| Private subnet outbound internet | NAT Gateway |
| Route traffic | Route Table |
| Instance firewall | Security Group |
| Subnet firewall | Network ACL |
| Temporary AWS permissions | IAM Role |
| Collection of users | IAM Group |
| Permission document | IAM Policy |
| Least privilege | Minimal IAM permissions |

## Cram Guide

### VPC
A logically isolated network in AWS where you define IP ranges, subnets, route tables, and access controls.

### CIDR
Defines an IP address range.

Example:
- `10.0.0.0/16` = large VPC network
- `10.0.1.0/24` = smaller subnet range

### Subnet
A smaller network segment inside a VPC.

- Public subnet: route to Internet Gateway
- Private subnet: no direct inbound internet access

### Route Table
Controls where network traffic goes.

Example:
- `0.0.0.0/0 -> Internet Gateway` means internet-bound traffic goes to the internet.

### Security Group
Instance-level firewall.

- Stateful
- Attached to EC2/resources
- Controls inbound/outbound traffic

### Network ACL
Subnet-level firewall.

- Stateless
- Applies to subnet traffic
- Supports allow and deny rules

## Instance-Level vs Subnet-Level Networking

| Layer | AWS Control | Scope | Stateful? |
|---|---|---|---|
| Instance level | Security Group | EC2/resource level | Yes |
| Subnet level | Network ACL | Entire subnet | No |
| Routing | Route Table | Subnet traffic paths | N/A |
| Identity access | IAM | AWS API/service access | N/A |

## Practice Questions

1. What AWS service provides an isolated virtual network?
   - Answer: Amazon VPC.

2. What does CIDR define?
   - Answer: An IP address range.

3. What is a subnet?
   - Answer: A smaller network segment inside a VPC.

4. What makes a subnet public?
   - Answer: It has a route to an Internet Gateway.

5. What does a route table do?
   - Answer: It determines where network traffic is routed.

6. Which AWS component allows public internet access from a VPC?
   - Answer: Internet Gateway.

7. Which AWS component allows private subnet resources outbound internet access?
   - Answer: NAT Gateway.

8. What is the instance-level firewall in AWS?
   - Answer: Security Group.

9. What is the subnet-level firewall in AWS?
   - Answer: Network ACL.

10. What IAM identity should be used for temporary permissions?
   - Answer: IAM Role.

## Scenario Questions

1. A company is building a three-tier web application. Web servers must be internet-facing, but the database must not be public. What should you recommend?
   - Answer: Place web servers in a public subnet and the database in a private subnet.

2. An EC2 instance in a public subnet cannot reach the internet. What should you check?
   - Answer: Verify the route table has a default route to an Internet Gateway.

3. A private application server needs outbound internet access for updates but no inbound internet traffic. What should you use?
   - Answer: NAT Gateway.

4. A security team wants firewall rules applied directly to EC2 instances. What should they use?
   - Answer: Security Groups.

5. A network team wants subnet-level allow and deny rules. What should they use?
   - Answer: Network ACLs.

6. An EC2 instance needs to access S3 without stored access keys. What should be used?
   - Answer: Attach an IAM Role to the EC2 instance.

7. Analysts need the same read-only permissions. What should be used?
   - Answer: IAM Group with a read-only policy.

8. A new app needs permission to read only one S3 bucket. What principle applies?
   - Answer: Least privilege.

9. A database should only accept traffic from app servers. What should be configured?
   - Answer: Security group rule allowing inbound traffic from the app server security group.

10. A company wants production and development workloads separated. What can help?
   - Answer: Separate VPCs, separate subnets, and controlled routing/security rules.
