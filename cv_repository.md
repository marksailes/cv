# Mark Sailes — CV Experience Repository

_Working document. Not a CV. Source of truth for all three CV variants._

---

## Contact
- Leeds, UK (full address omitted on CV)
- LinkedIn: linkedin.com/in/mark-sailes
- sailes.co.uk
- DOB removed (UK convention; reduces age-discrimination signal)

---

## Roles

### Principal Solutions Architect, Leighton (AWS Advanced Partner)
**July 2025 – present**

- **Sole technical resource in the sales organisation** — own all technical requirements gathering and customer-facing sales conversations end-to-end.
- Working primarily on large enterprise engagements: migrations and greenfield builds.
- **Named customers since joining:** British Airways, IAG Loyalty, Greggs.
- Leighton is an AWS Advanced Partner; company turnover ~£10M.

### Specialist Solutions Architect, Amazon Web Services
**Aug 2018 – July 2025 (~7 years)**

**Progression:** L5 Solutions Architect (generalist, ~2 years) → joined Specialist org → promoted to L6 Senior Specialist SA

**Generalist phase (Aug 2018 – ~2020):** Worked with UK gambling industry customers, then ISVs. Broad workload exposure before specialising.

**Specialist scope:** UK & Ireland specialist for serverless (Lambda, API Gateway, SQS, SNS, Step Functions, EventBridge). 100+ customer projects across every industry/vertical.

**Internal recognition:**
- **AppMod "Think Big" Award** — 2022
- **UK SA "Learn and Be Curious" Award** — 2021

**Deal/revenue influence:** Average ~$10k MRR per customer engagement. Note: serverless workloads are low-cost-per-customer by design; impact-vs-revenue ratio is high. The **Barclays/Amazon JV credit card** engagement was the **largest AWS Lambda new-business opportunity worldwide** in its year.

**Specialism:** Java on AWS Lambda — 4 years building developer experience at this intersection.

**Flagship customer engagements:**
- **Disney** — worked on developer productivity improvements using serverless and open source. Published as an AWS Open Source Blog case study: `aws.amazon.com/blogs/opensource/improving-developer-productivity-at-disney-with-serverless-and-open-source/`. Notable that Disney rarely publishes case studies, making this a high-value reference for AWS.
- **Barclays / Amazon JV credit card** — designed/implemented idempotency on AWS Lambda for a new joint venture credit card product
- **Capital One** — designed active/active multi-region architecture
- **SonarQube / Sonar** — improved API latency using Lambda SnapStart + Micronaut (published as AWS blog: `aws.amazon.com/blogs/opensource/improving-api-performance-at-sonar-with-lambda-snapstart-and-micronaut/`)
- **UEFA World Cup 2022 start-up** — prepared a customer to absorb match-driven traffic spikes; coordinated AWS Premium Support live-coverage per match, drove service-quota increases across multiple service teams, advised the dev team on architectural isolation so low-priority workloads couldn't impact high-priority ones

**SnapStart leadership (flagship achievement):**
- Led the global technical field plan for AWS Lambda SnapStart — 2nd fastest-adopted Lambda feature of its launch year
- Delivered the first full-length re:Invent talk on SnapStart (re:Invent 2022) — primary technical voice post-keynote launch
- Trained 35 solutions architects globally to handle inbound SnapStart customer queries
- Identified a JVM tiered-compilation issue affecting Lambda Java cold starts; researched and proposed a fix; quantified that 99.9% of customer workloads would benefit and characterised the 0.01% regression case; drove the change through the Lambda service team to global rollout. Authored customer-facing blog content so customers could apply the change themselves ahead of the platform-level fix. Net result: ~50% reduction in first-invoke latency for Java Lambda workloads globally.
- Worked with open-source frameworks (Spring, Micronaut, Quarkus) to ship Day 1 support
- Authored the launch blog on the AWS Compute Blog
- Customer feedback I collected drove the SnapStart product roadmap for 2 years
- Identified a customer friction point affecting 14% of would-be adopters; partnered with PM to ship blog content, docs updates, and OSS nagging-tool fixes to address it
- Influenced prioritisation of ARM/Graviton support for SnapStart by quantifying the customer cohort blocked from adoption without it

**Other product/roadmap influence:**
- Contributor to quarterly AWS Lambda roadmap planning
- Technical blog reviewer for AWS
- Consulted by the Lambda service team on the Log4Shell (CVE-2021-44228) mitigation for the Java runtime. A peer engineer had developed a fix that materially affected customer code execution; the open question was whether the customer impact was acceptable. As the team's customer-facing technical voice, I was asked for the call. The fix shipped and mitigated Log4Shell for every AWS Lambda Java customer worldwide.
- AWS technical representative on the Micronaut Technical Advisory Board

**Internal advisory:**
- Advised internal AWS teams on Lambda + Java performance, including the EKS control plane team and internal HR teams

**Cost optimisation:**
- Regular customer billing reviews; standard saves via right-sizing and Reserved Instances.
- **Approach: used gamification to drive delivery teams to own and improve their own costs** — building durable FinOps culture inside customer engineering teams rather than running one-off audits.

**Speaking:**
- **re:Invent 2022** — first full-length SnapStart talk (post-keynote launch)
- **re:Invent 2023** — speaker
- **re:Invent 2024** — speaker
- **SpringOne 2023 — keynote speaker**
- **SpringOne 2021** — speaker
- **Devoxx UK 2025** — speaker
- **Devoxx Poland 2023** — speaker
- Micronaut Podcast (Jan 2023) — Lambda SnapStart + Micronaut 3.8

**Open source:**
- **Lambda Powertools for Java** — maintainer
- **aws-lambda-java-libs** — contributor (Java Lambda events library)
- Collaborated with Spring, Micronaut, Quarkus on SnapStart support

---

### Lead Software Engineer, Sky Betting & Gaming
**March 2016 – August 2018**

**Hiring context:** Recruited into SB&G specifically for prior experience designing real-time sports trading systems. Joined to design and build the next-generation Trading Engine from scratch.

**Team build:**
- **Designed the system. Hired the entire team** — 14 engineers, multi-disciplined (quantitative analysts, test engineers, software engineers, product owner).
- Line management and technical direction for the full squad.
- **Career development outcomes:**
  - Promoted one engineer to Senior.
  - Hired a sports trader (domain expert, non-engineer) and developed them into a working software engineer — rare cross-disciplinary career conversion.
- Performance-managed one team member out for behavioural reasons that were materially affecting team functioning.

**System scope and growth:**
- Trading Engine: ingested real-time data from football matches worldwide, ran mathematical models to calculate event probabilities, fed pricing into the consumer site and cash-out engine.
- **Coverage grew from lower-division football at launch to all UK football two years later — pre-match, in-play, and cash-out — including Premier League.**
- Responsible for balancing customer-facing attractiveness against the business's risk exposure on live money.

**Technical leadership:**
- **Led migration of the system from on-premise single-datacentre infrastructure to AWS cloud-native serverless.** This was the engagement that convinced me serverless was the right substrate for systems that have to survive infrastructure failure — and the origin point for the AWS specialism that followed.
- Designed a betting-suspension safety mechanism after a third-party data-feed supplier failure caused on-site probabilities to go stale. The original system did not detect data starvation; I designed the mechanism that suspends markets on stale opportunities, eliminating a real-money risk exposure to the business.

**Stakeholder management:**
- Primary stakeholders: Product Owner (in-squad), Head of Sports Trading (business side). Required ongoing trade-off conversations between trader-facing flexibility, customer-facing product behaviour, and risk exposure.

**Reason for leaving (for interview context, not CV):** Two management changes within ~18 months; role scope and compensation moved in directions that didn't reflect the work being carried. AWS specialist SA role was the right next step.

### Head of Delivery, Rockshore Ltd
**May 2014 – March 2016**

- Engineering management role at a client-services firm.
- Led **4 development teams** working concurrently on multiple external client projects.
- Notable client: **AT&T**.
- Responsible for delivery across the portfolio: technical direction, team health, and client outcomes.

---

### Earlier career: Software Engineer → Senior Engineer, William Hill
**~2007 – 2014 (7 years)**

- Joined as a graduate developer; progressed to Senior Engineer.
- Built **real-time sports trading systems across multiple sports**. This is the domain expertise that led Sky Bet to recruit me specifically in 2016.

---

## Cross-cutting

### Education
- **BSc Computing (with industrial placement)** — University of Leeds, 2006

### Certifications
- Held **8 AWS certifications** including **AWS Certified Solutions Architect – Professional**. Currently maintain 2 active. Working inside AWS for ~7 years provided depth beyond what certification renewal would add.

### Public artefacts
- AWS Compute Blog: SnapStart launch deep-dive (2022)
- AWS Open Source Blog: SonarQube + SnapStart + Micronaut case study
- Conference recordings on YouTube
- sailes.co.uk
- Micronaut Podcast (Jan 2023)

### Side project
- **Study From Experts** — premium video course platform for senior/principal engineers. Founder. Launched April 2026.

