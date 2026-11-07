# Bartłomiej Miłosz

**Computer Science Student | Python Backend & Linux**

I'm a Computer Science student at PJATK in Warsaw, focusing on Python backend development with FastAPI and building my Linux administration skills. I'm interested in how services work end to end: from an HTTP request and a database transaction through to deployment and troubleshooting.

I'm looking for my first internship or junior role in **Python backend development or DevOps**. Python is my main language, for both backend development and automation.

## Selected projects

### [Boxing Club API](https://github.com/bartlomiej-milosz/boxing-club-api)

My main portfolio project: a FastAPI backend for a single boxing club, inspired by my interest in boxing. The first stage covers bearer-token authentication with role-based access (owner, trainer, member), rooms, dated classes, reservations, cancellations and trainer rosters. Memberships, payments, attendance and hosted deployment are planned for later stages.

The focus is on correctness under concurrent requests: PostgreSQL exclusion constraints prevent overlapping classes, row locking protects seat counts, and a unique index blocks duplicate reservations. Integration and race tests run against disposable PostgreSQL containers, and the project includes a reproducible Docker Compose setup with explicit migrations, health checks and CI. Linux deployment, monitoring and recovery are the next steps.

**Core stack:** Python · FastAPI · Pydantic · SQLAlchemy · PostgreSQL · Alembic · pytest · Docker Compose · GitHub Actions

### [Dotfiles](https://github.com/bartlomiej-milosz/dotfiles)

My macOS and Ubuntu shell and terminal setup (Zsh, Starship, Ghostty), managed with GNU Stow. It includes installation scripts and an offline check suite covering shell behavior, ShellCheck and configuration linking, configured to run in GitHub Actions.

## Linux learning

I'm studying Linux system administration with **RHCSA** as my certification goal.

- **RH104** — completed
- **RH124** — next course
- **RH134** — planned after RH124

Alongside Python, I have experience with Java from educational projects. My current focus is Python, backend systems and Linux.

## From architecture to IT

My professional background is in residential architecture, and I hold a master's degree in Architecture and Urban Planning. That work taught me to clarify client requirements, prepare precise technical documentation, coordinate with clients, designers and contractors, and communicate design changes clearly.

I bring those habits to software projects: understand the problem, make decisions explicit, document the reasoning and follow through on details.

Outside IT, I enjoy boxing, the inspiration for my main project.

[LinkedIn](https://www.linkedin.com/in/bartlomiej-milosz/)
