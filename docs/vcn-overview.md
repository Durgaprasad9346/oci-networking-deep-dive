# Virtual Cloud Network (VCN)

## Overview

A Virtual Cloud Network (VCN) is the foundational networking component in Oracle Cloud Infrastructure. It is a logically isolated virtual network that allows cloud resources such as compute instances, load balancers, and databases to communicate securely.

A VCN functions similarly to a traditional on-premise network but is fully managed within OCI.

VCNs provide:

- Private IP addressing
- Network segmentation
- Secure communication between resources
- Controlled connectivity to the internet or on-premises networks

---

## VCN CIDR Block

When creating a VCN, you must define an IP range using CIDR notation.

Example:

10.0.0.0/16


10.0.0.0/16


## VCN Architecture Flow


Internet
│
▼
Internet Gateway
│
▼
Virtual Cloud Network
│
├── Public Subnet
│ │
│ ▼
│ Bastion Host
│
└── Private Subnet
│
▼
Application Servers



---

## Key Components inside a VCN

A typical VCN contains several networking components:

- Subnets
- Route tables
- Gateways
- Security Lists
- Network Security Groups

These components work together to control traffic flow and network security.

---

## Benefits of VCN

Using a VCN allows organizations to:

- Isolate workloads
- Implement secure network segmentation
- Control inbound and outbound traffic
- Connect cloud environments to on-premise networks
