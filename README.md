# Hi, I'm Bartek

I build Java APIs and Python tools as personal projects. I study computer science part-time at PJATK in Warsaw, alongside my work as a residential architect. I expect to graduate in June 2028.

## [Order & Inventory System](https://github.com/bartlomiej-milosz/order-inventory-system)

Two orders each request the last 10 units in a warehouse. What happens when both confirmation requests arrive together?

[Read the concurrency test](https://github.com/bartlomiej-milosz/order-inventory-system/blob/2ed99aad2d60f1d6318d6aef5b1c02bfe51716eb/src/test/java/dev/bartlomiejmilosz/inventory/orders/OrderDraftTests.java#L628-L643). It holds one PostgreSQL transaction open while a second transaction tries to reserve the same stock. One order gets all 10 units. The other stays in draft, and its confirmation request returns `409 Conflict`.

The Spring Boot API also handles what happens next. Shipping a confirmed order deducts the stock. Cancelling it releases the reservation. [Run the order walkthrough](https://github.com/bartlomiej-milosz/order-inventory-system/blob/main/demo/README.md#fulfillment-and-cancellation).

## [Dev Assistant](https://github.com/bartlomiej-milosz/dev-assistant)

Ask this Python CLI a question about a repository and you can check the model's answer against the code. It quotes the source and links to the exact lines at the indexed commit. If the model invents a quote, the CLI withholds the answer. [See the citation tests](https://github.com/bartlomiej-milosz/dev-assistant/blob/606627779939709319b1d50fb6f9b30a88a903d0/tests/test_answers.py#L10-L24).

I'm looking for a software engineering internship or junior backend role. [Connect on LinkedIn](https://www.linkedin.com/in/bartlomiej-milosz/).
