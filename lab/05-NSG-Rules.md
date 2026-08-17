# NSG Security Rules

## Objective

Configure NSG rules to implement the required network access.

## Web Server Rule

Allow web traffic to the Web Server ASG.

```text
Source: Any
Destination: Web Server ASG
Protocol: TCP
Destination Ports: 80, 443
Action: Allow
