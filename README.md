**Junior Backend & Infrastructure Developer**

Computer Science student at PJATK focused on backend systems, Python, and Linux infrastructure. I like building core components from scratch - TCP/HTTP servers, request parsers, a DI container - to understand how things work at the implementation level instead of only wiring frameworks together. Five years of prior experience as a residential architect, bringing strong project management and analytical problem-solving skills to software engineering.

Currently building out a self-hosted homelab and working toward LFCS.

---

## Featured projects

### [Raw Network Stack](https://github.com/bartlomiej-milosz/raw-network-stack)
`Python · raw TCP sockets · Docker Compose · GitHub Actions`

Dependency-free, from-scratch network stack - four layers, each extending the last: `TCPServer` (raw sockets), `HTTPServer` (request parsing, routing), `ProxyServer` (reverse proxy via `select()` I/O multiplexing), and `LoadBalancerServer` (thread-safe round-robin). Full 5-container topology (3 backends + load balancer + proxy) orchestrated with Docker Compose; pytest suite covers concurrency and connection refusal edge cases; CI runs on every push via GitHub Actions.

### [Mini Spring Core](https://github.com/bartlomiej-milosz/mini-spring-core)
`Java · Reflection API · JUnit 5 · Maven`

Custom dependency-injection container replicating Spring's IoC - bean instantiation, singleton scope, `@Autowired` resolution, circular-dependency detection - with a JUnit 5 suite covering deep dependency chains. Built to understand framework internals from the ground up.

---

## Tech

| | |
|---|---|
| **Languages** | Python · Bash · Java |
| **Backend & Data** | REST APIs · TCP/HTTP Sockets · SQL (basics) |
| **Tooling & Testing** | pytest · Docker (basics) · Git · CI/CD fundamentals (GitHub Actions) · uv · ruff |
| **Linux & Systems** | Linux (daily driver) · Bash automation · self-hosted homelab · networking fundamentals (UDP / TCP / HTTP) · LFCS (in progress) |

---

## Contact

[Email](mailto:bartlomiej.milosz@gmail.com) · [LinkedIn](https://www.linkedin.com/in/) · Warsaw, Poland
