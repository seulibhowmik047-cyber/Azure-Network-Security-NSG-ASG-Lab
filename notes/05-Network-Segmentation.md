# Network Segmentation

## Overview

Network segmentation divides a network into separate logical segments such as subnets.

Segmentation helps control communication between workloads and reduces unnecessary network access.

## Flat Network

A flat network has limited network segmentation and allows workloads to communicate more freely.

### Risks

- Higher lateral movement risk
- Larger attack surface
- Easier movement between compromised resources

## Segmented Network

A segmented network separates workloads into different subnets or security zones.

NSGs and other security controls can be used to control communication between segments.

## Example

An organization may separate:

- Web Servers
- Application Servers
- Database Servers
- Management Servers

Each segment can have different security rules.

## Lateral Movement

Lateral movement occurs when an attacker compromises one resource and then moves to other resources within the environment.

Network segmentation can reduce this risk by restricting unnecessary communication.

## Benefits

- Reduced attack surface
- Reduced lateral movement
- Better access control
- Improved security posture
- Easier security management

## Key Takeaway

Network segmentation is an important defense-in-depth strategy for protecting cloud workloads.
