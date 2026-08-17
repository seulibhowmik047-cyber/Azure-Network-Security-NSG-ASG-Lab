# Network Security Group (NSG)

## Overview

A Network Security Group (NSG) is a collection of inbound and outbound security rules used to allow or deny network traffic in Azure.

NSG rules are evaluated based on priority.

## NSG Rule Components

An NSG rule can contain:

- Source
- Source Port
- Destination
- Destination Port
- Protocol
- Action
- Priority

## Actions

The main actions are:

- Allow
- Deny

## Inbound Traffic

Inbound rules control traffic coming into a resource.

Examples:

- RDP
- HTTP
- HTTPS
- SSH

## Outbound Traffic

Outbound rules control traffic leaving a resource.

## NSG Association

An NSG can be associated with:

- A subnet
- A network interface (NIC)

## Default NSG Rules

Azure provides default NSG rules.

Important default rules include:

- AllowVNetInBound
- AllowVNetOutBound

These rules allow communication between resources within the same virtual network by default.

## Rule Priority

NSG rules are evaluated according to priority.

A lower numerical priority has higher precedence.

Example:

- Priority 100 → evaluated before 200
- Priority 200 → evaluated before 300

If a higher-priority rule matches the traffic, lower-priority rules are not evaluated for that traffic.

## Key Takeaway

NSGs provide basic network traffic filtering and are an important foundation of Azure network security.
