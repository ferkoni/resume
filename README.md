# Fernando Konishi
**Senior Full Stack Engineer**

Encarnación, Paraguay | ferkoni@gmail.com
[GitHub](https://github.com/ferkoni) | [LinkedIn](https://www.linkedin.com/in/fernando-konishi-5abb01114)

## Summary
Senior Full Stack Engineer with 11+ years building backend systems and third-party integrations, including 8 years at a B2B SaaS startup that grew from early-stage to an established platform. Most of that work replaced a step an engineer had to do with a setting a non-engineer could change: billing providers, client integrations, report routing, client onboarding. Also multi-tenant architecture, integration layers against systems that do not follow the standard, billing, data pipelines on AWS, and background jobs that report when they die. 8 years of EmberJS, and React on a personal project.

---

## Experience

### **Ovation** *(B2B SaaS platform for clinical genomics laboratories)* | Senior Full Stack Engineer
*November 2021 - March 2026*

* Replaced a hardcoded single-vendor billing integration with a provider-agnostic adapter architecture, so customer success could select the billing provider and configure per-client field mappings (patient, physician, test type) without engineering involvement.
* Replaced a third-party document generation vendor with an in-house AWS Lambda pipeline rendering per-tenant HTML templates to PDF, cutting vendor costs while giving dozens of enterprise clients full control of branding and layout: logos, colors, structure, and content.
* Built an integration layer from scratch for ~10 enterprise clients, with a canonical schema and a configurable JSON mapping layer that absorbed each client's non-standard implementation of the HL7 healthcare messaging standard. It moved orders, results and billing messages over S3 with per-client file format definitions and per-project bucket routing, replacing manual CSV imports and one-off API calls, and turned new client onboarding into a configuration task rather than an engineering project.
* Built an integration event log view for non-engineering users, unifying records spread across four tables into a single normalized feed with filtering and pagination, using SQL views and UNION queries to present one consistent format across every integration feature.
* Maintained a signature-verified inbound webhook endpoint receiving result-ready callbacks from external analysis vendors, and made the handler idempotent after spotting a vendor redelivering identical payloads in the event feed above, which the endpoint had been processing as distinct events.
* Built a heartbeat and reaper mechanism for long-running background jobs that were dying silently without status updates or logs: each job writes a timestamp to a Redis key on a timer thread, and a recurring sweeper flags jobs whose heartbeat has gone stale, posts them to Slack, and clears their database locks so the work becomes retryable.
* Migrated ~40 background job workers from RabbitMQ to SQS, adapting each job class and its RSpec unit tests to the new message structure, improving operational visibility across the queue.
* Shipped every feature with RSpec coverage, including regression specs for each bug fix, and used request and integration specs to lock in behavior across the configurable mapping and routing layers before customer success touched them.
* Informally led onboarding for 7 engineers over two years through pairing, code reviews, and breaking down implementation approaches, and remained the go-to resource for architecture and debugging questions across the team.
* **Tools:** Ruby on Rails, RSpec, EmberJS, Python, SCSS, MySQL, Redis, RabbitMQ, AWS S3, AWS Lambda, AWS SQS, Docker.

### **Ovation** *(B2B SaaS platform for clinical genomics laboratories)* | Full Stack Engineer
*April 2018 - November 2021*

* Replaced an engineer-configured report routing system with a workflow customer success could configure themselves, integrating three external analysis vendors and routing report generation per project and test type across 20+ enterprise clients.
* Built a JSON export/import pipeline that promoted validated client configurations from staging to production, serializing deeply nested records across 10+ tables while preserving referential integrity. It replaced a manual, error-prone process that had required an engineer at every client onboarding, and was covered end to end by RSpec specs over the full nested fixture set.
* **Tools:** Ruby on Rails, RSpec, EmberJS, SCSS, MySQL, AWS S3.

### **Inspira** *(enterprise management software for hospitals)* | Full Stack Engineer
*May 2016 - April 2018*

* Built an access control system from the ground up, scoping work order visibility by work area across hundreds of users in clinical, administrative, and accounting roles.
* Built an accounting and billing transaction history system from scratch, handling thousands of transactions per week for the accounting team.
* **Tools:** Ruby on Rails, Minitest, JQuery, SCSS, PostgreSQL, Heroku.

### **Earlier roles** | Software Developer
*October 2013 - May 2016*

* JSP scripts for large customer data maintenance and corrections at Power Steering (Java, JSP); REST API service for an Android "walk tracker" application at IMoti (Ruby on Rails, PostgreSQL); a game-like English pronunciation application at PronounceApp (Ruby on Rails, PostgreSQL).

## Projects

### **Practice Management SaaS** *(multi-tenant product for clinics)* | Co-founder and Engineer
*October 2019 - November 2025*

* Co-founded and built a multi-tenant practice management product with one other engineer, a Rails JSON API with an EmberJS client, sold under contract to a non-profit physical therapy provider and delivered against payment milestones, then extended for three more years with an inventory module and a fiscal invoicing layer. Still running in production, where around 15 staff use it daily to run about 500 appointments a week.
* Gathered requirements directly from the director, therapists and front desk staff, ran the demo that released a contract payment milestone, and supported the system in production afterwards.
* Owned the authorization layer, with a permission model and request-aware Pundit policies, plus a generic reporting engine with typed cells and row and column totals, the CSV export subsystem, and a fiscal invoicing module for Paraguayan tax compliance.
* Built a configurable form builder that let each organization define its own record templates, sections, fields, input types and validation rules, so adapting the product to a new organization was configuration rather than development.
* Owned deployment for the life of the product, configuring the API's database and backups on Heroku, and moved the frontend to DigitalOcean once the Ember build's peak memory grew past what Heroku allowed and started killing deploys.
* **Tools:** Ruby on Rails, RSpec, EmberJS, PostgreSQL, Pundit, Heroku, DigitalOcean, AWS S3.

### **Photo Gallery App** *(self-hosted photo management system)* | Personal Project
*In progress* | [github.com/ferkoni/gallery](https://github.com/ferkoni/gallery)

* Built JWT authentication with per-session revocation, image uploads to S3 with presigned URLs, async album download via background jobs with WebSocket notification, and full-text search with pagination.
* Built with Claude Code on a written-down agent workflow: custom skills for research, planning and TDD plus a project-level `CLAUDE.md`, with work planned up front as fixed constraints, open decisions, and small spikes to settle the risky parts first.
* **Tools:** React 19, TypeScript, Vitest, Ruby on Rails 8.1, PostgreSQL, AWS S3, Claude Code.

---

## Education

* **Computer Science Engineering** | National University of Itapúa - Graduated November 2021
  *Completed while working full-time as a Software Engineer*

---

## Languages

* **Spanish:** Native/Bilingual
* **English:** Full Professional Proficiency
