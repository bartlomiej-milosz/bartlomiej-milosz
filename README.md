**Junior Software Engineer — Python · Infrastructure · Backend**

Computer Science student at PJATK focused on backend systems, Python, and Linux infrastructure. I like building core components from scratch — TCP/HTTP servers, request parsers, a DI container — to understand how things work at the implementation level instead of only wiring frameworks together. Five years of prior experience as a residential architect, now part-time while I move into software.

Currently building out a self-hosted homelab and working toward LFCS.

---

## Featured projects

### [Raw Network Stack](https://github.com/bartlomiej-milosz/raw-network-stack)
`Python · raw TCP sockets · Docker Compose · GitHub Actions`

Dependency-free, from-scratch network stack — four layers, each extending the last: `TCPServer` (raw sockets), `HTTPServer` (request parsing, routing), `ProxyServer` (reverse proxy via `select()` I/O multiplexing), and `LoadBalancerServer` (thread-safe round-robin). Full 5-container topology (3 backends + load balancer + proxy) orchestrated with Docker Compose; pytest suite covers concurrency and connection refusal edge cases; CI runs on every push via GitHub Actions.

### [Real Estate Data Processing System](https://github.com/bartlomiej-milosz/real-estate-data-processing-system)
`Python · asyncio · httpx · SQLAlchemy · pandas · pydantic · Docker · pytest`

Async pipeline that scrapes, stores, cleans, and exports real-estate listings across all 18 Warsaw districts. Async httpx client with bounded concurrency (`asyncio.Semaphore`) and tenacity retries; SQLite via SQLAlchemy 2 as the single source of truth, with idempotent, resumable upserts keyed on listing id. Vectorised pandas cleaning into frozen pydantic v2 models (raw and typed schemas kept separate as an audit trail), exposed through a typer CLI (`scrape` / `clean` / `export`). Dockerised, with a pytest suite and CI on GitHub Actions.

### [Mini Spring Core](https://github.com/bartlomiej-milosz/mini-spring-core)
`Java · Reflection API · JUnit 5 · Maven`

Custom dependency-injection container replicating Spring's IoC — bean instantiation, singleton scope, `@Autowired` resolution, circular-dependency detection — with a JUnit 5 suite covering deep dependency chains. Built to understand framework internals from the ground up.

---

## Tech

| | |
|---|---|
| **Languages** | Python · Bash · Java |
| **Backend & Data** | REST APIs · asyncio · pandas · FastAPI *(learning)* |
| **Tooling & Testing** | pytest · Docker · Git · GitHub Actions · uv · ruff |
| **Linux & Systems** | Linux (daily driver) · Bash automation · self-hosted homelab · networking fundamentals (UDP / TCP / HTTP) |

---

## Contact

[Email](mailto:bartlomiej.milosz@gmail.com) · [LinkedIn](https://www.linkedin.com/in/) · Warsaw, Poland
