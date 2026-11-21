# Hi, I'm Bartek

I study computer science at PJATK in Warsaw and build backend services with **Java and Spring Boot**. I'm looking for a software engineering internship or a junior backend role. Before moving into software, I worked in architecture, where I translated client requirements into technical documentation.

[LinkedIn](https://www.linkedin.com/in/bartlomiej-milosz/)

## Order & Inventory System

A B2B API for managing orders across multiple warehouses. Confirming an order reserves stock. Fulfilling it records the goods leaving the warehouse. Cancelling a confirmed order releases the reservation.

**When two orders each request the last 10 units**, a PostgreSQL row lock makes the second confirmation wait. Once the first transaction commits, the second gets an HTTP 409 and its order stays in draft. A Testcontainers integration test runs both transactions and checks which order was confirmed and how many units were reserved.

**Project stack** · Java 25 · Spring Boot · Spring Data JPA · Spring Security · PostgreSQL · Flyway · Testcontainers · Docker Compose · GitHub Actions

[Repository](https://github.com/bartlomiej-milosz/order-inventory-system) · [Concurrency test](https://github.com/bartlomiej-milosz/order-inventory-system/blob/2ed99aad2d60f1d6318d6aef5b1c02bfe51716eb/src/test/java/dev/bartlomiejmilosz/inventory/orders/OrderDraftTests.java#L628-L643) · [Run the Python demo](https://github.com/bartlomiej-milosz/order-inventory-system/blob/main/demo/README.md#start-here)
