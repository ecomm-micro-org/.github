# Microservices-based E-commerce Application

This repository contains the source code, infrastructure, and configuration for a microservices-based e-commerce application.

## Design
![system desig](https://github.com/ecomm-micro-org/.github/blob/main/profile/architecture.png?raw=true)

## Application Services & Port Mappings

Here is the list of all internal application microservices, where their source code is located, and the ports they are configured to run on.

| Service Name | Port (Local/Exposed) | Description |
|---|---|---|
| **API Gateway** | `6969` | Main entry point for all client requests, routing to respective internal services. |
| **Frontend UI** | `5173` | React frontend application powered by Vite. |
| **Service Registry (Eureka)** | `8761` | Netflix Eureka service registry for service discovery. |
| **Products Service** | `42069` | Manages products, inventory, and product embedding/similarity searches. |
| **Orders Service** | `42067` | Handles order creation, payment events (Razorpay), and fulfillment. |
| **Chat Client / GenAI Service** | `8086` | AI-powered chat and generation service utilizing Google GenAI API and embeddings. |
