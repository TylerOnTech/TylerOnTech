<a href="https://tylerontech.github.io"><img src="https://tylerontech.github.io/assets/img/og.png" alt="Tyler Kunkel: I build real products, from the database up." width="100%"></a>

# Hi, I'm Tyler 👋

Founder of **TyKu Technologies** and co-founder of **Black Box Fragrances**. I design, build, and ship
full-stack SaaS, from multi-tenant database design all the way to the interface.

🌐 **Portfolio:** [tylerontech.github.io](https://tylerontech.github.io)<br>
🔭 **Now:** shipping BindHQ V2: policies, vehicles, drivers, and documents.<br>
📍 Fort Wayne, Indiana

## 🚀 Featured work

### [CarrierBridge](https://github.com/TylerOnTech/CarrierBridge) · Integration engine

Pulls insurance policies from carriers that each work differently (a modern OAuth REST API, a legacy
XML-bridged service, and a portal only a headless browser can read) and normalizes them into one
versioned `NormalizedPolicy` contract behind an async API. It runs on a Postgres task queue with leases
and fencing tokens, isolates partial failures, retries at two layers, and encrypts credentials while they
wait. Backed by 164 tests.

`TypeScript` `Node.js 22` `Express 5` `PostgreSQL 16` `Prisma` `Zod` `Playwright` `Vitest` `Docker Compose`

[Code](https://github.com/TylerOnTech/CarrierBridge) · [Design decisions](https://github.com/TylerOnTech/CarrierBridge/blob/main/docs/design-decisions.md) · [Case study](https://tylerontech.github.io/#work)

### [CarrierChaos](https://github.com/TylerOnTech/CarrierChaos) · Reliability engine

Retrieves insurance policy data correctly even when carrier APIs are slow, rate-limited, flaky, down,
or wrong. Concurrent jobs run against mock carriers that fail on purpose, and the infrastructure
responds with per-carrier queues, circuit breakers, Redis rate limits, bounded retries that honor
`Retry-After`, hard timeouts, dead-letter replay, and fenced effectively-once results. Backed by 198
tests, four reproducible experiments, and a 1,000-job load test.

`TypeScript` `Node.js 22` `Express 5` `BullMQ` `Redis` `PostgreSQL` `Prisma 7` `Zod` `Prometheus` `Vitest`

[Code](https://github.com/TylerOnTech/CarrierChaos) · [Experiment results](https://github.com/TylerOnTech/CarrierChaos/blob/main/docs/results/EXPERIMENTS.md) · [Case study](https://tylerontech.github.io/#work)

### [PolicyWatch](https://github.com/TylerOnTech/PolicyWatch) · Event-driven monitoring

Polls carrier APIs in three different formats (camelCase JSON, snake_case JSON, ACORD-style XML),
normalizes them into one contract, detects meaningful policy changes (cancellations, renewals, premium
and coverage changes, vehicles added or removed), and delivers HMAC-signed webhooks with retries, a
transactional outbox, SSRF protection, and a full audit trail. Includes Terraform and Ansible for a
locked-down AWS environment. Backed by 135+ tests.

`TypeScript` `Node.js 22` `Express 5` `PostgreSQL 17` `Prisma` `Redis` `BullMQ` `Terraform` `Ansible` `AWS`

[Code](https://github.com/TylerOnTech/PolicyWatch) · [Architecture](https://github.com/TylerOnTech/PolicyWatch/blob/main/docs/architecture.md) · [Case study](https://tylerontech.github.io/#work)

### BindHQ · TyKu Technologies

An agency management system and CRM for independent insurance agencies. It's a true multi-tenant SaaS,
with tenant isolation enforced in the database by forced Postgres row-level security. V1 is live in
production and V2 is in progress.

`Next.js 16` `React 19` `TypeScript` `PostgreSQL` `Drizzle ORM` `Better Auth` `Tailwind` `Vercel`

[Live app](https://bindhq.vercel.app) · [Case study](https://tylerontech.github.io/#work) · Private repo, code walkthrough on request

### Black Box Fragrances · Black Box Media

A personal fragrance decision engine built for an audience of 70,000+. A three-minute taste quiz builds
your Scent Profile, then every fragrance gets an explainable Match Score and a Bottle Check verdict that
knows what's already in your collection. Backed by ~880 automated tests.

`Next.js 16` `React 19` `TypeScript` `PostgreSQL` `Drizzle ORM` `Playwright` `PostHog` `Vercel`

[blackboxfragrances.com](https://www.blackboxfragrances.com) · [Case study](https://tylerontech.github.io/#work) · Private repo, code walkthrough on request

## 🧰 More projects

- **[Password Analyzer](https://github.com/TylerOnTech/Password_Analyzer)**: a Python CLI that rates
  password strength using entropy estimates and pattern detection, tested with pytest.
- **[CLI Task Manager](https://github.com/TylerOnTech/CLI_Task_Manager)**: an interactive Python task
  manager with JSON persistence, built on the standard library alone.

## 🤳 Connect with me

[Portfolio](https://tylerontech.github.io) · [LinkedIn](https://linkedin.com/in/tjkunkel) · [YouTube](https://www.youtube.com/@TylerOnTech) · [Instagram](https://www.instagram.com/really_low/) · [Email](mailto:tkunkel1629@gmail.com)
