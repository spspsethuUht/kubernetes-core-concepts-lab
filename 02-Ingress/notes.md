# Ingress Notes

## What is Ingress?

Ingress provides Layer-7 routing for HTTP and HTTPS traffic.

Ingress routes user requests to backend services.

## Features

- Host Based Routing
- Path Based Routing
- SSL Termination
- Single Entry Point

## Examples

api.company.com

shop.company.com

blog.company.com

## Traffic Flow

Client

↓

Ingress

↓

Service

↓

Pod

## Advantages

- Better Routing Control
- Cost Effective
- Easier URL Management

## Key Takeaway

Ingress is commonly used in production Kubernetes environments to manage web traffic.
