# EShoppingZone Centralized Config Repository (.properties)

This repository holds the centralized external `.properties` configurations for all **EShoppingZone Microservices** served via **Spring Cloud Config Server**.

## 📁 Repository Structure

* `application.properties` — Global default shared properties (Eureka, Actuator, Resilience4j defaults)
* `api-gateway.properties` — Spring Cloud API Gateway routes, predicates, and circuit breakers
* `auth-service.properties` — Authentication, JWT security, and user registration configs
* `profile-service.properties` — Profile and delivery address database configs
* `product-service.properties` — Product catalog and search database configs
* `cart-service.properties` — Cart database and ProductClient circuit breaker configs
* `order-service.properties` — Order lifecycle, database, and RabbitMQ events configs
* `inventory-service.properties` — Inventory stock management and reservation queue configs
* `payment-service.properties` — Payment transactions and WalletClient circuit breaker configs
* `wallet-service.properties` — Digital wallet balances and transaction configs
* `checkout-service.properties` — Checkout orchestrator and circuit breaker configs
* `notification-service.properties` — Email notifications and RabbitMQ listener configs
* `storefront.properties` — Web storefront Thymeleaf, H2 database, and OpenAI circuit breaker configs

---

## 🌐 How to View Configurations in Browser via Spring Cloud Config Server

When **`ConfigServerApplication`** is running on **Port `8888`**, you can open your browser to view the live JSON / Properties configurations for any service:

* **Cart Service**: `http://localhost:8888/cart-service/default` (or `http://localhost:8888/cart-service.properties`)
* **Product Service**: `http://localhost:8888/product-service/default` (or `http://localhost:8888/product-service.properties`)
* **Order Service**: `http://localhost:8888/order-service/default` (or `http://localhost:8888/order-service.properties`)
* **Payment Service**: `http://localhost:8888/payment-service/default` (or `http://localhost:8888/payment-service.properties`)
* **Checkout Service**: `http://localhost:8888/checkout-service/default` (or `http://localhost:8888/checkout-service.properties`)
* **API Gateway**: `http://localhost:8888/api-gateway/default` (or `http://localhost:8888/api-gateway.properties`)
* **Auth Service**: `http://localhost:8888/auth-service/default` (or `http://localhost:8888/auth-service.properties`)
* **Profile Service**: `http://localhost:8888/profile-service/default` (or `http://localhost:8888/profile-service.properties`)
* **Inventory Service**: `http://localhost:8888/inventory-service/default` (or `http://localhost:8888/inventory-service.properties`)
* **Wallet Service**: `http://localhost:8888/wallet-service/default` (or `http://localhost:8888/wallet-service.properties`)
* **Notification Service**: `http://localhost:8888/notification-service/default` (or `http://localhost:8888/notification-service.properties`)
* **Storefront**: `http://localhost:8888/storefront/default` (or `http://localhost:8888/storefront.properties`)
