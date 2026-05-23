<div align="center">

<!-- ELITE TYPING HEADER -->
<a href="https://github.com/shivam-nayak-ds">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=38&pause=1500&color=00E5FF&center=true&vCenter=true&width=800&height=100&lines=SHIVAM+NAYAK;AI+Systems+Engineer;GenAI+%26+Applied+ML;0-to-1+Infrastructure+Builder" alt="Typing SVG" />
</a>

> **Bridging the gap between ML research and production-grade scalable systems.** <br> I specialize in architecting stateful Agentic workflows, advanced Information Retrieval (RAG) pipelines, and low-latency ML microservices. I build AI systems that are deterministic, evaluation-driven, and fault-tolerant.

<br>

<p align="center">
  <a href="https://www.linkedin.com/in/shivam-nayakk"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=101010" alt="LinkedIn" /></a>
  <a href="mailto:shivamnayak296@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white&labelColor=101010" alt="Email" /></a>
  <a href="https://github.com/shivam-nayak-ds"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white&labelColor=101010" alt="GitHub" /></a>
</p>

</div>

---

### 🧠 Core Engineering Expertise

I don't just train models in isolation; I engineer complete, production-ready AI architectures.

*   **Generative AI & Agentic Systems:** Orchestrating complex, multi-step reasoning workflows using function-calling LLMs, **LangGraph** (stateful agents), and **CrewAI**. Designing robust system prompts, tool abstractions, and fallback routing.
*   **Advanced RAG Architectures:** Moving beyond naive retrieval. Implementing semantic chunking, dense/sparse hybrid search, query rewriting, and **MS-MARCO cross-encoder re-ranking** to minimize context hallucinations.
*   **Applied CV & Remote Sensing AI:** Engineering scalable pipelines for high-resolution satellite imagery, geospatial data processing, and object detection/segmentation using **PyTorch** and **TensorFlow**.
*   **MLOps & AI Infrastructure:** Designing reproducible training pipelines, robust experiment tracking (**MLflow**, **DVC**), and deploying heavily optimized, high-throughput model endpoints using **FastAPI** and **Docker**.

---

### ⚙️ Engineering Principles

> *The philosophies that drive my system design.*

| Principle | Execution |
| :--- | :--- |
| **Evaluation-Driven** | Relying on programmatic evaluation (LLM-as-a-judge, ROUGE, BERTScore) over "vibes" to measure retrieval precision and generation groundedness. |
| **Inference Optimization** | Obsessing over P99 latency, cost-per-token, KV-cache optimization, and batch-processing for both LLMs and traditional predictive models. |
| **Deployment-First** | Architecting modular, containerized systems from Day 1. If it doesn't run reliably in a Dockerized CI/CD pipeline, it's not finished. |
| **System Observability** | Implementing strict telemetry, logging, and monitoring for AI endpoints to detect data drift and gracefully handle edge cases in production. |

---

### 🏗️ Featured System Architectures

#### 1. [Enterprise-Grade Document Intelligence (Advanced RAG)](https://github.com/shivam-nayak-ds/Semantic-Resume-Insight-RAG)
*High-precision, hallucination-resistant retrieval system for unstructured HR data.*
*   **Architecture:** 2-Stage Retrieval Pipeline (Vector Search via **ChromaDB** + Cross-Encoder Re-Ranking).
*   **Engineering Challenge:** Naive RAG failed at highly specific deterministic queries (e.g., exact years of experience).
*   **Solution:** Implemented structured LLM metadata extraction layered over semantic search, using **Groq (Llama-3)** for ultra-low latency inference, drastically improving retrieval precision.

#### 2. [High-Throughput Anomaly Detection API](https://github.com/shivam-nayak-ds/Fraud-detection-ml-system)
*Low-latency microservice for real-time transaction fraud detection.*
*   **Architecture:** Optimized predictive model served via asynchronous **FastAPI** backend, fully containerized.
*   **Engineering Challenge:** Extreme dataset class imbalance leading to high false-negative rates on edge-case fraud.
*   **Solution:** Engineered an automated preprocessing pipeline utilizing targeted **SMOTE** oversampling. Tuned the inference server to maintain sub-100ms response times under concurrent load.

#### 3. [End-to-End Retail MLOps Pipeline](https://github.com/shivam-nayak-ds/Retail-Ops-End-to-End-Sales-Forecasting-Pipeline)
*Scalable, version-controlled machine learning pipeline for demand forecasting.*
*   **Architecture:** Modular ETL and training pipeline with decoupled data ingestion, model validation, and deployment stages.
*   **Engineering Challenge:** Ensuring reproducibility and tracking model decay across dynamic, shifting retail datasets.
*   **Solution:** Integrated **MLflow** for rigorous experiment tracking and hyperparameter tuning, paired with **DVC** for deterministic large-scale data versioning.

---

### 🛠️ Technical Ecosystem

**AI & Machine Learning Ecosystem**  
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit_learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)

**GenAI, RAG & Agents**  
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![CrewAI](https://img.shields.io/badge/CrewAI-FF4F00?style=flat-square)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF4F00?style=flat-square&logo=chroma&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=flat-square)

**MLOps, Backend & Infra**  
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/CI/CD-2088FF?style=flat-square&logo=github-actions&logoColor=white)

---

### 🔭 Current Focus & Research

*   **Agentic System Design:** Exploring robust routing, reflection, and state-management patterns in multi-agent workflows using LangGraph.
*   **Inference & Cost Optimization:** Evaluating open-source model deployment strategies (vLLM, Ollama) and techniques like model quantization.
*   **RAG Evaluation:** Implementing rigorous, metric-driven evaluation frameworks for retrieval systems to systematically reduce hallucinations.
*   **Remote Sensing AI:** Applying modern CV architectures to massive geospatial datasets for scalable Earth-observation analytics.

---

### 📊 Engineering Analytics

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=shivam-nayak-ds&theme=tokyonight&border_radius=4&hide_border=true" width="48%" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=shivam-nayak-ds&layout=compact&theme=tokyonight&border_radius=4&hide_border=true" width="48%" />
</div>

<br>

<div align="center">
  <h3>🤝 Let's Build the Future</h3>
  <p>I am currently exploring opportunities to join high-velocity AI startups as a Core/Founding AI Engineer.<br> If you are building scalable, complex AI products and need an engineer who can own systems from data to deployment—<b><a href="mailto:shivamnayak296@gmail.com">let's talk.</a></b></p>
  
  <img src="https://komarev.com/ghpvc/?username=shivam-nayak-ds&label=SYSTEM+HITS&color=00E5FF&style=for-the-badge" alt="views" />
</div>
