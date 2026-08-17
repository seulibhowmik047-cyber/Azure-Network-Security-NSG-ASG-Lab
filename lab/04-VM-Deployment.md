# Virtual Machine Deployment

## Objective

Deploy two Windows virtual machines for the network security lab.

## Virtual Machines

### Web Server VM

Purpose:

- Host web services
- Allow HTTP/HTTPS traffic
- Test internet connectivity

### Management Server VM

Purpose:

- Administrative access
- RDP testing
- Test restricted internet access

## Network Configuration

Both virtual machines are deployed into the lab Virtual Network and subnet.

The subnet is protected by the configured NSG.

## Public Inbound Ports

Public inbound ports were not opened through the VM creation wizard because the lab uses the subnet-level NSG to control traffic.

## ASG Association

- Web Server VM → Web Server ASG
- Management Server VM → Management Server ASG
