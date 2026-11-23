# Nabeegh Khan

I build and evaluate machine learning and LLM systems in Python: LLM extraction pipelines, retrieval-augmented generation (RAG) and the web and cloud services around them. I'm completing a Master of Engineering (MEng) in Electrical and Computer Engineering at the University of Toronto, with an emphasis in data analytics and machine learning, and I'm looking for full-time machine learning, AI, data and software roles from May 2027.

### What I'm working on

- **AI for Mental Health (AI-M) program, University of Toronto.** Research software engineer leading a team of two on an LLM pipeline that extracts evidence for depression (PHQ-8) and PTSD (PCL-C) items from clinical interview transcripts, toward publication. Every piece of evidence must be an exact quote from the transcript, checked in code. Against a psychiatrist-annotated key, precision rose from 0.53 to 0.66 on 17 validation sessions, and temperature scaling cut expected calibration error from 0.24 to 0.05. Over 300 tests run as a required CI check. The repository is private.
- **My Master of Engineering project.** A conversational AI agent that tests students' understanding of C programs they wrote, through tracing, what-if and follow-up questions, designed from over 90 papers. It has a Python backend with sandboxed runs, a job queue and PostgreSQL, a mobile-first React front end, and over 1,000 tests with Playwright end-to-end tests in CI, built for a January pilot. A session now asks tracing, what-if, concept-check and bug-you-hit questions, and a student whose program never compiled gets a debugging session instead. The work-in-progress abstract was accepted to ASEE 2027.
- **JurisEngine.** A jurisdiction-aware retrieval prototype for Canadian employment law. I built it in five days for the Vector Institute FastLane program and pitched it to its industry partner. Code resolves the province and the law in force on the date before retrieval, and the LLM only phrases an answer a validator checks. It met its four success metrics in CI, including 100% jurisdiction precision over 27,918 served citations. FastAPI on Supabase PostgreSQL, with a demo on Vercel. The repository is private.
- **Engineering education research, ISTEP.** Survey analysis in Python and LLM-assisted qualitative coding, toward an ASEE 2027 full paper and a CEEA 2027 paper with Dr. Qin Liu. Presented at the University of Toronto Engineering Research Conference in 2025 and 2026.
- **Graduate course projects, each with a team of four.** [FitnessCoach](https://github.com/harunm1/FitnessCoach) is a Next.js and TypeScript web application with an AI workout coach, on Vercel and Neon PostgreSQL. My part is the foundation and the LLM coach: streamed replies, guardrails, and failover between providers. [ContentCollab](https://github.com/nabeegh-khan/contentcollab) is a cloud application for reviewing documents together, live on DigitalOcean Kubernetes. My part is the architecture, cluster, worker service and browser client, with autoscaling from two to five API pods, Prometheus and Grafana, and load tests at up to 250 requests a second.

### Projects

- [3gpp-rag](https://github.com/nabeegh-khan/3gpp-rag): RAG over 4,493 pages of 3GPP telecom specifications, with cited answers, a FastAPI endpoint, a Streamlit interface and RAGAS evaluation. [Demo](https://youtu.be/tEcylKm4xwk)
- [real-time-anomaly-mlops](https://github.com/nabeegh-khan/real-time-anomaly-mlops): streaming anomaly detection from Kafka through Spark to a DuckDB and dbt feature store, served with FastAPI and tracked in MLflow.
- [6g-lwm-beam-prediction](https://github.com/nabeegh-khan/6g-lwm-beam-prediction): LoRA fine-tuning of a wireless foundation model for 6G beam prediction, with ONNX export and INT8 quantization.

### Earlier course projects

- [Ontario-Electricity-Demand-Forecasting](https://github.com/nabeegh-khan/Ontario-Electricity-Demand-Forecasting): next-hour demand forecasting from 109,056 hourly records; five models compared (machine learning course, Fall 2025; I built the pipeline and models, teammates reviewed).
- [cadusd-cot-feature-engineering](https://github.com/nabeegh-khan/cadusd-cot-feature-engineering): weekly CAD/USD features from CFTC Commitments of Traders and price data, with stationarity testing (AI in Finance course, Summer 2025; my part was the feature engineering).
- [canada-innovation-policy-analysis](https://github.com/nabeegh-khan/canada-innovation-policy-analysis): NewsAPI and YouTube Data API collection with topic clustering, findings reports and visualisations (data science course, Winter 2025).

### Background

Before graduate school I spent nearly six years in engineering, including two years leading project engineering and two in design on electrical and instrumentation and control projects, as a client point of contact. That's where I learned to turn requirements into specifications and check every change before it ships. I do the same with models: test them, audit them, and report what didn't work.

### Stack

**Machine learning and LLMs:** Python, PyTorch, Hugging Face Transformers, PEFT and LoRA, scikit-learn, pandas, OpenAI API, RAG, ChromaDB, RAGAS, ONNX

**Data and MLOps:** Kafka, Spark, DuckDB, dbt, MLflow, FastAPI, Docker

**Web and cloud (graduate coursework):** TypeScript, React, Next.js, Node.js, Express, PostgreSQL, Prisma, Supabase, Vercel, Kubernetes, Prometheus and Grafana, DigitalOcean

**Engineering practice:** Git, GitHub Actions, pytest, Jest, Playwright, pull-request review, Claude Code

### How I use AI

Each README says which parts AI wrote and which I designed and checked. I use AI coding assistants for implementation under my direction, and I verify results against the source.

[LinkedIn](https://www.linkedin.com/in/nabeeghkhan/) · nabeegh.as.khan@gmail.com · Cambridge, Ontario
