# Bartłomiej Miłosz

I build backend systems and tools that use language models. I'm looking for a software engineering internship or a junior developer role.

I study computer science part-time at PJATK in Warsaw and expect to graduate in June 2028. Alongside my studies, I work as a residential architect.

## [Order & Inventory System](https://github.com/bartlomiej-milosz/order-inventory-system)

**Java · Spring Boot · PostgreSQL · Flyway · Testcontainers · Docker**

Two orders each request the last 10 units in a warehouse. The API takes a pessimistic write lock on the stock row before checking availability. When both confirmations arrive together, one order reserves all 10 units. The other waits, then gets `409 Conflict` and stays in draft.

[Read the concurrency test](https://github.com/bartlomiej-milosz/order-inventory-system/blob/2ed99aad2d60f1d6318d6aef5b1c02bfe51716eb/src/test/java/dev/bartlomiejmilosz/inventory/orders/OrderDraftTests.java#L628-L643) · [See the locking query](https://github.com/bartlomiej-milosz/order-inventory-system/blob/2ed99aad2d60f1d6318d6aef5b1c02bfe51716eb/src/main/java/dev/bartlomiejmilosz/inventory/inventory/StockLevelRepository.java#L36-L43)

## [Dev Assistant](https://github.com/bartlomiej-milosz/dev-assistant)

**Python · PostgreSQL · pgvector · Ollama**

This command-line tool uses retrieval-augmented generation (RAG) to answer questions about a GitHub repository. It indexes one commit, retrieves relevant passages and passes them to a local language model. Each answer includes a quote and a link to the exact lines. If the model invents a quote, the CLI withholds the answer.

I used the order system as a test case. Asked which user runs the backend container, the tool found the Dockerfile and quoted [`USER 10001:10001`](https://github.com/bartlomiej-milosz/order-inventory-system/blob/2ed99aad2d60f1d6318d6aef5b1c02bfe51716eb/Dockerfile#L18).

[Read the citation tests](https://github.com/bartlomiej-milosz/dev-assistant/blob/606627779939709319b1d50fb6f9b30a88a903d0/tests/test_answers.py#L11-L24) · [Compare text and vector search in the notebook](https://github.com/bartlomiej-milosz/dev-assistant/blob/606627779939709319b1d50fb6f9b30a88a903d0/notebooks/retrieval-evaluation.ipynb)

[Connect on LinkedIn](https://www.linkedin.com/in/bartlomiej-milosz/)
