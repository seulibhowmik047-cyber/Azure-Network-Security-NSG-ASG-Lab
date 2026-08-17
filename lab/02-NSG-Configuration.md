# NSG Configuration

## Objective

Create and associate a Network Security Group with the lab subnet.

## Steps

1. Open Azure Portal.
2. Search for Network Security Groups.
3. Create a new NSG.
4. Select the appropriate resource group.
5. Provide an NSG name.
6. Select the required Azure region.
7. Create the NSG.
8. Open the NSG.
9. Select Subnets.
10. Associate the NSG with the lab subnet.

## Association

The NSG is associated with the subnet so that the security rules can control traffic for workloads in that subnet.

## Security Goal

The NSG will be used to control:

- HTTP
- HTTPS
- RDP
- Other inbound and outbound traffic
