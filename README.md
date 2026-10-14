# Sayed MD. Fahim Fahad

**Senior Backend Engineer · Java, Spring Boot & AWS · Payments and high-volume data systems**

<div align="center">

<img src="/Fahim%20Fahad.png" alt="Fahim Fahad" width="320" height="240" style="border-radius: 12px; object-fit: cover;" />

<br/><br/>

[![Toptal](https://img.shields.io/badge/Toptal-Top%203%25%20Talent-3863A0?style=flat-square&logo=toptal&logoColor=white)](https://www.toptal.com/resume/fahim-fahad)
[![Java & Spring Boot](https://img.shields.io/badge/Java%20%26%20Spring%20Boot-10%2B%20Years-ED8B00?style=flat-square&logo=openjdk&logoColor=white)](#)
[![AWS](https://img.shields.io/badge/AWS-5%2B%20Years-FF9900?style=flat-square&logo=amazonaws&logoColor=white)](#)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-000000?style=flat-square&logo=vercel&logoColor=white)](https://portfolio-three-snowy-36.vercel.app)

</div>

---

## About Me

- ☕ **Java & Spring Boot** engineer, 10+ years building backend systems, from first commit to production
- 💳 **Payments**: built the core financial engine of a central-bank-licensed payments platform; certified card gateway integration (CIT/MIT, tokenisation)
- ☁️ **AWS-focused**: ECS, Lambda, SQS, S3, EventBridge, ElastiCache and more, 5+ years in production
- 🤖 **LLM features in production**: streaming tool-use agent on the Anthropic API, with cost tracked per conversation
- 🚀 **Startup veteran**: founding engineer at a fintech, built several products from scratch
- 🐞 Strong in **production debugging**, query tuning and load testing
- 🌍 **Toptal** freelancer since 2021, working with US product teams
- 🎓 **MSc & BSc, 1st Position**, Jahangirnagar University · published in **IEEE** and **IJCIT**

---

## Selected Work

Production systems I designed or owned. Client code is private, so this is what was built and what it changed.

| Project | What it was | Scale / outcome |
|---|---|---|
| **Core Financial Engine** | System of record for money at a licensed digital payments platform, built from scratch | Zero to central-bank licensing and commercial launch |
| **AI Property Search Assistant** | Streaming LLM agent for natural-language property search | **60%** lower cost per conversation |
| **Card Payment Gateway Integration** | CIT and MIT card processing with tokenisation, through vendor certification | **50,000+** paying users |
| **Bulk Listing Search API** | Sync and async search with deduplication and atomic job claiming | **Billions** of property records |
| **Notification Service** | Owned the service after extraction from the monolith; designed types and ran experiments | **+5%** DAU, **150k** peak daily |

<details>
<summary><b>Core Financial Engine</b> · digital payments platform licensed as a PSP by Bangladesh Bank</summary>
<br/>

- Joined before the first commit and built the system of record for every movement of money on the platform
- Transaction processing, balance management, end-of-day merchant reconciliation and financial reporting
- Ran regular load tests and migrated the database to optimise the payment flow
- Platform reached 50k registered users and commercial launch during my time there

`Java` `Spring Boot` `Oracle` `Microservices`
</details>

<details>
<summary><b>AI Property Search Assistant</b> · natural-language property search for a US real-estate data platform</summary>
<br/>

- Designed and built the server side: a streaming tool-use agent on the Anthropic API
- Filter taxonomy sourced from S3, so search categories change without a redeploy
- Prompt caching cut cost per conversation by 60%
- Per-conversation logging of tokens, cache hits and cost, so spend is tracked rather than estimated

`Java` `Spring Boot` `Anthropic API` `AWS S3` `PostgreSQL`
</details>

<details>
<summary><b>Card Payment Gateway Integration</b> · subscription billing for 50,000+ paying users</summary>
<br/>

- Integrated a card gateway across two services, covering CIT and MIT with card tokenisation
- Took the integration through the vendor's certification process before production
- Request-trace IDs on every gateway payment log, so any charge can be followed by one identifier
- Alerting on recurring-billing job failures, so a failed nightly run surfaces immediately

`Java` `Spring Boot` `PostgreSQL` `Hibernate`
</details>

<details>
<summary><b>Bulk Listing Search API</b> · search over billions of property records for a sister company's platform</summary>
<br/>

- Two modes: small queries return inline, large ones become background jobs
- SHA-256 request hashing, so identical queries are recognised instead of re-run
- Atomic job claiming, so two workers can never pick up the same job
- Reads routed to a replica, keeping heavy search traffic off the primary

`Java` `Spring Boot` `PostgreSQL` `AWS`
</details>

<details>
<summary><b>Notification Service</b> · consumer platform with ~150k monthly active users</summary>
<br/>

- Became the owning engineer after the service was extracted from the core monolith
- Designed new notification types and ran Statsig experiments to measure whether they changed behaviour
- Targeted push drove a 5% increase in daily active users
- 20–30k notifications a day in steady state, peaking near 150k on event days

`Java` `Spring Boot` `MongoDB` `AWS` `OneSignal` `Statsig`
</details>

---

## Featured Repositories

| Repository | What it shows |
|---|---|
| [**secure-shop-platform**](https://github.com/fahimfahad92/secure-shop-platform) | OAuth2 / OIDC end to end: four Spring Boot services behind a gateway, Keycloak login, tokens never reach the browser |
| [**java-21-spring-boot-3-devops**](https://github.com/fahimfahad92/java-21-spring-boot-3-devops) | Container optimisation for Spring Boot: image cut from 739 MB to 220 MB (70%), plus CRaC, CDS and GitHub Actions CI |
| [**design-pattern**](https://github.com/fahimfahad92/design-pattern) | Classic design patterns implemented in a Spring Boot codebase, with class diagrams |
| [**portfolio**](https://github.com/fahimfahad92/portfolio) | Personal site on Next.js 16, React 19 and Tailwind · [live](https://portfolio-three-snowy-36.vercel.app) |

---

## Technical Skills

**Backend**
Java 8–21 · Spring Boot 2.6+ / 3.x · Spring Data JPA · Spring Security · JEE · Hibernate · GraphQL · REST

**Cloud (AWS)**
ECS · ECR · Lambda · SQS · S3 · EventBridge · CloudFront · API Gateway · ElastiCache · CloudWatch · Secrets Manager · Parameter Store · AppConfig · IAM · EKS · EC2

**Databases**
PostgreSQL · Oracle · MySQL · MongoDB · Elasticsearch · Redis

**Payments & Identity**
Card gateway integration · Tokenisation · CIT/MIT · Stripe · Third-party bank APIs · OAuth2 · OIDC · JWT · Keycloak

**AI / LLM**
Anthropic API · Tool use · Streaming · Prompt caching

**DevOps & Tools**
Docker · Terraform · Kubernetes · GitHub Actions · Maven · Gradle · Git

**Observability & Testing**
Datadog · New Relic · CloudWatch · ELK · JUnit · RestAssured · JMeter

**Messaging & Analytics**
Apache Kafka · SQS · EventBridge · Mixpanel · Statsig · OneSignal · SendGrid

**Frontend**
React · Next.js · TypeScript · Tailwind CSS · shadcn/ui · React Query

---

## Career

**Senior Software Engineer** · PropStream *(via Toptal)* · Oct 2025 – Present · Remote, USA
> US real-estate data platform. Lead feature delivery across teams of three to four engineers. Built the AI property-search assistant, bulk listing-search API and certified card gateway integration; delivered the direct-mail rebuild end to end; migrated 1.5 billion Do-Not-Call records onto a new data model.

**Frontend Developer** · PianoTrax *(via Toptal, part-time)* · Nov 2024 – Sep 2025 · Remote, USA
> Admin portal for an online sheet-music retailer. Rebuilt catalogue navigation on dynamic routing, merged blog editing into one form, built coupon management. Stack: Next.js, shadcn/ui, React Query.

**Backend Engineer** · GrowthDay *(via Toptal, then hired full-time)* · May 2021 – Jun 2024 · Remote, USA
> Personal-development platform, ~150k MAU. Owned the notification service (+5% DAU), goals and reminders; built the signup service from scratch. Upgraded Java 8→21 and Spring Boot 2→3. Cut dashboard load from 10s+ to 3–4s and support tickets by ~20%.

**Senior Software Engineer** · TigerIT Bangladesh Ltd. · Feb 2020 – Aug 2021 · Hybrid
> Designed the backend and led API development for Action Tracker, with an Elasticsearch search layer and newly introduced load testing. Built API and reporting for TigerHRMS (200+ employees).

**Software Engineer** · Dmoney Bangladesh Ltd. · May 2017 – Jan 2020 · On-site, Startup
> Founding engineer at a digital payments startup, from first commit through Bangladesh Bank PSP licensing and launch (50k users). Built the core financial engine, the bank and biller payment gateway, and the user management service.

**Software Engineer** · BJIT Ltd. · Jun 2016 – Apr 2017 · On-site

---

## Education & Research

**MSc in Computer Science & Engineering**
Jahangirnagar University · 2015–2016 · CGPA **3.95** · **1st Position**

**BSc in Computer Science & Engineering**
Jahangirnagar University · 2010–2014 · CGPA **3.79** · **1st Position**

**Publications**
- [Reform Based Version Management System for XML Data](https://www.ijcit.com/archives/volume3/issue6/Paper030618.pdf), *IJCIT, Nov 2014*
- [Cloud-Based Solution for Improvement of Response Time of MySQL RDBMS](http://ieeexplore.ieee.org/document/7860329/), *IEEE IWCI, Dec 2016*

---

## Recent Blog Posts

<!-- BLOG-POST-LIST:START -->
- [Statsig integration with Spring Boot](https://medium.com/spring-boot/statsig-integration-with-spring-boot-75cc91a68952?source=rss-fd28ce5a235e------2)
- [How to Integrate Spring Boot 3 with Aws Secret Manager and Parameter Store Using AWS SDK v2](https://awstip.com/how-to-integrate-spring-boot-3-with-aws-secret-manager-and-parameter-store-using-aws-sdk-v2-390a59cfdbae?source=rss-fd28ce5a235e------2)
- [How to Integrate Spring Boot 3 with Amazon SQS Using AWS SDK v2](https://awstip.com/how-to-integrate-spring-boot-3-with-amazon-sqs-using-aws-sdk-v2-044e93e4fc11?source=rss-fd28ce5a235e------2)
- [Access static content from S3 using CloudFront](https://awstip.com/access-static-content-from-s3-using-cloudfront-458d323041a1?source=rss-fd28ce5a235e------2)
- [How to Integrate Spring Boot 3 with Amazon S3 Using AWS SDK v2](https://awstip.com/how-to-integrate-spring-boot-3-with-amazon-s3-using-aws-sdk-v2-c5500f01df31?source=rss-fd28ce5a235e------2)
<!-- BLOG-POST-LIST:END -->

<div align="center">

<a href="https://www.toptal.com/resume/fahim-fahad#XM92Wo" target="_blank">
  <img src="/assets/toptal-badge.png" alt="Toptal Top 3% Talent Badge" width="180" height="180" style="border-radius: 12px; object-fit: contain;" />
</a>

</div>

---

## Connect

<p align="center">
  <a href="https://portfolio-three-snowy-36.vercel.app" target="_blank"><img src="https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=vercel&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/fahimfahadcseju/" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" /></a>
  <a href="https://medium.com/@fahimfahad92" target="_blank"><img src="https://img.shields.io/badge/Medium-000000?style=flat-square&logo=medium&logoColor=white" /></a>
  <a href="https://www.toptal.com/resume/fahim-fahad" target="_blank"><img src="https://img.shields.io/badge/Toptal-3863A0?style=flat-square&logo=toptal&logoColor=white" /></a>
  <a href="mailto:fahimfahad92@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" /></a>
</p>
