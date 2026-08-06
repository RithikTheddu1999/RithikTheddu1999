# Rithik Theddu

**AI Engineer at [Capco](https://www.capco.com/)** — I build production RAG systems and the data pipelines underneath them for financial services clients.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square)](https://www.linkedin.com/in/rithikreddy-dev/)
[![Email](https://img.shields.io/badge/Email-Get%20in%20touch-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:rithiksunny1999@gmail.com)
[![Resume](https://img.shields.io/badge/Resume-View-4285F4?style=flat-square&logo=googledocs&logoColor=white)](https://docs.google.com/document/d/1--KckuCO9q3K9TdftpMhG3RrJpmvfdha/edit?usp=sharing&ouid=114686238345698614306&rtpof=true&sd=true)
[![HackerRank](https://img.shields.io/badge/HackerRank-Profile-00EA64?style=flat-square&logo=hackerrank&logoColor=white)](https://www.hackerrank.com/profile/rithiksunny1999)

📍 Maitland, FL · H-1B · MS Computer Science, George Mason University

---

## What I'm working on

At Capco I own AI features end-to-end for financial services clients — React front-ends through FastAPI services to the retrieval layer and the pipelines that feed it.

- **RAG in production.** Snowflake and DealCloud sources normalized and chunked to 80–200 words with metadata, retrieved through Amazon Kendra, generated with GPT-4.1 / GPT-5 via OpenAI and Bedrock. Low-latency streaming responses, with PII scrubbing and prompt-injection defenses in the request path.
- **The data underneath.** PySpark transforms on Databricks and AWS Glue, curated datasets persisted to S3 and DynamoDB.
- **The infrastructure around it.** Terraform-managed AWS, deployed across EC2/ECS/EKS/Lambda with Step Functions, monitored on CloudWatch against defined latency and cost SLOs.

Before this: ETL for financial portfolio data at **State Street** (PySpark, Airflow, Databricks, Redshift), enterprise Java at **Caliber IT**, and .NET full-stack at **Cognizant**.

---

## Selected projects

| Project | What it does | Why it's interesting |
|---|---|---|
| **[CommitLens AI](https://github.com/RithikTheddu1999/commitlens-ai)** <br/> `Python` `FastAPI` `Next.js` | Extracts measurable executive commitments from earnings calls, investor letters, and press releases into a cited, auditable ledger with a reliability score per commitment. | Six sequential agents — intake, extraction, evidence research, verification, financial risk, governance — coordinated in plain Python with **no agent framework**. The scoring model (`commitlens_crs_aggregate_v1`) is deterministic: the LLM reads language, Python owns every number, date, and status transition. Auditable by design, which is the only way this ships in finance. |
| **[News Automater](https://github.com/RithikTheddu1999/news-automater)** <br/> `Python` `Docker` `GDELT` | Autonomous pipeline: discovers news every 30 minutes, generates grounded articles with AI imagery, and pushes them through WordPress and LinkedIn adapters with no manual approval step. | A **zero-token local pre-gate** filters on newness, corroboration, and relevance *before* any paid API call, and syndicated wire duplicates collapse via union-find so they don't inflate the source count. Hard spend ceilings enforced pre-call, grounding audit on every draft, offline fixture mode for deterministic tests. Publishing adapters run mocked end-to-end — real credentials swap in at the adapter boundary. |
| **[Smart Voting System](https://github.com/RithikTheddu1999/Smart-Voting-System)** <br/> `Python` `OpenCV` | Three-factor voter authentication: election ID → OTP → face recognition. | Local Binary Pattern face recognition over Haar cascade detection, trained per-voter at registration. Layered auth where each factor fails closed. |
| **[StudyBuddy](https://github.com/RithikTheddu1999/StudyBuddy)** <br/> `Django` | Topic-based study rooms with real-time discussion — a focused take on Discord for study groups. | Full Django app with a JSON API endpoint and role-scoped room access. [**Demo video →**](https://youtu.be/3i34TAig4Eg) |
| **[Masking Tool](https://github.com/RithikTheddu1999/masking-tool)** <br/> `Python` | Config-driven PII masking for Excel datasets, with full rollback. | Masking is reversible: a run-keyed data dictionary with per-run backups lets you walk any dataset back to a prior state — the part most masking tools skip, and the part compliance actually asks about. |

---

## Technical focus

| | |
|---|---|
| **Languages** | Python, PySpark, SQL, Java, C#, JavaScript, R |
| **AI / Retrieval** | RAG, GPT-4.1 / GPT-5, Amazon Bedrock, Kendra, SageMaker, few-shot prompting, response streaming |
| **Data** | Snowflake, Redshift, Databricks, Airflow, AWS Glue, PostgreSQL, DynamoDB, S3 |
| **Backend** | FastAPI, Django, Flask, Spring Boot, Node.js, ASP.NET |
| **Frontend** | React, Redux, Hooks, MUI, WebSockets, Angular |
| **Cloud / Ops** | AWS, Azure, Terraform, ECS, EKS, Lambda, Step Functions, IAM, VPC, CloudWatch, CI/CD |

---

## 2026 focus

Agent evaluation and observability — specifically, how you prove a multi-step agent pipeline is *correct* rather than merely plausible. Deterministic scoring, grounding audits, and replayable traces are the thread running through most of what I build.

---

**Open to AI/ML engineering roles.** Reach me at [rithiksunny1999@gmail.com](mailto:rithiksunny1999@gmail.com) or on [LinkedIn](https://www.linkedin.com/in/rithikreddy-dev/).
