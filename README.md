# EShoppingZone Centralized Config Repository

This repository holds the centralized external configurations for all **EShoppingZone Microservices** served via **Spring Cloud Config Server**.

## 📁 Repository Structure

* `application.yml` — Global default shared properties (Eureka, Actuator, Resilience4j defaults)
* `api-gateway.yml` — Spring Cloud API Gateway routes, predicates, and circuit breakers
* `auth-service.yml` — Authentication, JWT security, and user registration configs
* `profile-service.yml` — Profile and delivery address database configs
* `product-service.yml` — Product catalog and search database configs
* `cart-service.yml` — Cart database and ProductClient circuit breaker configs
* `order-service.yml` — Order lifecycle, database, and RabbitMQ events configs
* `inventory-service.yml` — Inventory stock management and reservation queue configs
* `payment-service.yml` — Payment transactions and WalletClient circuit breaker configs
* `wallet-service.yml` — Digital wallet balances and transaction configs
* `checkout-service.yml` — Checkout orchestrator and circuit breaker configs
* `notification-service.yml` — Email notifications and RabbitMQ listener configs
* `storefront.yml` — Web storefront Thymeleaf, H2 database, and OpenAI circuit breaker configs

---

## 🌐 How to View Configurations in Browser via Spring Cloud Config Server

When **`ConfigServerApplication`** is running on **Port `8888`**, you can open your browser to view the live JSON configurations for any service:

* **Cart Service**: `http://localhost:8888/cart-service/default`
* **Product Service**: `http://localhost:8888/product-service/default`
* **Order Service**: `http://localhost:8888/order-service/default`
* **Payment Service**: `http://localhost:8888/payment-service/default`
* **Checkout Service**: `http://localhost:8888/checkout-service/default`
* **API Gateway**: `http://localhost:8888/api-gateway/default`
* **Auth Service**: `http://localhost:8888/auth-service/default`
* **Profile Service**: `http://localhost:8888/profile-service/default`
* **Inventory Service**: `http://localhost:8888/inventory-service/default`
* **Wallet Service**: `http://localhost:8888/wallet-service/default`
* **Notification Service**: `http://localhost:8888/notification-service/default`
* **Storefront**: `http://localhost:8888/storefront/default`
