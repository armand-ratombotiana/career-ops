# Article & Proof Points Digest — Armand Judicael RATOMBOTIANA

<!-- ============================================================
     This file contains detailed proof points, project write-ups,
     and case study metrics. The evaluation system reads this file
     to find specific numbers and stories to use in CVs and applications.
     
     Source: RATOMBOTIANA_ARMAND_JUDICAEL.pdf (extracted 2026-04-11)
     ============================================================ -->

---

## Case Study 1: Incident Management System Migration — Ambatovy

**Company:** Ambatovy Joint-Venture (Nickel/Cobalt mining, ~6,000 employees)
**Role:** Full-Stack Java Developer
**Timeline:** Oct 2022 – Present

### Problem
The legacy Incident Management System ran on a monolithic Java EE stack on GlassFish. P2+ alerts (production incidents affecting mining operations) had slow resolution routing — averaging several hours from detection to the right team.

### Solution
Migrated the IMS to Spring Boot 3, redesigned the alert routing engine, and built a new Angular 15+ dashboard with real-time status updates via WebSocket.

### Result
- **P2+ alert resolution time dropped 65%**
- Deployment process standardized with Docker + Jenkins pipeline
- System now serves ~200 IT staff across the mine site 24/7

### Hero Quote
> "After the migration, our P2+ alert response time dropped 65%. For a mining operation that never stops, that's the difference between a contained incident and a production shutdown."

---

## Case Study 2: IT Asset Inventory System — Ambatovy

**Company:** Ambatovy Joint-Venture
**Role:** Full-Stack Java Developer

### Problem
IT assets (6,000+ physical items: laptops, servers, networking equipment) were tracked in spreadsheets. A lookup could take hours as staff cross-referenced multiple sheets to find which department had which equipment.

### Solution
Built Asset Inventory from scratch: Java EE backend with barcode scanning integration, PostgreSQL database, RESTful API, and Angular 15+ self-service frontend.

### Result
- **Lookup time: half a day → < 3 seconds**
- Reduced IT ticket volume by 40% (staff self-serve instead of emailing IT)
- 6,000+ assets now tracked with full audit trail

### Hero Quote
> "We went from half a day of spreadsheet archaeology to a 3-second barcode scan. The IT team recovered 2+ hours per day they'd been spending on asset queries."

---

## Case Study 3: Spring Batch ETL — Oracle to PostgreSQL — Ambatovy

**Company:** Ambatovy Joint-Venture
**Role:** Full-Stack Java Developer

### Problem
Oracle 19C → PostgreSQL migration required moving years of operational data (historical incidents, asset records, canteen orders) without data loss during cutover.

### Solution
Implemented a multi-phase Spring Batch ETL pipeline with checkpointing, retry logic, and data-quality validation at each step.

### Result
- **99.97% data reliability at 50,000 rows/batch**
- Zero rollback required at cutover
- Full audit log for compliance with operational data governance requirements

---

## Case Study 4: Real-Time Canteen Platform — Ambatovy

**Company:** Ambatovy Joint-Venture
**Role:** Full-Stack Java Developer

### Problem
The mine canteen serving ~1,500+ workers daily was managed manually. Order errors, queue management, and reporting were done by hand.

### Solution
Built a real-time ordering platform: Spring Boot 3 REST backend, React 18 frontend for kitchen and cashier stations, WebSocket for live order streaming.

### Result
- **200+ daily orders with zero data loss**
- Eliminated manual order tracking errors
- Kitchen throughput improved via real-time queue display

---

## Case Study 5: Multi-Tenant SaaS CRM — DDS.mg

**Company:** DDS.mg
**Role:** Full-Stack Java Developer
**Timeline:** 2020 – 2022

### Problem
DDS.mg needed a CRM for multiple clients with strict data isolation. Starting from zero with a small team and a 4-month deadline before funding review.

### Solution
Architected multi-tenant SaaS CRM from scratch using Spring Boot 3, PostgreSQL row-level security for tenant isolation, JWT/OAuth2 auth, React 18 frontend.

### Result
- **MVP delivered in 4 months**
- **Zero data-isolation incidents** across all tenants in production
- Secured next funding tranche on the demo

### Hero Quote
> "4 months from whiteboard to live SaaS with multiple paying tenants and zero isolation incidents. That's the pace I work at when the deadline is real."

---

## Case Study 6: Monolith → Microservices Migration — DDS.mg

**Company:** DDS.mg
**Role:** Full-Stack Java Developer

### Problem
Legacy monolith had grown to the point where a single deployment took 45 minutes, test coverage was near zero, and every release was a risk event.

### Solution
Led phased migration to Spring Boot 3 / Java 17 microservices with Docker-based deployments. Introduced JUnit 5, Mockito, and Testcontainers for automated testing.

### Result
- **Deployment time: 45 minutes → 8 minutes**
- **Test coverage: ~0% → 75%**
- Release cadence improved from monthly to weekly

---

## Case Study 7: AI Code Quality Review — Outlier AI / Scale AI

**Company:** Outlier AI / Scale AI (contract)
**Role:** Java Consultant — Code Quality
**Timeline:** Feb 2024 – Feb 2025

### Problem
LLM providers needed expert Java engineers to review AI-generated code samples for correctness, idiomatic usage, and migration accuracy (Java EE → Jakarta EE 10).

### Result
- Reviewed **600+ AI-generated Java samples**
- Provided structured feedback on correctness, style, and EE → Jakarta EE migration patterns
- Unique insight: where GPT-class models get Java right and wrong (injection, lifecycle, persistence contexts)

### Talking Point
> "Having reviewed 600+ AI-generated Java samples for Scale AI, I know exactly where LLMs hallucinate in enterprise Java — dependency injection lifecycle, persistence context boundaries, Jakarta EE namespace migration. That lens makes me a sharper reviewer of AI-assisted code."

---

## Project: JNoSQL-EMBED (Open Source)

**URL:** https://github.com/armand-ratombotiana
**Stack:** Java 17+, Eclipse JNoSQL, embedded storage engine

### What It Does
Embedded NoSQL engine for the JVM following the Eclipse JNoSQL API standard. Enables in-process NoSQL storage for testing, edge computing, and offline scenarios — no external NoSQL server required.

### Key Metric
- **+40% throughput improvement** vs. remote NoSQL baseline in benchmarked read/write scenarios
- Contributed to Eclipse JNoSQL ecosystem; demonstrates deep JVM and storage internals knowledge

---

## Project: TalentPilotAI

**Stack:** Spring Boot 3, GPT-4o (OpenAI API), PostgreSQL, React 18

### What It Does
End-to-end AI-powered hiring automation: ingests CVs, scores candidates against job requirements using GPT-4o function calling, generates structured interview question sets.

### Talking Point
> "TalentPilotAI was my way of eating my own dog food — I built the kind of tool that evaluates candidates like me. It parses CVs, runs scoring against JD requirements via GPT-4o, and outputs structured interview prep. Full Spring Boot 3 backend, React 18 frontend."

---

## Project: Hybrid 3D Chess Engine

**Stack:** Java 21, OpenGL (LWJGL), GPU compute

### Key Metric
- **4x speed improvement** on move generation via GPU path vs. pure CPU baseline
- Demonstrates advanced JVM + native interop (LWJGL/JNI) and performance engineering mindset

---

## Languages & Communication

- **French** — Native (can target francophone job markets: France, Belgium, Switzerland, Quebec, Madagascar)
- **English** — C1 / Professional (all technical writing, documentation, code reviews)
- **Public speaking** — Toastmasters International member (structured presentation, impromptu speaking)

---

## Character Proof Points

- **BJJ Blue Belt** — Discipline, resilience, comfort with discomfort. Not just a hobby: BJJ blue belt takes 1–3 years of consistent training.
- **Toastmasters** — Active investment in communication skills beyond just technical work.
- **Open Source** — JNoSQL-EMBED shows initiative beyond paid work; ecosystem citizenship.
