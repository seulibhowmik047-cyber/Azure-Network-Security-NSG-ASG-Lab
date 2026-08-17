# ASG Configuration

## Objective

Create Application Security Groups for different workload types.

## ASGs Created

### Web Server ASG

Used to group Web Server virtual machines.

### Management Server ASG

Used to group Management Server virtual machines.

## Purpose

ASGs provide logical grouping of virtual machines so that NSG rules can reference workload groups instead of individual IP addresses.

## Configuration

The following ASGs were created:

- ASG-Web-Servers
- ASG-Management-Servers

The appropriate virtual machines were then associated with their respective ASGs.
