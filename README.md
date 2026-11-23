# Bartłomiej Miłosz

I build backend APIs in Java and integrate local language models into Python developer tools. I'm looking for a software engineering internship or a junior developer role.

I study computer science part-time at PJATK in Warsaw and expect to graduate in June 2028. As a self-employed residential architect, I work directly with clients to define project scope and document design changes.

## [Order & Inventory System](https://github.com/bartlomiej-milosz/order-inventory-system)

**Java · Spring Boot · PostgreSQL · Flyway · Testcontainers · Docker**

This API tracks orders and stock across warehouses, from reservation to shipment or cancellation.

Two orders each request the last 10 units in a warehouse. To prevent a double reservation, the API takes a pessimistic write lock on the stock row before checking availability. The first order reserves all 10 units. The second confirmation waits for the first transaction to commit, then returns `409 Conflict`. That order stays in draft.

[Read the concurrency test](https://github.com/bartlomiej-milosz/order-inventory-system/blob/2ed99aad2d60f1d6318d6aef5b1c02bfe51716eb/src/test/java/dev/bartlomiejmilosz/inventory/orders/OrderDraftTests.java#L628-L643) · [See the locking query](https://github.com/bartlomiej-milosz/order-inventory-system/blob/2ed99aad2d60f1d6318d6aef5b1c02bfe51716eb/src/main/java/dev/bartlomiejmilosz/inventory/inventory/StockLevelRepository.java#L36-L43)

## [Dev Assistant](https://github.com/bartlomiej-milosz/dev-assistant)

**Python · PostgreSQL · pgvector · Ollama**

This CLI uses retrieval-augmented generation (RAG) to answer questions about code. It links each quote to the indexed commit and withholds the answer if the model invents a quote.

On six held-out questions about the order system, PostgreSQL full-text search ranked the expected source in the top three for all six. Vector search did so for four. The CLI defaults to full-text search.

[Read the citation tests](https://github.com/bartlomiej-milosz/dev-assistant/blob/606627779939709319b1d50fb6f9b30a88a903d0/tests/test_answers.py#L11-L24) · [Explore the retrieval experiment](https://github.com/bartlomiej-milosz/dev-assistant/blob/606627779939709319b1d50fb6f9b30a88a903d0/notebooks/retrieval-evaluation.ipynb)

## Availability & contact

I'm available to start full-time immediately and prefer hybrid work in Warsaw.

[bartlomiej.milosz@gmail.com](mailto:bartlomiej.milosz@gmail.com) · [LinkedIn](https://www.linkedin.com/in/bartlomiej-milosz/)
