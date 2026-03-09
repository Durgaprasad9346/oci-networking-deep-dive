# Subnet Design in OCI

## Overview

Subnets divide a Virtual Cloud Network into smaller network segments. Each subnet contains cloud resources such as compute instances and load balancers.

Subnets help organize infrastructure and apply network security policies.

---

## Types of Subnets

OCI provides two types of subnets.

### Public Subnet

Resources inside a public subnet can communicate with the internet through an Internet Gateway.

Example resources:

- Bastion hosts
- Load balancers
- Public-facing services

---

### Private Subnet

Resources inside a private subnet cannot directly access the internet.

These resources typically communicate with the internet through a NAT Gateway.

Example resources:

- Application servers
- Databases
- Internal services

---

## Subnet Architecture


VCN
│
├── Public Subnet
│ │
│ ▼
│ Load Balancer
│
└── Private Subnet
│
▼
Application Servers



---

## Best Practices

Recommended subnet architecture:

- Public subnet for internet-facing services
- Private subnet for application workloads
- Separate database subnet for data isolation
