# Nabeegh Khan

Master of Engineering (MEng) student in Electrical & Computer Engineering at the University of Toronto, graduating April 2027, with an emphasis in Data Analytics and Machine Learning. Licensed Professional Engineer (P.Eng) and PMP, with six years in engineering, most recently four years of nuclear electrical and instrumentation design, now working in applied machine learning.

My work sits between applied NLP and the research methods that make a result mean something: retrieval and its evaluation, parameter-efficient fine-tuning and compression, and the annotation, statistics and record linkage underneath. Alongside that, engineering-education research as a graduate research assistant, and clinical NLP as a research volunteer. I try to build things that are reproducible and reported honestly, including the results that came out modest or negative.

[ORCID](https://orcid.org/0009-0007-3142-7372) · nabeegh.khan@mail.utoronto.ca · Cambridge, Ontario

## Now

* **Research Volunteer, Artificial Intelligence for Mental Health (AI-M) Program**, University of Toronto, with Unity Health Toronto and University Health Network, since September 2026. Retrieval-augmented extraction of clinical scale items (PHQ-8 depression, PCL post-traumatic stress) from interview transcripts on the public Distress Analysis Interview Corpus, Wizard of Oz. The design answers an item only where the transcript carries evidence and abstains otherwise, so coverage is reported alongside accuracy rather than a single score.
* MEng student at the University of Toronto, graduating April 2027. Open to part-time research and analysis work through the coming year, and full-time roles from May 2027.
* Based in Cambridge, Ontario. Open to roles in the Waterloo Region, the Greater Toronto Area, and remote across Canada.

## Selected projects

| Project | What it does | Stack |
|---|---|---|
| [3GPP Specification Assistant (RAG)](https://github.com/nabeegh-khan/3gpp-rag) | Retrieval-augmented QA over 13 3GPP specifications: 4,493 pages extracted with PyPDF and recursive character splitting into 18,187 chunks in ChromaDB, served through FastAPI with citations back to source document and page. Evaluated with RAGAS across four metrics; the weakest traced to segmentation rather than the model, since fixed-size chunking was separating tables from their headers. | LangChain, ChromaDB, GPT-4o-mini, FastAPI, Streamlit, RAGAS, LangSmith |
| [AI in the Classroom: Mixed-Methods Survey + Reddit](https://github.com/nabeegh-khan/ai-education-mixed-methods) | Convergent design integrating 625 published survey responses with 465 Reddit posts I collected, coded deductively with spaCy PhraseMatcher against pre-defined categories and inductively with BERTopic. Ordinal regression found attitude toward use the dominant predictor of adoption (OR=8.32, p<0.001); self-report and discourse diverge on academic writing. | BERTopic, VADER, spaCy, statsmodels, Reddit JSON |
| [AI-in-Education Bibliometric + NLP Analysis](https://github.com/nabeegh-khan/ai-education-bibliometric-analysis) | 4,403 records harvested from OpenAlex with cursor pagination and rate-limit handling, joined to Semantic Scholar on DOI and deduplicated on the OpenAlex identifier. BERTopic surfaced 27 clusters; a chi-square test confirmed a post-ChatGPT topic shift (χ²=323.87, p<0.0001). | BERTopic, VADER, OpenAlex API, pandas, scipy |
| [LWM-LoRA: Scenario-Adaptive mmWave Beam Prediction](https://github.com/nabeegh-khan/6g-lwm-beam-prediction) | LoRA fine-tuning of the Large Wireless Model for 64-beam prediction across three DeepMIMO scenarios. Rank-4 adapters train 4.82% of parameters and reach 76.8% top-1; cross-scenario transfer with 20% of target data matches full fine-tuning within 0.3%. ONNX Runtime on CPU runs 3.38x faster than PyTorch on GPU for single-sample inference at no accuracy loss; INT8 quantization cuts model size 69.5% for a 2.5-point accuracy cost and no latency gain. | PyTorch, HuggingFace, LoRA/PEFT, DeepMIMOv3, ONNX Runtime, W&B |
| [Real-Time Anomaly Detection MLOps](https://github.com/nabeegh-khan/real-time-anomaly-mlops) | Streaming pipeline built as a `src/` package: Kafka into Spark Structured Streaming, rolling features materialised into a DuckDB feature store with dbt models and schema tests, an LSTM autoencoder tracked in MLflow, a Dockerised FastAPI endpoint with Pydantic validation, Airflow orchestration and Evidently drift monitoring. ROC-AUC 0.64 on a hard unsupervised task, reported with its limitations. | Kafka, Spark, DuckDB, dbt, PyTorch, MLflow, Airflow, FastAPI, Docker, Evidently |
| [Ontario Electricity Demand Forecasting](https://github.com/nabeegh-khan/Ontario-Electricity-Demand-Forecasting) | 109,056 hourly records (Jun 2013 – Nov 2025) assembled from four sources with three join keys and two time granularities: IESO hourly demand, Environment Canada hourly weather downloaded month by month from station 51459, NASA POWER daily solar irradiance broadcast across hours, and Ontario statutory holidays left-joined so no hours were dropped. 13 engineered features including 1h/24h/168h demand lags, cyclical sine/cosine time encodings and heating/cooling degree days. Five models benchmarked; a 3-layer network reached RMSE 203.92 MW and R² 0.9928, cutting error 50.7% against the linear baseline. Three-person course project (ECE1513H); I owned data collection, feature engineering, model implementation and the report. | pandas, scikit-learn (MLPRegressor), XGBoost, requests |
| [Big Data Analytics: Spark & Azure Synapse](https://github.com/nabeegh-khan/big-data-analytics-spark-azure) | MEM6287, Advanced Data Analytics, University of Ottawa, group of three. Distributed processing with Spark (RDD and DataFrame APIs, Scala on Databricks) and cloud SQL analytics on Azure Synapse over multi-file text corpora and partitioned retail data. A second healthcare component used Power BI with a geospatial join, linking patient encounters to dwelling value and gross rent by Forward Sortation Area. | Apache Spark, Scala, Databricks, Azure Synapse, T-SQL, Power BI |
| [DeepSense 6G V2V Beam Prediction](https://github.com/nabeegh-khan/deepsense-6g-beam-prediction) | Beam prediction on 112,189 real vehicle-to-vehicle measurements at 60 GHz. Random Forest reached 22.6% top-1, beating every deep model I tried; a DQN analysis traced its ceiling to feature compression. | PyTorch, scikit-learn, DeepSense 6G, Gymnasium |
| [6G Massive MIMO Resource Allocation](https://github.com/nabeegh-khan/6g-mimo-resource-allocation) | DQN versus supervised learning for power allocation across 7 cells and 70 users. Supervised reward regression matched the DQN controller at 4.4× the random baseline, a cheaper alternative to RL on this problem. | PyTorch, Stable-Baselines3, Gymnasium |

## Research experience

**Research Assistant, ISTEP, University of Toronto — May to August 2026.** Quantitative analysis of roughly 4,700 responses across three Faculty surveys under Dr. Qin Liu: chi-square with permutation p-values, Fisher's exact, Mann-Whitney U, two one-sided tests for equivalence, logistic regression and k-means, with Benjamini-Hochberg and Bonferroni corrections across 74 tests. Built a record linkage matching 723 students across two survey years by encrypted identifier. Conducted one semi-structured interview and co-led another under a Health Sciences REB protocol. Co-authored the research brief delivered to a Vice Dean and Deans of Undergraduate Studies.

**Research Assistant, ISTEP, University of Toronto — May to August 2025.** Mixed-methods analysis of generative-AI adoption among 124 engineering students under Dr. Qin Liu: descriptive statistics, chi-square testing and demographic breakdowns, with inductive coding of over 1,000 open-ended responses verified against a deductive scheme and thematic analysis run through the OpenAI API.

**Presentations.** Podium presentation at UTERC 2026 on whether an undeclared-entry pathway supported disciplinary exploration; poster at UTERC 2025 on student adoption of generative AI. Both with Dr. Qin Liu.

## Earlier data work

Graduate coursework at the University of Ottawa, all of which predates any use of AI tools and was done without them. The Spark and Azure Synapse work from MEM6287 is in the projects table above.

**MEM5300, Principles of Data Analytics.** Full CRISP-DM pipeline in IBM SPSS Modeler over 20,867 records extracted from 800 images of the Avila Bible, classifying the work of 12 copyists. A data audit on the type node found large outliers and no missing values; fractional ranking binning converted z-scored features into a continuous 0–19 range while keeping 100% valid records, benchmarked against six iterations of an outlier and extreme SuperNode using nullify and algorithm imputation. A heavily imbalanced target was balanced with a boost node before partitioning, then a C5.0 decision tree, an artificial neural network and K-Means clustering were compared. Group of five; I ran the data export and deployment, the K-Means report node, independent verification of the team's models, and produced the report.

**MEM5265, Business Intelligence and Performance Management.** Delivered an optional session on data cleansing methodology drawn from the work above, covering data warehousing and star schema design.

## Skills

**NLP & retrieval:** LangChain, ChromaDB, OpenAI embeddings, RAGAS retrieval evaluation, LangSmith, BERTopic, VADER, spaCy, NLTK, TF-IDF, topic modeling, qualitative coding, content analysis

**Foundation models:** HuggingFace Transformers, LoRA/PEFT, ONNX Runtime, INT8 quantization, Weights & Biases

**Machine learning:** PyTorch, scikit-learn, XGBoost, CNN/LSTM/RNN, Random Forest, SVM, reinforcement learning (DQN, Stable-Baselines3, Gymnasium), feature engineering

**Statistics & research methods:** chi-square with permutation p-values, Mann-Whitney U, Fisher's exact, ordinal and binary logistic regression, two one-sided tests for equivalence, k-means, Benjamini-Hochberg and Bonferroni correction, effect sizes, mixed-methods research, semi-structured interviews under REB protocol, statsmodels, scipy

**Data collection & linkage:** REST API harvesting with cursor pagination and rate limiting (OpenAlex, Semantic Scholar, NewsAPI, YouTube Data API, Reddit JSON), text extraction from PDFs (PyPDF, recursive character splitting), record linkage, schema and value-code reconciliation, deduplication, de-identification

**Data engineering & pipelines:** Kafka, Spark Structured Streaming (RDD and DataFrame APIs), DuckDB, dbt, Databricks, Azure Synapse, Airflow, ETL design

**Serving & MLOps:** MLflow, Evidently, Docker, FastAPI, Pydantic, Streamlit, drift monitoring

**Wireless domain:** mmWave beam prediction, beamforming, massive MIMO, V2V, DeepMIMO and DeepSense 6G

**Languages & tools:** Python, Scala, SQL, Git, Jupyter, pandas, NumPy, Matplotlib, Seaborn, Plotly, IBM SPSS Modeler, Power BI

## A note on tooling

My own projects above were built with significant AI-assisted coding; I used Claude (Anthropic) as a coding assistant. I scoped the questions, chose the datasets and methods, and ran, validated and interpreted the results. Each repository documents this in its README. The research assistantships were assisted in prompt design and model-assisted analysis through the University's licensed accounts, and I keep a dated log of that use. The University of Ottawa coursework predates all of this and was done without AI assistance.
