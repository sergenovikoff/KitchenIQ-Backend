# KitchenIQ - Restaurant Management Backend

## Overview
KitchenIQ is a microservices-based restaurant management system designed to streamline restaurant operations. It includes features for user authentication, menu management, order processing, payments, inventory tracking, and reporting.

## Technologies Used
- **Backend:** Java Spring Boot (User, Menu, Payments, Inventory), C++ (High-performance order processing)
- **Database:** PostgreSQL with optimizations (Partitioning, Indexing, Caching)
- **API Gateway:** Spring Cloud Gateway
- **Event Handling:** Kafka/RabbitMQ for asynchronous messaging
- **Security:** OAuth2 + JWT-based authentication
- **DevOps:** Docker, Kubernetes, GitHub Actions

## Microservices Structure
- `user-service` – Handles user authentication and roles
- `menu-service` – Manages restaurant menu items
- `order-service` – C++ service for real-time order processing (gRPC)
- `payment-service` – Manages Stripe/PayPal transactions
- `inventory-service` – Tracks stock levels and low-stock alerts
- `gateway-service` – Routes API requests across services
- `event-broker` – Handles messaging between microservices (Kafka/RabbitMQ)

## Getting Started
### 1. Clone the Repository
```sh
git clone https://github.com/sergenovikoff/KitchenIQ-Backend.git
cd KitchenIQ-Backend
```

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request.

## License
This project is licensed under the MIT License.