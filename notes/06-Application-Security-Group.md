# Application Security Group (ASG)

## Overview

An Application Security Group (ASG) is a logical grouping mechanism used with NSGs to organize virtual machines based on their application role.

## Purpose

ASGs make NSG rule management easier, especially in environments containing many virtual machines.

## Example

An organization may create:

- ASG-Web-Servers
- ASG-Management-Servers
- ASG-Application-Servers
- ASG-Database-Servers

Virtual machines can then be associated with the appropriate ASG.

## ASG and NSG

ASG does not independently filter network traffic.

Instead, ASGs are referenced in NSG rules to simplify traffic management.

## Example Rule

A rule could allow:

```text
Source: Internet
Destination: ASG-Web-Servers
Protocol: TCP
Ports: 80, 443
Action: Allow
