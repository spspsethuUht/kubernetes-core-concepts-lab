# NodePort Notes

## What is NodePort?

NodePort exposes an application externally through a port on every node.

The default NodePort range is:

30000 - 32767

## Traffic Flow

Browser

↓

NodeIP:NodePort

↓

Service

↓

Pod

## Use Cases

- Testing
- Development
- Small Environments

## Advantages

- Easy External Access
- No Additional Load Balancer Needed

## Key Takeaway

NodePort is simple and commonly used in labs and development environments.
