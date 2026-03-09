# OCI Gateways

## Overview

Gateways allow resources inside a VCN to communicate with external networks or services.

OCI provides several gateway types depending on the required connectivity.

---

## Internet Gateway

An Internet Gateway allows resources in a public subnet to communicate with the public internet.

Example:

Users accessing a public web application.

---

## NAT Gateway

A NAT Gateway allows resources in private subnets to access the internet without exposing them to inbound internet traffic.

Example use case:

Application servers downloading software updates.

---

## Service Gateway

A Service Gateway allows private access to OCI services without sending traffic through the public internet.

Example services:

- Object Storage
- Autonomous Database

---

## Dynamic Routing Gateway

A Dynamic Routing Gateway enables hybrid cloud connectivity between OCI and on-premise networks.

Used for:

- Site-to-site VPN
- FastConnect

---

## Gateway Connectivity Flow

Private Instance
│
▼
NAT Gateway
│
▼
Internet

