# Architecture patterns

## 1. Layered Architecture (n-tier)
This is a traditional architecture pattern where the system is divided into different layers, such as presentation, business logic, and data access layers. Each layer is responsible for a specific role and interacts only with the adjacent layers.

### Example
A typical web application where:
* The UI layer handles user interaction.
* The business logic layer handles the application's logic.
* The data access layer interacts with the database.

## 2. Modular Monolith
In a modular monolith, the system is developed as a single application (monolith), but it is organized into distinct, independent modules. Each module represents a specific domain or functionality within the system, but the entire system is deployed as one unit.

### Example
An ERP system where accounting, sales, and HR modules exist within the same application but are isolated from each other in code.

## 3. Microkernel Architecture (Plug-in Architecture)
The core functionality is minimal, and additional features are implemented as plug-ins or extensions that interact with the core. This architecture is suitable for products that require a robust base and can be extended with various plug-ins.

### Example
Eclipse IDE or Adobe Photoshop, where the core application is lightweight, but users can add different plug-ins to extend functionality.

## 4. Microservices Architecture
Microservices architecture divides the application into smaller, loosely coupled, independently deployable services. Each service focuses on a specific business function and communicates with other services using lightweight protocols (e.g., HTTP/REST, messaging).

### Example
Netflix uses microservices where services like user management, recommendations, and billing are separate microservices that work together.

## 5. Service-Based Architecture
This architecture is similar to microservices but with less strict boundaries. Services in this architecture are still separate but may share databases and more tightly coupled logic.

### Example
An e-commerce platform where services like inventory management, payment processing, and customer management are separate services, but they might share a common database.

## 6. Service-Oriented Architecture (SOA)
SOA is an older architecture pattern where services are reusable and communicate through a common messaging protocol, often via an enterprise service bus (ESB). SOA focuses on integrating various services into a single workflow.

### Example
Banking systems where different departments (e.g., loans, accounts, and transactions) expose their services and are integrated into a larger workflow through an ESB.

## 7. Event-Driven Architecture (EDA)
In EDA, components produce and consume events. The system reacts to events in real-time, often using an event bus or message broker to facilitate communication between producers and consumers.

### Example
Stock trading platforms where different services respond to events such as "new trade executed" or "price change," with each service reacting accordingly (e.g., updating portfolios, triggering alerts).
## 8. Space-Based Architecture
This architecture is designed for scalability by splitting the processing and data across multiple nodes (spaces). It aims to avoid bottlenecks by distributing load across spaces and using in-memory grids for fast data access.
### Example
Online gaming systems that handle large amounts of concurrent users by distributing game state and user data across multiple servers to balance the load.
