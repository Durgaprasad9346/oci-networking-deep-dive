# Security Lists vs Network Security Groups

## Overview

OCI provides two primary mechanisms for controlling network traffic:

- Security Lists
- Network Security Groups

Both act as virtual firewalls but operate at different levels.

---

## Security Lists

Security Lists apply at the subnet level.

Rules defined in a security list affect all resources deployed in that subnet.

Example rule:

Allow SSH access

Protocol: TCP
Port: 22
Source: 0.0.0.0/0



---

## Network Security Groups

Network Security Groups provide more granular network control.

Instead of applying rules to an entire subnet, NSGs allow rules to be applied to specific compute instances.

Benefits:

- Better security isolation
- Flexible rule management
- Application-level control

---

## Security Control Flow


Internet
│
▼
Security List
│
▼
Compute Instance
│
▼
Network Security Group



---

## Best Practice

Use Security Lists for basic subnet security and NSGs for fine-grained application security policies.

