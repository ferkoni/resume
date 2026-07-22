# Fernando Konishi
**Senior Full Stack Engineer**

Encarnación, Paraguay | ferkoni@gmail.com
[GitHub](https://github.com/ferkoni) | [LinkedIn](https://www.linkedin.com/in/fernando-konishi-5abb01114)

## Summary
Senior Full Stack Engineer with 11+ years building backend systems and third-party integrations, including 8 years at a B2B SaaS startup that grew from early-stage to an established platform. Specialised in turning engineer-dependent workflows into self-serve systems: configurable by non-engineers, operable without engineering involvement. Experience spans multi-tenant architecture, integration layers against non-standard external systems, billing, and data pipelines on AWS. Currently expanding frontend depth into React after 8 years of EmberJS.

---

## Experience

### **Ovation** *(B2B SaaS platform for clinical genomics laboratories)* | Senior Full Stack Engineer
*2021 — 2026*

* Replaced a hardcoded single-vendor billing integration with a provider-agnostic adapter architecture, so customer success could select the billing provider and configure per-client field mappings (patient, physician, test type) without engineering involvement.
* Replaced a third-party document generation vendor with an in-house AWS Lambda pipeline rendering per-tenant HTML templates to PDF, cutting vendor costs while giving dozens of enterprise clients full control of branding and layout: logos, colors, structure, and content.
* Built an automated S3-based bulk data exchange pipeline for ~10 enterprise clients, replacing manual CSV imports and one-off API calls, with per-client file format definitions and per-project bucket routing configurable by customer success.
* Built an integration layer from scratch for ~10 enterprise clients, with a canonical schema and a configurable JSON mapping layer that absorbed each client's non-standard implementation of the HL7 healthcare messaging standard, turning new client onboarding into a configuration task rather than an engineering project.
* Migrated ~40 background job workers from RabbitMQ to SQS, adapting each job class and its unit tests to the new message structure, improving operational visibility across the queue.
* Informally led onboarding for 7 engineers over two years through pairing, code reviews, and breaking down implementation approaches, and remained the go-to resource for architecture and debugging questions across the team.
* **Tools:** Ruby on Rails, EmberJS, Python, SCSS, MySQL, AWS S3, AWS Lambda, Docker.

### **Ovation** *(B2B SaaS platform for clinical genomics laboratories)* | Full Stack Engineer
*2018 — 2021*

* Replaced an engineer-configured report routing system with a workflow customer success could configure themselves, integrating three external analysis vendors and routing report generation per project and test type across 20+ enterprise clients.
* Built a JSON export/import pipeline that promoted validated client configurations from staging to production, serializing deeply nested records across 10+ tables while preserving referential integrity, and replacing an error-prone manual process that previously required an engineer at every client onboarding.
* **Tools:** Ruby on Rails, EmberJS, SCSS, MySQL, AWS S3.

### **Inspira** *(enterprise management software for hospitals)* | Full Stack Engineer
*2016 — 2018*

* Built an access control system from the ground up, scoping work order visibility by work area across hundreds of users in clinical, administrative, and accounting roles.
* Built an accounting and billing transaction history system from scratch, handling thousands of transactions per week for the accounting team.
* **Tools:** Ruby on Rails, JQuery, SCSS, PostgreSQL, Heroku.

### **Power Steering** | Software Developer
*2016*

* Developed JSP scripts for large customer data maintenance and corrections.
* **Tools:** Java, JSP.

### **IMoti** | Software Developer
*2015*

* Developed REST API service for Android "walk tracker" application.
* **Tools:** Ruby on Rails, Heroku, PostgreSQL.

### **PronounceApp** | Software Developer
*2013 — 2014*

* Designed and developed a game-like application for English pronunciation improvement.
* **Tools:** Ruby on Rails, Heroku, PostgreSQL.

## Projects

**Photo Gallery App** | React 19, TypeScript, Ruby on Rails 8.1, PostgreSQL, AWS S3 — (https://github.com/ferkoni/gallery)
*In progress*
Self-hosted photo management system: JWT authentication with per-session revocation, image uploads to S3 with presigned URLs, async album download via background jobs with WebSocket notification, full-text search and pagination.

---

## Education

* **Computer Science Engineering** | National University of Itapúa — Graduated 2021
  *Completed while working full-time as a Software Engineer*

---

## Languages

* **Spanish:** Native/Bilingual
* **English:** Full Professional Proficiency
