# VNet Architecture

## Objective

Create an Azure Virtual Network and subnet for the NSG and ASG lab.

## Architecture

The lab contains:

- One Virtual Network
- One subnet
- Web Server VM
- Management Server VM
- Network Security Group
- Web Server ASG
- Management Server ASG

## Logical Design

```text
Internet
   |
   |--- HTTP/HTTPS ---> Web Server
   |
   |--- RDP ----------> Management Server
                         |
                     Virtual Network
                         |
                       Subnet
                         |
                       NSG
