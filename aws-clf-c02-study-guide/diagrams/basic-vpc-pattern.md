# Basic VPC Pattern

```text
VPC: 10.0.0.0/16

Public Subnet: 10.0.1.0/24
- Internet Gateway route
- Web server
- NAT Gateway

Private Subnet: 10.0.2.0/24
- No direct inbound internet route
- App/database resources
- Outbound internet through NAT Gateway
```

## Traffic Flow

```text
Users
  ↓
Route 53
  ↓
CloudFront
  ↓
Load Balancer
  ↓
Public Subnet Web Tier
  ↓
Private Subnet App/Database Tier
```

## Security Pattern

```text
Security Group = instance/resource level firewall
Network ACL = subnet level firewall
Route Table = traffic path control
IAM = AWS API/service permission control
```
