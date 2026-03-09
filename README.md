# oci-networking-deep-dive

## Overview

Networking is a fundamental component of cloud architecture. Oracle Cloud Infrastructure provides a flexible and highly secure networking model that allows administrators to design isolated virtual networks for deploying applications.

This repository provides an in-depth explanation of OCI networking components including Virtual Cloud Networks (VCN), subnets, gateways, routing, and network security controls.

The goal of this project is to explain how these networking components interact to provide secure and scalable infrastructure.

---

## Core Networking Components

OCI networking is built using several components:

- Virtual Cloud Network (VCN)
- Subnets
- Route Tables
- Gateways
- Security Lists
- Network Security Groups

These components work together to control traffic flow and protect cloud workloads.

---

## Networking Architecture Example

Typical OCI networking architecture:


Internet
│
▼
Internet Gateway
│
▼
VCN
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

## Topics Covered

This repository explains the following OCI networking concepts:

- VCN architecture
- Subnet design strategies
- Gateway types and their roles
- Security Lists vs Network Security Groups
- Traffic routing and network flow

Each concept is explained in detail within the documentation folder.


## OCI Networking Architecture

![OCI Networking Architecture](architecture/oci-network-architecture.png)

## Detailed Documentation

- [VCN Overview](docs/vcn-overview.md)
- [Subnet Design](docs/subnet-design.md)
- [OCI Gateways](docs/gateways.md)
- [Security Lists vs Network Security Groups](docs/security-lists-vs-nsg.md)
- [Routing and Traffic Flow](docs/routing-and-traffic-flow.md)

---

## Learning Outcome

This guide demonstrates how networking infrastructure can be designed securely in Oracle Cloud Infrastructure using VCNs, routing policies, and network security controls.
