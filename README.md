# Hi, I'm Bartek

I study computer science at PJATK in Warsaw and build backend projects with **Java and Spring Boot**. I'm looking for a software engineering internship or a junior backend role. I expect to graduate in June 2028.

I also work as a residential architect, where I turn clients' requirements into design documents.

## Start here · Order & Inventory System

A B2B API for managing orders across multiple warehouses. Confirming an order reserves stock. Fulfilling it records the goods leaving the warehouse. Cancelling a confirmed order releases the reservation.

**What happens when two orders each request the last 10 units?** A PostgreSQL row lock makes the second confirmation wait. The integration test uses Testcontainers to run two transactions and checks the result. One order is confirmed, the second request returns `409 Conflict`, and the second order stays in draft. Exactly 10 units are reserved.

[Open the repository](https://github.com/bartlomiej-milosz/order-inventory-system) · [Read the concurrency test](https://github.com/bartlomiej-milosz/order-inventory-system/blob/2ed99aad2d60f1d6318d6aef5b1c02bfe51716eb/src/test/java/dev/bartlomiejmilosz/inventory/orders/OrderDraftTests.java#L628-L643) · [Run the Python demo](https://github.com/bartlomiej-milosz/order-inventory-system/blob/main/demo/README.md#start-here)

## Dev Assistant · Python

A command-line tool for asking questions about a GitHub repository. It checks each quote from a local Ollama model against the indexed source and links to the exact lines at that commit. If the quote is missing from the passage, the tool reports that it has insufficient evidence.

[Open Dev Assistant](https://github.com/bartlomiej-milosz/dev-assistant) · [Read the citation tests](https://github.com/bartlomiej-milosz/dev-assistant/blob/606627779939709319b1d50fb6f9b30a88a903d0/tests/test_answers.py#L10-L24)

[Connect on LinkedIn](https://www.linkedin.com/in/bartlomiej-milosz/)
