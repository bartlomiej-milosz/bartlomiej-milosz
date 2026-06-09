# Bartłomiej Miłosz

**Junior Software Developer** — Python · Bash · Backend & Data Processing

Computer Science student at PJATK focused on backend systems, Python, and Linux
infrastructure. I like building core components from scratch — TCP/HTTP servers,
request parsers, a DI container — to understand how things work at the
implementation level instead of only wiring frameworks together. Five years of
prior experience as a residential architect, now part-time while I move into
software.

Currently building out a self-hosted homelab, working toward LFCS, and learning
FastAPI.

---

## Featured projects

### [Real Estate Data Processing System](https://github.com/bartlomiej-milosz/real-estate-data-processing-system)
`Python · asyncio · httpx · SQLAlchemy · pandas · pydantic · Docker · pytest`

Async pipeline that scrapes, stores, cleans, and exports real-estate listings
across all 18 Warsaw districts. Async httpx client with bounded concurrency
(`asyncio.Semaphore`) and tenacity retries; SQLite via SQLAlchemy 2 as the single
source of truth, with idempotent, resumable upserts keyed on listing id.
Vectorised pandas cleaning into frozen pydantic v2 models (raw and typed schemas
kept separate as an audit trail), exposed through a typer CLI
(`scrape` / `clean` / `export`). Dockerised, with a pytest suite and CI on
GitHub Actions.

### [Mini Network Tools Series](https://github.com/bartlomiej-milosz/mini-http-server) *(in progress)*
`Python · raw TCP sockets · pytest`

From-scratch implementations of foundational backend infrastructure, to
internalise how networking and data transfer work under the hood. Python is used
as a thin language layer to keep focus on protocols and architecture.
**Done:** TCP server (abstract base class) and HTTP server (request parser,
response builder, mocked-socket test suite with pytest / pytest-mock).
**Planned:** load balancer, forward proxy.

### [Mini Spring Core](https://github.com/bartlomiej-milosz/mini-spring-core)
`Java · Reflection API · JUnit 5 · Maven`

Custom dependency-injection container replicating Spring's IoC — bean
instantiation, singleton scope, `@Autowired` resolution, circular-dependency
detection — with a JUnit 5 suite covering deep dependency chains. Built to
understand framework internals from the ground up.

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
