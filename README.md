# Nabeegh Khan

Engineer building applied AI and full-stack software, with personal projects in telecom and wireless. I'm completing a Master of Engineering in Electrical & Computer Engineering at the University of Toronto in April 2027, after nearly six years on cross-functional client teams, four of them in project engineering and design.

### Current work

**AI for Mental Health (AI-M), University of Toronto.** Building a two-stage LLM pipeline that extracts evidence from clinical interview transcripts and scores questionnaire items: depression (PHQ-8) first, then PTSD (PCL-C) and anxiety (GAD-7), toward a co-authored journal paper. Versioned, audited prompts raised held-out recall from 0.54 to 0.63 at 0.92 precision, and seven models were compared on recall, false positives and cost. Two raters audit sessions independently and report Cohen's kappa. I lead the repository for a three-person team: pull requests to a protected main branch under a mutual-review rule and 87 unit tests in GitHub Actions CI (64 merged, the rest in review). The repository is private.

**MEng project, with Dr. Salma Emara.** CAIRO, an AI agent that questions students about C programs they wrote and gives feedback on their answers. A sandboxed run of the student's code produces verified facts that ground the agent's questions and scoring. 36 papers read and noted, an ASEE 2027 work-in-progress abstract submitted, and the design accepted at the October design proposal; the build runs to December.

**Graduate course projects, fall 2026.** [FitnessCoach](https://github.com/harunm1/FitnessCoach), a full-stack TypeScript web application that recommends workout plans with an AI coaching agent, and [ContentCollab](https://github.com/nabeegh-khan/contentcollab), a stateful cloud-native application on DigitalOcean, each built with a team of four.

**Engineering education research, ISTEP.** Survey analysis and an ASEE 2027 paper, with the abstract submitted in October.

### Personal projects

- [3gpp-rag](https://github.com/nabeegh-khan/3gpp-rag): retrieval-augmented assistant over 4,493 pages of 3GPP specifications, with grounded, cited answers, a FastAPI endpoint, a Streamlit interface and RAGAS evaluation. [Demo](https://youtu.be/tEcylKm4xwk)
- [6g-lwm-beam-prediction](https://github.com/nabeegh-khan/6g-lwm-beam-prediction): LoRA fine-tuning of a wireless foundation model for 6G beam prediction, with ONNX export and INT8 quantization for edge inference.
- [real-time-anomaly-mlops](https://github.com/nabeegh-khan/real-time-anomaly-mlops): streaming anomaly detection from Kafka through Spark to a dbt feature store, with MLflow experiment tracking and Evidently drift monitoring.

### Earlier course projects

- [Ontario-Electricity-Demand-Forecasting](https://github.com/nabeegh-khan/Ontario-Electricity-Demand-Forecasting): next-hour demand forecasting from 109,056 hourly records; five models compared, a three-layer neural network best (machine learning course, Fall 2025; I built the pipeline and models, teammates reviewed).
- [cadusd-cot-feature-engineering](https://github.com/nabeegh-khan/cadusd-cot-feature-engineering): weekly CAD/USD features from CFTC Commitments of Traders and price data, with stationarity testing (AI in Finance course, Summer 2025; my part was the feature engineering).
- [canada-innovation-policy-analysis](https://github.com/nabeegh-khan/canada-innovation-policy-analysis): NewsAPI and YouTube Data API collection with topic clustering, findings reports and policy visualisations (data science course, Winter 2025).

### Toolchain

**Languages:** Python, JavaScript, Scala

**Machine learning and LLMs:** PyTorch, Hugging Face Transformers, PEFT and LoRA fine-tuning, scikit-learn, XGBoost, ONNX export and INT8 quantization, OpenAI and OpenRouter APIs, RAG, LangChain, ChromaDB, multi-agent design, prompt engineering

**LLM evaluation:** prompt and version management, offline evaluation against human-review audits, RAGAS, precision and recall, Cohen's kappa

**Web and cloud (graduate coursework):** Node.js, Express, REST APIs, TypeScript, React, Next.js, PostgreSQL, SQLite, Docker Compose, Nginx, DigitalOcean

**Data and MLOps:** Kafka, Spark Structured Streaming, Spark SQL on Databricks, DuckDB and dbt, Airflow, MLflow, Evidently, Docker, FastAPI

**Engineering practice:** Git, GitHub Actions CI, pytest, Jest, pull-request review, branch protection, Claude Code

**Statistics:** chi-square, Fisher's exact, Mann-Whitney U, logistic regression, equivalence testing, ADF and KPSS stationarity tests, multiple-comparison correction

### A note on tooling

Problem formulation, method selection, experimental design and interpretation in these projects are my own. I use AI coding assistants for implementation under my direction and verify every result against source. Each repository documents this.

**Open to full-time roles from May 2027.**

[LinkedIn](https://www.linkedin.com/in/nabeeghkhan/) · nabeegh.as.khan@gmail.com · Based in Cambridge, Ontario.
