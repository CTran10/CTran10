<h1 align="center">Hi 👋, I'm Calvin Tran</h1>
<h3 align="center">Software Engineer · Backend, AI Infrastructure, Product</h3>

<p align="left">
  <img src="https://komarev.com/ghpvc/?username=ctran10&label=Profile%20views&color=0e75b6&style=flat" alt="profile views" />
</p>

---

- 🛠️ I build production **Django** and **FastAPI** systems on **PostgreSQL** and **TypeScript**.
- 🏍️ I build portfolio-grade systems on the side: **Apex** (security-first rider setup logbook + community), **Clearance** (event-driven payment authorization in Go), and **Properly** (landlord operations),.
- 🎓 B.S. Computer Science, **Colorado School of Mines**, 2026.
- 💬 Ask me about FastAPI, PostgreSQL and RLS, event-driven systems, LLM evaluation, and backend performance.
- 📫 Reach me at **calvintran1027@gmail.com**.

---

<h3 align="left">Connect</h3>
<p align="left">
  <a href="https://linkedin.com/in/calvintran-tech" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:calvintran1027@gmail.com" target="_blank">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
</p>

---

<h3 align="left">Languages and Tools</h3>
<p align="left">
  <a href="https://www.python.org" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/></a>
  <a href="https://www.typescriptlang.org/" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg" alt="typescript" width="40" height="40"/></a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/></a>
  <a href="https://www.w3schools.com/sql/" target="_blank"><img src="https://www.svgrepo.com/show/331760/sql-database-generic.svg" alt="sql" width="40" height="40"/></a>
  <a href="https://fastapi.tiangolo.com/" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/fastapi/fastapi-original.svg" alt="fastapi" width="40" height="40"/></a>
  <a href="https://www.djangoproject.com/" target="_blank"><img src="https://cdn.worldvectorlogo.com/logos/django.svg" alt="django" width="40" height="40"/></a>
  <a href="https://go.dev/" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/go/go-original.svg" alt="go" width="40" height="40"/></a>
  <a href="https://www.postgresql.org" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original.svg" alt="postgresql" width="40" height="40"/></a>
  <a href="https://www.sqlalchemy.org/" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/sqlalchemy/sqlalchemy-original.svg" alt="sqlalchemy" width="40" height="40"/></a>
  <a href="https://nextjs.org/" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nextjs/nextjs-original.svg" alt="nextjs" width="40" height="40"/></a>
  <a href="https://reactjs.org/" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="40" height="40"/></a>
  <a href="https://svelte.dev" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/svelte/svelte-original.svg" alt="svelte" width="40" height="40"/></a>
  <a href="https://supabase.com/" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/supabase/supabase-original.svg" alt="supabase" width="40" height="40"/></a>
  <a href="https://www.docker.com/" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="docker" width="40" height="40"/></a>
  <a href="https://openai.com/" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/openai/openai-original.svg" alt="openai" width="40" height="40"/></a>
  <a href="https://git-scm.com/" target="_blank"><img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/></a>
</p>

---

<h3 align="left">🚀 Featured Work</h3>

**LLM Evaluation Platform** _(Breef)_
<br/><sub>Python, PostgreSQL, OpenAI API</sub>

I build AI features and own the evaluation service that keeps them reliable in production.

- Built **PostgreSQL-backed pipelines for LLM production sampling, review tracking, and evaluation workflows**, so model behavior is measured against real traffic.
- Shipped **OpenAI API integrations** that automate internal operational workflows and cut manual review overhead.
- Diagnosed and fixed **framework-level cached-token accounting** that would have overstated operational AI cost by about **6x**.
- The result: I can build the AI tooling and the harness that validates correctness, cost, and regressions before they reach users.

<br/>

**[Apex: Rider Setup Vault](https://github.com/CTran10/Apex)**
<br/><sub>FastAPI, Next.js, PostgreSQL, Supabase, TypeScript, Docker</sub>

A security-first, full-stack setup logbook and community platform for motorcycle track riders — the rider loop runs end to end and now layers a privacy-conscious social tier on top.

- **Database-enforced authorization:** Postgres Row-Level Security (SECURITY INVOKER), per-request JWT, and a quarantined `service_role` that never touches the user request path.
- **Immutable history model:** copy-on-write session snapshots and database-controlled adjustment state transitions, so historical records never resolve through live bike state.
- **Community without leakage:** opt-in session sharing, a track-scoped shared feed, kudos/comments, rider follows, public rider profiles, and exact-filter search — shared sessions stay readable without exposing anyone's private logbook.
- **175+ automated tests** with full CI (pytest on real Postgres, Ruff, mypy, pip-audit) plus a cross-account IDOR/RLS suite, enforced through local Git hooks and a pre-push CI gate.

<br/>

**[Clearance: Event-Driven Authorization](https://github.com/CTran10/clearance)**
<br/><sub>Go, PostgreSQL, Redis, Redpanda (Kafka), Docker Compose</sub>

A Go transaction-authorization platform built to explore the reliability patterns that appear once a system goes asynchronous — transactions flow through ingestion, risk evaluation, and immutable ledger recording across four focused services.

- **Transactional outbox:** transaction, idempotency key, and event are written in one DB transaction, then published by a poller using `FOR UPDATE SKIP LOCKED` — no "DB committed but publish failed" gap.
- **Reliability primitives:** idempotency keys with payload-conflict detection, automatic retries with dead-letter handling, correlation-ID propagation, and an immutable double-entry ledger with explicit DB constraints.
- **Trust boundaries taken seriously:** bearer auth with constant-time comparison, request-size limits, strict validation, parameterized SQL, CORS allowlists, and Redis-backed rate limiting.
- **Tested where it matters:** `go test ./...` covers idempotency, outbox/retry/DLQ behavior, ledger writes, and auth paths, with CI validating tests, `go vet`, and the Compose stack.

<br/>

**[Properly: Landlord Operations](https://github.com/CTran10/Properly)**
<br/><sub>FastAPI, Next.js App Router, PostgreSQL (RLS), Supabase, Cloudflare R2, TypeScript</sub>

A multi-tenant landlord operations app for tracking properties, units, expenses, vendors, photos, and tax-season exports — built in vertical slices so each shipped feature has API, UI, tenancy, validation, and tests.

- **Tenant isolation by default:** account-scoped data with Postgres RLS policies, Supabase-issued JWTs verified by the API via JWKS, and tenant-scoped request context.
- **Money done right:** integer-cents accounting across a vendors/expenses ledger with filtering, soft deletes, yearly category totals, and read-only accountant access.
- **Secure file handling:** private Cloudflare R2 presigned upload/download with checksum and magic-byte verification on property photos.
- **Layered quality gate:** Vitest, ESLint, Stylelint, pytest, Ruff, and mypy wired into GitHub Actions CI for both frontend and backend.

---

<h3 align="left">📸 When I'm not shipping code</h3>

<table>
  <tr>
    <td width="33%"><img src="images/track.jpg" alt="At the track" width="100%" /></td>
    <td width="33%"><img src="images/ski.jpg" alt="Skiing" width="100%" /></td>
    <td width="33%"><img src="images/golf.jpg" alt="Golf" width="100%" /></td>
  </tr>
  <tr>
    <td align="center">🏍️ Night Rides</td>
    <td align="center">⛷️ Skiing Breckenridge</td>
    <td align="center">⛳ Playing 18</td>
  </tr>
</table>

