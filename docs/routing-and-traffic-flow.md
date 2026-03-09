# Routing and Traffic Flow in OCI

## Overview

Routing determines how network traffic moves between resources within a VCN and external networks.

OCI uses route tables to define how traffic should be directed.

---

## Route Tables

A route table contains rules that specify the destination and the target gateway.

Example rule:

Destination:

0.0.0.0/0

Target:
Internet Gateway


This allows internet-bound traffic from the subnet.

---

## Traffic Flow Example

Typical OCI application architecture:


User
│
▼
Internet
│
▼
Internet Gateway
│
▼
Public Subnet
│
▼
Load Balancer
│
▼
Private Subnet
│
▼
Application Servers



---

## Internal Traffic

Instances inside the same VCN can communicate using private IP addresses without leaving the network.

Example:


App Server → Database Server


---

## Benefits of Proper Routing

Effective routing design helps:

- Improve security
- Control network paths
- Optimize traffic performance
- Enable hybrid connectivity
