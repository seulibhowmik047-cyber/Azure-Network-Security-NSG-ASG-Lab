# Azure-Network-Security-NSG-ASG-Lab
Azure Network Security Lab covering Network Security Groups (NSG), Application Security Groups (ASG), network segmentation, security rules, RDP/HTTP/HTTPS traffic control, and Azure Network Manager concepts.
## Overview

This project demonstrates Azure network security using:

- Virtual Network (VNet)
- Subnets
- Network Security Group (NSG)
- Application Security Group (ASG)
- Virtual Machines
- Network segmentation
- RDP traffic control
- HTTP/HTTPS traffic control

## Objectives

- Create an Azure Virtual Network
- Create and configure Application Security Groups
- Create and associate a Network Security Group
- Configure inbound security rules
- Deploy Web and Management VMs
- Test RDP connectivity
- Test web server connectivity
- Understand network segmentation
- Reduce lateral movement

## Architecture

Internet
   |
   | HTTP/HTTPS
   v
Web Server VM

Management User
   |
   | RDP 3389
   v
Management Server VM

Both VMs are deployed inside the Azure VNet.

## Security Requirements

| Server | HTTP/HTTPS | RDP | Internet |
|---|---|---|---|
| Web Server | Allow | Deny | Allow |
| Management Server | Not Required | Allow | Deny |

## Technologies

- Microsoft Azure
- Azure Virtual Network
- Network Security Group
- Application Security Group
- Azure Virtual Machines
- IIS
- RDP

## Key Concepts

### NSG

Controls inbound and outbound network traffic using security rules.

### ASG

Provides logical grouping of VM network interfaces for easier NSG rule management.

### Network Segmentation

Reduces lateral movement and limits communication between network segments.

## Lab Result

- RDP to Management Server: Successful
- RDP to Web Server: Blocked
- Web Server HTTP/HTTPS access: Allowed
- Management Server Internet access: Restricted

## Conclusion

This lab demonstrates how NSG and ASG can be used to implement least-privilege network access and improve Azure network security.
