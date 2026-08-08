# Nabeegh Khan

Licensed Professional Engineer (P.Eng) specializing in machine learning. MEng candidate in Electrical & Computer Engineering at the University of Toronto, graduating December 2026, with an emphasis in Data Analytics and Machine Learning. P.Eng, PMP, and five years of professional engineering experience.

I work on retrieval-augmented and NLP systems, foundation-model fine-tuning and compression, end-to-end ML pipelines, and machine learning for wireless communications, alongside engineering-education research as a graduate research assistant. Recent projects span a retrieval-augmented QA system over 3GPP standards with source citations, parameter-efficient fine-tuning of a wireless foundation model, a streaming MLOps pipeline, reinforcement and supervised learning for MIMO power allocation, beam prediction on real vehicle-to-vehicle measurements, and mixed-methods and bibliometric studies of generative AI in education. I try to build things that are reproducible and reported honestly, including the results that came out modest or negative.

## Selected projects

| Project | What it does | Stack |
|---|---|---|
| [3GPP Specification Assistant (RAG)](https://github.com/nabeegh-khan/3gpp-rag) | Retrieval-augmented QA over 14 3GPP NR specs (4,493 pages, 18,187 chunks). Answers come back with source citations, evaluated with RAGAS (faithfulness 0.675, context recall 0.750). | LangChain, ChromaDB, GPT-4o-mini, FastAPI, Streamlit, RAGAS |
| [LWM-LoRA: Scenario-Adaptive mmWave Beam Prediction](https://github.com/nabeegh-khan/6g-lwm-beam-prediction) | LoRA fine-tuning of the Large Wireless Model (LWM v1.1) for 64-beam mmWave prediction across three DeepMIMO scenarios. Rank-4 adapters train 4.82% of parameters and reach 76.8% top-1 on Miami; cross-scenario transfer with 20% of target data matches full fine-tuning within 0.3%; ONNX INT8 export cuts model size 69.5%. | PyTorch, HuggingFace, LoRA/PEFT, DeepMIMOv3, ONNX Runtime, W&B |
| [Real-Time Anomaly Detection MLOps](https://github.com/nabeegh-khan/real-time-anomaly-mlops) | Streaming anomaly-detection pipeline on the NAB benchmark: Kafka to Spark Structured Streaming to a DuckDB feature store, an LSTM autoencoder tracked in MLflow, FastAPI serving, Airflow orchestration, Evidently drift monitoring. ROC-AUC 0.64 on a hard unsupervised task, reported with its limitations. | PyTorch, Kafka, Spark, MLflow, FastAPI, Airflow, Evidently, DuckDB |
| [AI in the Classroom: Mixed-Methods Survey + Reddit](https://github.com/nabeegh-khan/ai-education-mixed-methods) | Convergent mixed-methods study integrating survey data (n=625) with 465 Reddit posts. Ordinal regression found attitude toward use the dominant predictor of AI adoption (OR=8.32, p<0.001). | BERTopic, VADER, spaCy, statsmodels, Reddit API |
| [DeepSense 6G V2V Beam Prediction](https://github.com/nabeegh-khan/deepsense-6g-beam-prediction) | mmWave beam prediction on 112,189 real V2V measurements (Scenarios 36–39, 60 GHz). Random Forest reached 22.6% top-1, beating every deep model I tried; a DQN analysis traced its ceiling to feature compression. | PyTorch, scikit-learn, DeepSense 6G, Gymnasium |
| [6G Massive MIMO Resource Allocation](https://github.com/nabeegh-khan/6g-mimo-resource-allocation) | DQN versus supervised learning for power allocation in a 7-cell, 70-user Massive MIMO environment. Supervised reward regression matched the DQN controller at 4.4× the random baseline, a cheaper alternative to RL on this problem. | PyTorch, Stable-Baselines3, Gymnasium |
| [AI-in-Education Bibliometric + NLP Analysis](https://github.com/nabeegh-khan/ai-education-bibliometric-analysis) | Collected 4,403 papers via the OpenAlex and Semantic Scholar APIs; BERTopic surfaced 27 research clusters; a chi-square test confirmed a post-ChatGPT topic shift (χ²=323.87, p<0.0001). | BERTopic, VADER, OpenAlex API, pandas, scipy |
| [Ontario Electricity Demand Forecasting](https://github.com/nabeegh-khan/Ontario-Electricity-Demand-Forecasting) | Hourly demand forecasting on 109,000+ records from IESO, Environment Canada, and NASA POWER, with 13 engineered features. Benchmarked five models; a 3-layer network cut RMSE 50.7% over the linear baseline. Three-person course project (ECE1513H); I owned data collection, feature engineering, model implementation, and the report. | scikit-learn, XGBoost, PyTorch, pandas |
| [Big Data Analytics: Spark & Azure Synapse](https://github.com/nabeegh-khan/big-data-analytics-spark-azure) | Distributed processing with Spark (RDD and DataFrame APIs, Scala on Databricks) and cloud SQL analytics on Azure Synapse over multi-file corpora and partitioned retail data. | Apache Spark, Scala, Databricks, Azure Synapse, T-SQL |

## Skills
**Machine learning:** PyTorch, scikit-learn, XGBoost, deep learning, CNN/LSTM/RNN, reinforcement learning (DQN, Stable-Baselines3, Gymnasium), Random Forest, SVM, feature engineering

**LLM & RAG:** LangChain, ChromaDB, OpenAI embeddings, GPT-4o-mini, RAGAS, LangSmith

**NLP & text analytics:** BERTopic, VADER, spaCy, topic modeling, qualitative coding

**Foundation models & transfer learning:** HuggingFace Transformers, LoRA/PEFT, Large Wireless Model (LWM), ONNX Runtime, INT8 quantization, Weights & Biases

**MLOps & serving:** MLflow, Airflow, Evidently, Docker, FastAPI, Streamlit, model serving, drift monitoring

**Streaming & data engineering:** Kafka, Spark Structured Streaming, DuckDB, dbt, Databricks, Azure Synapse

**Statistics & research methods:** chi-square, ANOVA, Mann-Whitney U, ordinal logistic regression, equivalence testing, mixed-methods research, hypothesis testing, statsmodels, scipy

**Domain experience (wireless):** mmWave beam prediction, beamforming, massive MIMO, V2V communications, DeepMIMO and DeepSense 6G datasets

**Languages & tools:** Python, Scala, SQL, Git, Jupyter, pandas, NumPy, Matplotlib, Seaborn, Plotly

## Now

* Finishing my MEng in Electrical & Computer Engineering at the University of Toronto, graduating December 2026. Available for full-time roles from January 2027.
* Based in Cambridge, Ontario. Open to roles in the Waterloo Region, the Greater Toronto Area, and remote across Canada.
* Research Assistant at ISTEP, University of Toronto (summers 2025 and 2026). Quantitative and qualitative analysis of engineering-education survey data; co-authored a research brief and presented a poster at UTERC 2025.

## A note on tooling

These projects were built with significant AI-assisted coding; I used Claude (Anthropic) as a coding assistant. I scoped the questions, chose the datasets and methods, and ran, validated, and interpreted the results. Each repository documents this in its README.
