# Hi, I'm Rachana 👋

**Software Engineer, Platform and Infrastructure** ☁️ 🛠️

I build the platform pieces other teams deploy on: Kubernetes, GitOps, Terraform, CI that tells you the truth, and data infrastructure that holds up at billions of rows.

For the last four years at HG Insights I've worked on Kubernetes reliability, search infrastructure, GitOps delivery, data warehouse migrations, and the CI platform that validates our CRM connectors end to end. Before that I spent years in test engineering, which is why I treat "how do we know this works in production" as part of the job, not someone else's.

🔎 **Open to work**

- ☁️ Platform Engineer, Infrastructure Engineer, Software Engineer (Platform). My main focus.
- 🧪 Senior SDET, Test Infrastructure, Developer Experience. Still open to these, and still good at them.

---

## 🏗️ Platform work at HG Insights

- **GitOps migration.** I moved our service deploys off an internal build system and onto Argo CD, and converted 15+ backend repos to trunk-based delivery. We now ship 5x as many deploys a week.
- **Search at 60x scale.** I scaled a customer-facing record-matching service from 1M to 60M companies on Elasticsearch.
- **Warehouse migrations.** I moved customer analytics from Snowflake to ClickHouse. The ClickHouse clusters are immutable, run on Kubernetes through Argo CD, and the cutovers were Route 53 changes in Terraform, all on an 8B-record serving layer.
- **Kubernetes reliability.** A service backed by 38M reference records kept failing health checks in production. I fixed it in the manifests.
- **Multi-tenant CI orchestration.** I built an eight-phase pipeline that leases staging tenants from a DynamoDB pool with compare-and-swap, seeds deterministic CRM data, and asserts exact row counts from S3 through Redshift to the serving layer. It covers six connectors, it's found about 40 platform bugs, and a failed run now costs 40 minutes to retry instead of 2.5 hours.
- **Least-privilege IAM.** I wrote the Terraform IAM policies for CI access across 12 AWS services and two cross-account roles. When we hit AWS's policy-size limit, I split the overflow into its own policy.
- **SaaS simulation with fault injection.** I built eight services that pretend to be third-party CRMs, and they can inject rate limits, timeouts, expired auth and partial outages on demand. That's how we hardened retry and recovery. Setting up an integration went from a week to two hours.
- **Self-healing CI.** I shipped an LLM agent into four production codebases. When a CI run fails it finds the root cause, applies a fix, reruns the full suite, and opens a draft PR so a person makes the final call.

---

## 🚢 Side projects

### 📊 ChurnGuard-AI: RAG + survival analysis for B2B churn

It's a demonstration project on seeded data, not real customers. I built a dbt warehouse, Qdrant retrieval over 771 documents, LangGraph agents, DuckDB locally and S3/Athena in production. AUC 0.877 for churn ranking, 0.791 on actual churners.

The README's the real point. I retracted a 94.7% accuracy I'd claimed earlier and wrote up why it was wrong. The 196-day date-prediction error and non-stationary hazard rates are listed as open gaps, and every claim that's left is backed with 52 dbt tests, 28 dataset validation checks, and reproducible retrieval benchmarks across 8 ADRs.

### 🔎 Multi-agent RAG platform: five retrieval strategies, measured against each other

FastAPI, LangChain and LangGraph, Qdrant, Next.js, Docker Compose. Dual-team agent architecture with five sub-agents, RAGAS evaluation, and synthetic data for baselines. I built it because I didn't want to pick a retrieval approach and hope. I wanted to compare them on evidence.

---

## ⚡ How I work

🧭 **I own the deploy path.** Building the service is half the job. I don't consider it done until it deploys through GitOps, reports somewhere people actually look, and can block a bad release.

🔍 **I debug across the whole stack.** Real failures live in the seams. I'll trace a problem from the API through the queue, the container, the IAM policy and into the database, and I'd rather prove a root cause than ship a plausible guess.

📈 **I've worked at scale, and it changes what survives.** Multi-tenant systems, billions of records, parallel workers. Shared state becomes flakiness and retries become stampedes, so I design for isolation, leases and guaranteed teardown from the start.

🧪 **I make systems provable.** I'd rather a regression block a release than reach a customer, so I use deterministic seed data, exact assertions, and thresholds that are wired into CI.

---

## 🧰 Tech

**☁️ Infrastructure & Cloud**

![Kubernetes](https://img.shields.io/badge/Kubernetes%20(EKS)-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Argo CD](https://img.shields.io/badge/Argo%20CD-EF7B4D?style=flat-square&logo=argo&logoColor=white)
![Kustomize](https://img.shields.io/badge/Kustomize-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![AWS](https://img.shields.io/badge/AWS%20(EKS%2C%20IAM%2C%20Route%2053%2C%20S3%2C%20Lambda%2C%20SQS%2C%20ECS%2C%20ECR)-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)

**🗄️ Data**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![ClickHouse](https://img.shields.io/badge/ClickHouse-FFCC01?style=flat-square&logo=clickhouse&logoColor=black)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=flat-square&logo=elasticsearch&logoColor=white)
![DynamoDB](https://img.shields.io/badge/DynamoDB-4053D6?style=flat-square&logo=amazondynamodb&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white)
![Redshift](https://img.shields.io/badge/Redshift-8C4FFF?style=flat-square&logo=amazonredshift&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white)
![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)

**💻 Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![HCL](https://img.shields.io/badge/HCL-7B42BC?style=flat-square&logo=terraform&logoColor=white)

**🧠 AI**

![Anthropic](https://img.shields.io/badge/Claude%20API-D97757?style=flat-square&logo=anthropic&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=flat-square&logo=anthropic&logoColor=white)

**🧪 Test**

![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)

**🏅 Certifications:** AWS Certified AI Practitioner, and Certified AI Engineer from AI Makerspace

---

## 🌐 Elsewhere

- 💼 [LinkedIn](https://www.linkedin.com/in/rachana-banik)
- 📫 r.banik16@gmail.com

If you're hiring for platform or infrastructure work, I'd like to hear from you.
