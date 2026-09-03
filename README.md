# Hi, I'm Rachana 👋

**Software Engineer in Test → Forward Deployed Engineer** 🛠️ → 🚀

I take AI systems from prototype to something a team can actually depend on.

9+ years building quality engineering and test infrastructure for distributed, event-driven systems on AWS, now applied to LLM systems: evaluation, guardrails, agent orchestration, and the release gates that make AI changes safe to ship. Forward-deployed work is where that lands — sitting with the people who have the problem, building the thing end to end, and owning it into production. The part most AI projects skip is the part I've done for a decade.

🔎 **Open to work** — Forward Deployed Engineer · AI Solutions Engineer · Applied AI · Platform / Developer Experience

---

## 🚢 Shipped

### 📊 ChurnGuard-AI — RAG + survival analysis for B2B churn

dbt warehouse, Qdrant retrieval over 771 documents, LangGraph agents, DuckDB locally and S3/Athena in production. AUC 0.877 for churn ranking, 0.791 on actual churners.

The README is the point. It retracts a previously claimed 94.7% accuracy and explains why the number was wrong, lists the 196-day date-prediction error and non-stationary hazard rates as open gaps, and backs every surviving claim with 52 dbt tests, 28 dataset validation checks, and reproducible retrieval benchmarks across 8 ADRs. Anyone can ship a demo that looks good. Deployed work needs someone who will tell you which half doesn't work yet.

### 🔎 Multi-agent RAG platform — five retrieval strategies, measured against each other

FastAPI, LangChain and LangGraph, Qdrant, Next.js, Docker Compose. Dual-team agent architecture with five sub-agents, RAGAS evaluation, and synthetic data generation for baselines. Built to compare retrieval approaches on evidence rather than pick one and hope.

### 🛠️ Next up

Forward-deployed style projects: customer-shaped problems solved end to end, with a real deploy path and evals that gate it. Shipping over the coming months — this section will keep growing.

---

## ⚡ How I work

🧪 **I make AI systems provable.** Golden sets, retrieval measured separately from generation so failures can be attributed to a stage, negative tests that verify refusal rather than fabrication, and thresholds wired into CI so a regression blocks a release instead of surfacing in front of a user.

🎯 **I build for someone specific, not for a spec.** Everything I've shipped had real consumers on the other side — versioned, reviewed, released on a cadence, and designed to be maintained by someone other than me. Getting other teams to actually adopt it is a people problem as much as an engineering one.

🚀 **I own the deploy path.** Kubernetes, Terraform, GitOps, GitHub Actions. Building the thing is half the job. Making it run on every deploy, report somewhere people actually look, and gate a release is the other half, and I don't hand that off.

🔍 **I debug across the whole stack.** Real failures live in the seams between systems, not inside one. I'll trace a problem from the UI through the API, the queue, the container, the IAM policy, and into the database, and I'd rather build a controlled experiment that confirms a root cause than ship a plausible guess.

📈 **I've worked at scale, and it changes what survives.** Multi-tenant systems, billions of records, distributed workers and queues. Hardcoded fixtures rot, retries turn into stampedes, and shared state across parallel workers becomes the flakiness. Per-worker namespacing, variance-bounded assertions, seeded data with guaranteed teardown. Load and stress testing with k6 and Locust, including autoscaler validation and non-deterministic tool-call paths.

🧭 **I set standards and grow people.** Owning a roadmap rather than a backlog: defining the reusable standard other teams adopt, agreeing conventions with developers before a feature ships, and mentoring engineers.

---

## 🧰 Tech

**🧠 AI & Agents**

![Anthropic](https://img.shields.io/badge/Claude%20API-D97757?style=flat-square&logo=anthropic&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white)
![RAGAS](https://img.shields.io/badge/RAGAS%20evals-8A2BE2?style=flat-square&logo=ray&logoColor=white)

**💻 Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**🌐 App & API**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

**☁️ Cloud & Infrastructure**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes%20(EKS)-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![Argo CD](https://img.shields.io/badge/Argo%20CD-EF7B4D?style=flat-square&logo=argo&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Datadog](https://img.shields.io/badge/Datadog-632CA6?style=flat-square&logo=datadog&logoColor=white)

**🗄️ Data**

![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)
![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black)
![Athena](https://img.shields.io/badge/S3%20%2F%20Athena-8C4FFF?style=flat-square&logo=amazonaws&logoColor=white)
![Redshift](https://img.shields.io/badge/Redshift-8C4FFF?style=flat-square&logo=amazonredshift&logoColor=white)
![ClickHouse](https://img.shields.io/badge/ClickHouse-FFCC01?style=flat-square&logo=clickhouse&logoColor=black)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white)

**🧪 Test & Load**

![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![WebdriverIO](https://img.shields.io/badge/WebdriverIO-EA5906?style=flat-square&logo=webdriverio&logoColor=white)
![Jest](https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white)
![k6](https://img.shields.io/badge/k6-7D64FF?style=flat-square&logo=k6&logoColor=white)
![Locust](https://img.shields.io/badge/Locust-2AA198?style=flat-square&logo=python&logoColor=white)

---

## 🌐 Elsewhere

- 💼 [LinkedIn](https://www.linkedin.com/in/rachana-banik)
- 📫 r.banik16@gmail.com
