<div align="center">

<!-- ELITE TYPING HEADER -->
<a href="https://github.com/shivam-nayak-ds">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=38&pause=1500&color=00E5FF&center=true&vCenter=true&width=800&height=100&lines=SHIVAM+NAYAK;AI+Systems+%26+Agentic+Engineer;GenAI+%2B+Applied+ML%2FDL;0-to-1+Infrastructure+Builder" alt="Typing SVG" />
</a>

> **Bridging the gap between ML research, Agentic Intelligence, and production-grade scalable systems.** <br> Engineering deterministic workflows, autonomous research agents, low-latency voice pipelines, and self-correcting RAG systems across ML, DL, NLP, and GenAI.

<br>

<p align="center">
  <a href="https://www.linkedin.com/in/shivam-nayakk"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=101010" alt="LinkedIn" /></a>
  <a href="mailto:shivamnayak296@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white&labelColor=101010" alt="Email" /></a>
  <a href="https://github.com/shivam-nayak-ds"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white&labelColor=101010" alt="GitHub" /></a>
</p>

</div>

---

### 🧠 Core Engineering Spectrum

I build production-ready systems across the entire Artificial Intelligence stack:

*   **Agentic Systems & Multi-Agent Workflows:** Designing autonomous reasoning systems, tool-use routing, state-machine architectures with **LangGraph**, and multi-agent task execution using **CrewAI**.
*   **Self-Correcting & Advanced RAG:** Engineering resilient retrieval systems featuring semantic chunking, dynamic query re-writing, self-correction feedback loops, and cross-encoder re-ranking.
*   **Voice & Low-Latency GenAI Agents:** Building end-to-end, sub-second latency speech-to-speech AI systems integrating STT, LLM reasoning, and natural voice synthesis for domain-specific automation.
*   **End-to-End MLOps & Applied ML/DL:** Training predictive and fine-tuning open-source models (**Llama-3**, **PyTorch**), paired with automated pipelines (**MLflow**, **DVC**, **Docker**, **FastAPI**).

---

### 🏗️ Production-Grade Featured Systems

#### 1. [Asha AI – Enterprise Healthcare Voice Agent](https://github.com/shivam-nayak-ds/ai-hospital-voice-agent)
*End-to-end real-time conversational AI agent for clinical patient triage and appointment management.*
*   **Architecture:** Ultra-low latency voice pipeline (STT $\rightarrow$ Domain-Prompted LLM $\rightarrow$ TTS Engine) integrated with asynchronous backend logic.
*   **Engineering Challenge:** Minimizing latency and handling unstructured, accents, and ambiguous medical phrasing during live phone/voice interactions.
*   **Solution:** Built streaming request handlers in FastAPI with fallback intent routing, enabling near instant response loops suitable for small clinics and enterprise hospitals alike.

#### 2. [CogniFlow AI – Autonomous Deep Research Agent](https://github.com/shivam-nayak-ds/CogniFlow-AI)
*Multi-agent autonomous research engine capable of deep web exploration, citation synthesis, and report generation.*
*   **Architecture:** Stateful Multi-Agent Graph built with **LangGraph**, web search tool integration, and citation verification loops.
*   **Engineering Challenge:** Preventing infinite agent loops and eliminating hallucinated source references in deep research tasks.
*   **Solution:** Implemented deterministic self-reflection cycles and strict verification nodes that score source relevance and cross-reference citations before output rendering.

#### 3. [Finance Guard – Self-Correcting Financial RAG](https://github.com/shivam-nayak-ds)
*Hallucination-resistant RAG pipeline engineered for complex, high-precision financial domain analytics.*
*   **Architecture:** 2-Stage Hybrid Retrieval (Vector + Keyword) augmented with an active Self-Correction Evaluation loop.
*   **Engineering Challenge:** Standard RAG pipelines fail when extracting precise metrics from dense financial statements and earnings reports.
*   **Solution:** Applied continuous document routing, query re-writing, and an LLM-as-a-Judge evaluation node to re-query the vector store dynamically whenever retrieved context confidence falls below threshold.

#### 4. [RetailOps – End-to-End Sales Forecasting Pipeline](https://github.com/shivam-nayak-ds/Retail-Ops-End-to-End-Sales-Forecasting-Pipeline)
*Scalable, version-controlled MLOps architecture designed for dynamic retail inventory forecasting.*
*   **Architecture:** Modular ETL and training pipeline featuring automated data transformation, model validation, and deployment stages.
*   **Engineering Challenge:** Ensuring experiment reproducibility and tracking performance decay across seasonal data shifts.
*   **Solution:** Integrated **MLflow** for hyperparameter tracking alongside **DVC** for deterministic dataset versioning, fully packaged inside **Docker** containers.

#### 5. [Domain-Specific Llama-3 Fine-Tuning Engine](https://github.com/shivam-nayak-ds/Llama3-Domain-Specific-FineTuning)
*Efficient Parameter-Efficient Fine-Tuning (PEFT) pipeline tailored for custom domain adaptation.*
*   **Architecture:** PyTorch + Hugging Face ecosystem using **LoRA / QLoRA** to adapt Llama-3 models on specialized datasets.
*   **Engineering Challenge:** Resource-constrained GPU memory overhead during full model fine-tuning.
*   **Solution:** Applied 4-bit quantization paired with LoRA adapters, drastically reducing VRAM consumption while preserving downstream domain performance.

#### 6. [Fake Job Detection System (NLP & Fraud Analysis)](https://github.com/shivam-nayak-ds/fake-job-detection-nlp)
*Production NLP service for detecting fraudulent job postings with explicit data tracking.*
*   **Architecture:** TF-IDF + XGBoost/NLP model served behind a **FastAPI** REST interface with a **Streamlit** front-end.
*   **Engineering Challenge:** Severe dataset class imbalance leading to false negatives in deceptive text detection.
*   **Solution:** Implemented robust text pre-processing pipelines combined with DVC version control to systematically evaluate precision/recall trade-offs under high-imbalance scenarios.

---

### 🛠️ Technical Ecosystem

**Core AI / ML / DL Stack**  
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit_learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)

**GenAI, Agents & Vector Databases**  
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![CrewAI](https://img.shields.io/badge/CrewAI-FF4F00?style=flat-square)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF4F00?style=flat-square&logo=chroma&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=flat-square)

**MLOps, Backend & Systems**  
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)
![DVC](https://img.shields.io/badge/DVC-945DD6?style=flat-square&logo=dvc&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/CI/CD-2088FF?style=flat-square&logo=github-actions&logoColor=white)

---

### 📊 Engineering Analytics

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=shivam-nayak-ds&theme=tokyonight&border_radius=4&hide_border=true" width="48%" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=shivam-nayak-ds&layout=compact&theme=tokyonight&border_radius=4&hide_border=true" width="48%" />
</div>

<br>

<div align="center">
  <h3>🤝 Let's Build the Future</h3>
  <p>I am looking for AI Engineering opportunities where I can own systems end-to-end—from research and agentic workflows to low-latency production deployment.<br> <b><a href="mailto:shivamnayak296@gmail.com">Let's connect and build.</a></b></p>
</div>
