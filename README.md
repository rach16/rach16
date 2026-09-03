Hi, I'm Rachana 👋

I take AI systems from prototype to something a team can actually depend on.

9+ years building quality engineering and test infrastructure for distributed, event-driven systems on AWS, now applied to LLM systems: evaluation, guardrails, agent orchestration, and the release gates that make AI changes safe to ship. The part most AI projects skip is the part I've done for a decade.

🚢 Shipped

🤖 Autonomous test-repair agent — production, post security review

A LangGraph agent that repairs broken tests without a human in the loop, running against a real codebase with real consequences. The engineering is in the constraints, not the prompt: confidence gating, per-run fix caps, scoped permissions, and a hard never-auto-merge rule. It passed security review before it went live. Agents that touch a company's repository are a trust problem before they're a modeling problem.

📊 ChurnGuard-AI — RAG + survival analysis for B2B churn

dbt warehouse, Qdrant retrieval over 771 documents, LangGraph agents, DuckDB locally and S3/Athena in production. AUC 0.877 for churn ranking, 0.791 on actual churners.

The README is the point. It retracts a previously claimed 94.7% accuracy and explains why the number was wrong, lists the 196-day date-prediction error and non-stationary hazard rates as open gaps, and backs every surviving claim with 52 dbt tests, 28 dataset validation checks, and reproducible retrieval benchmarks across 8 ADRs. Anyone can ship a demo that looks good. Deployed work needs someone who will tell you which half doesn't work yet.

🔎 Multi-agent RAG platform — five retrieval strategies, measured against each other

FastAPI, LangChain and LangGraph, Qdrant, Next.js, Docker Compose. Dual-team agent architecture with five sub-agents, RAGAS evaluation, and synthetic data generation for baselines. Built to compare retrieval approaches on evidence rather than pick one and hope.


⚡ How I work

🧪 I make AI systems provable. Golden sets, retrieval measured separately from generation so failures can be attributed to a stage, negative tests that verify refusal rather than fabrication, and thresholds wired into CI so a regression blocks a release instead of surfacing in front of a user.

🚀 I own the deploy path. Kubernetes, Terraform, GitOps, GitHub Actions. Building the thing is half the job. Making it run on every deploy, report somewhere people actually look, and gate a release is the other half, and I don't hand that off.

🔍 I debug across the whole stack. Real failures live in the seams between systems, not inside one. I'll trace a problem from the UI through the API, the queue, the container, the IAM policy, and into the database, and I'd rather build a controlled experiment that confirms a root cause than ship a plausible guess.

📈 I've worked at scale, and it changes what survives. Multi-tenant systems, billions of records, distributed workers and queues. Hardcoded fixtures rot, retries turn into stampedes, and shared state across parallel workers becomes the flakiness. Per-worker namespacing, variance-bounded assertions, seeded data with guaranteed teardown. Load and stress testing with k6 and Locust, including autoscaler validation and non-deterministic tool-call paths.

🧭 I set standards and grow people. Owning a roadmap rather than a backlog: defining the reusable standard other teams adopt, agreeing conventions with developers before a feature ships, and mentoring engineers.
