<img src="../assets/cover.svg" width="100%" alt="nepotato — full-stack development. Interfaces, systems, delivery." />

[Profile overview](../README.md) · [Русская версия](portfolio.ru.md) · [Memora](https://memorasolutions.ru) · [RuMarket](https://statik.obdrisher.ru/) · [Repositories](https://github.com/arar228?tab=repositories)

[Browse the public project catalogue](../PROJECTS.md) — product case studies, frontend
experiments, Telegram tools, learning material and ecosystem work.

I build web products, Telegram Mini Apps and interactive tools. My projects connect **React interfaces, server-side logic and data storage** with tests and release workflows.

## Project portfolio

### Memora Solutions

**Product platform · React / Node.js / PostgreSQL / Python / Electron**

A connected set of productivity tools: a web/desktop focus timer, travel-deal discovery, Kanban and Telegram integrations.

- A shared Pomodoro renderer with separate browser and desktop storage adapters.
- Payment-event verification, idempotent delivery and recovery paths in the Travel Radar service.
- Release checks tied to an exact commit, health checks and application rollback on the VPS.

[Live product](https://memorasolutions.ru) · [Source](https://github.com/arar228/memora-solutions) · [Architecture](https://github.com/arar228/memora-solutions/blob/master/docs/architecture.md) · [CI](https://github.com/arar228/memora-solutions/actions/workflows/ci.yml)

### Night Arcade

**Full-stack prototype · TypeScript / React / Fastify / Prisma / PostgreSQL**

A Telegram Mini App built around virtual game points, a ledger, daily rewards and server-resolved game rounds. The public repository is named `potato`.

- Shared Zod contracts connect the web client and API.
- The server owns balances and game outcomes; the client presents the result.
- Unit tests exercise game rules, authentication and wallet-service behavior with mocked persistence.

**Scope:** play-money prototype. PvP is an Arcade Bot demonstration; production multiplayer and real-payment readiness are outside the verified scope.

[Source & setup](https://github.com/arar228/potato) · [Engineering case study](https://github.com/arar228/potato/blob/main/docs/CASE_STUDY.md)

### Procedural GPU

**Creative engineering · TypeScript / Three.js / WebGL**

An editable triple-fan graphics card built from procedural geometry. A reusable model API sits alongside an interactive browser demo.

<a href="https://arar228.github.io/nepotato-threejs-gpu/"><img src="https://raw.githubusercontent.com/arar228/nepotato-threejs-gpu/main/docs/preview.png" width="640" alt="Preview of the procedural triple-fan GPU model; open the interactive demo" /></a>

[Interactive demo](https://arar228.github.io/nepotato-threejs-gpu/) · [Source & API](https://github.com/arar228/nepotato-threejs-gpu)

### RuMarket

**Economic intelligence · Python / pandas / NumPy / SciPy / JavaScript**

An explainable, continuously updated monitor of the Russian economy and financial markets. It combines official statistics, market prices, credit conditions and corporate reporting in one source-aware interface.

- Automated collection from Moscow Exchange, the Bank of Russia, Rosstat and the Ministry of Finance.
- Validation gates for freshness, coverage, plausible ranges and required fiscal indicators.
- Scheduled rebuilds, health snapshots, last-known-good data and delivery recovery checks.

[Live product](https://statik.obdrisher.ru/) · [Engineering case study](https://github.com/arar228/rumarket-showcase) · [Architecture](https://github.com/arar228/rumarket-showcase/blob/main/docs/architecture.md)

### TON Subscriptions Protocol

**Contract engineering · Tolk / TypeScript / TON Sandbox**

Recurring-payment channel research: deterministic addresses, timed state transitions, pause/resume semantics and tests for bounced transfers.

**Scope:** the public repository covers contracts and sandbox tests. Real-funds use requires an independent security audit; the separate application services are outside this repository.

[Source & architecture](https://github.com/arar228/ton-subscriptions-protocol) · [Sandbox tests](https://github.com/arar228/ton-subscriptions-protocol/tree/master/tests)

## Engineering decisions to explore

| Question | Where to look |
| --- | --- |
| How can one UI support web and desktop persistence? | [Memora component map](https://github.com/arar228/memora-solutions/blob/master/docs/component-map.md) |
| How are payment retries and release rollback handled? | [Memora operations guide](https://github.com/arar228/memora-solutions/blob/master/docs/operations.md) |
| Which rules belong on the server? | [Night Arcade case study](https://github.com/arar228/potato/blob/main/docs/CASE_STUDY.md) |
| How can an automated analytical pipeline expose source quality and freshness? | [RuMarket architecture](https://github.com/arar228/rumarket-showcase/blob/main/docs/architecture.md) |
| What happens when an asynchronous transfer bounces? | [Channel bounce tests](https://github.com/arar228/ton-subscriptions-protocol/blob/master/tests/ChannelJettonBounce.spec.ts) |

## Stack across these projects

**Frontend** — TypeScript, React, Vite, Tailwind CSS, Three.js<br>
**Backend & data** — Node.js, Fastify, Python, PostgreSQL, Prisma, Zod, pandas, NumPy, SciPy<br>
**Delivery & verification** — GitHub Actions, unit tests, reproducible builds, health checks

Each repository documents its own setup and verification boundaries. Live demos, local prototypes and contract experiments are labeled separately so the code can be reviewed in context.
