# Ivan Mudrik

Backend developer, PHP and Symfony. Six years commercial, four of them in fintech.

I work mostly on systems that already exist — payment integrations, legacy modernization, and the unglamorous business of changing a product while it stays online. What I'm best at is reading a domain: working out from a running monolith how the business actually behaves, then designing a clean model for it.

### Recent work

**E-commerce platform** — Developing and optimizing a Yii2 monolith in production while building its Symfony 8 replacement alongside it, so the live product keeps moving forward during the migration. Cut SQL queries on the product catalogue page from 600 to 30 by eliminating N+1 in Yii2 ActiveRecord, working from cachegrind profiles captured with Xdebug. Upgraded the platform from PHP 8.4 to 8.5. For the migration, designed the Doctrine model from scratch — derived from the business domain rather than ported from the ActiveRecord models — and a GraphQL schema as the API contract, so the frontend could start on Vue in parallel. Built search on Elasticsearch, and worked on the existing REST integration with 1C, debugging sync failures and data mismatches.

**Online banking platform** (4 years) — CodeIgniter 3 on PHP 7/8, a large legacy monolith. Integrated partner banks and payment providers — LHV Bank, IFX Payments, ViolaMoney, RippleNet — including ISO 20022 messaging with LHV Connect: pain.001 payment initiation, pain.002 status reports, camt.053 statements, camt.054 debit and credit notifications, plus reconciliation of card transactions against our own ledger. Most of the domain's difficulty lives in payment status handling, where a status arrives before the payment is committed, or twice, or never — so it was built for idempotency and eventual consistency. Maintained the platform's own API for wallet and payment operations. Led a team of four developers for six months. Found and closed a stored XSS in the view layer.

**Crypto crowdfunding platform** — Symfony with Doctrine, Twig and RabbitMQ on the backend; Vue.js and TypeScript on the frontend. Docker for local environments, GitLab CI, PHPUnit, and static analysis with PHPStan and Psalm. Half new features; the other half I proposed myself — an audit that found and fixed XSS, added CSRF tokens to close a route to unauthorised transactions, moved state-changing endpoints off GET, and put Content Security Policy and Subresource Integrity in place. Picked out of 50+ engineers to review other developers' code.

### Side project

**[titanium_flapdoodle](https://github.com/randomsymbols/titanium_flapdoodle)** — Asynchronous media analysis pipeline. Symfony 8 with Messenger, a separate FastAPI service behind a detector abstraction, Vue 3 on Vite, composed in Docker. Built with Claude Code; the commit history shows how the work was decomposed into phases.

### Stack

`PHP 8` `Symfony` `Doctrine` `Yii2` `CodeIgniter` `MySQL` `PostgreSQL` `MongoDB` `Redis` `Elasticsearch` `RabbitMQ` `GraphQL` `REST` `ISO 20022` `SEPA` `XML` `Docker` `PHPUnit` `PHPStan` `Psalm` `Vue.js` `Twig` `JavaScript` `TypeScript`

### Also

English at C2. Eight SymfonyCasts certifications in 2025, including Dependency Injection Attributes, Doctrine & the Database, Go Pro with Doctrine Queries, and API Platform 3.

### Contact

randomsymbols@protonmail.com · [LinkedIn](https://www.linkedin.com/in/ivanmudrik/) · Remote, UTC+3
