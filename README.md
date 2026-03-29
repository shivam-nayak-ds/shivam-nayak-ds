<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Shivam Nayak — GitHub Profile</title>
<link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;500&family=Sora:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    background: #010409;
    color: #e6edf3;
    font-family: 'Sora', sans-serif;
    font-size: 14px;
    line-height: 1.6;
    padding: 24px 16px;
  }

  .gh-card {
    background: #0d1117;
    border: 1px solid #30363d;
    border-radius: 12px;
    max-width: 880px;
    margin: 0 auto;
    overflow: hidden;
  }

  .banner img { width: 100%; display: block; }

  .gh-header {
    background: #161b22;
    border-bottom: 1px solid #30363d;
    padding: 20px 28px;
  }
  .header-top {
    display: flex; align-items: center;
    gap: 14px; margin-bottom: 16px;
  }
  .avatar {
    width: 56px; height: 56px; border-radius: 50%;
    background: linear-gradient(135deg, #1D9E75, #7F77DD);
    display: flex; align-items: center; justify-content: center;
    font-size: 20px; font-weight: 600; color: #fff; flex-shrink: 0;
  }
  .user-info h1 { font-size: 18px; font-weight: 600; color: #e6edf3; }
  .user-info p  { font-size: 12px; color: #7d8590; font-family: 'JetBrains Mono', monospace; margin-top: 2px; }

  .social-links { display: flex; gap: 6px; flex-wrap: wrap; }
  .social-badge {
    display: inline-flex; align-items: center; gap: 5px;
    padding: 5px 12px; border-radius: 6px;
    font-size: 11px; font-weight: 500;
    text-decoration: none; border: 1px solid;
    font-family: 'JetBrains Mono', monospace;
    transition: opacity .15s;
  }
  .social-badge:hover { opacity: .8; }
  .badge-li { background: #0a66c2;   color: #fff;    border-color: #0a66c2; }
  .badge-gm { background: #1e2a1e;   color: #4CAF50; border-color: #238636; }
  .badge-hf { background: #2d2a1a;   color: #FFD21E; border-color: #3d3a20; }
  .badge-pt { background: #1a1a2e;   color: #a78bfa; border-color: #2d2a40; }

  .content { padding: 24px 28px; }
  .section  { margin-bottom: 26px; }

  .section-title {
    font-size: 14px; font-weight: 600; color: #e6edf3;
    margin-bottom: 14px;
    display: flex; align-items: center; gap: 6px;
    border-bottom: 1px solid #21262d; padding-bottom: 8px;
  }

  .about-grid { display: grid; gap: 7px; }
  .about-item {
    display: flex; align-items: flex-start; gap: 8px;
    font-size: 13px; color: #8b949e; line-height: 1.5;
  }
  .about-icon { font-size: 14px; flex-shrink: 0; margin-top: 1px; }

  .badge-group { margin-bottom: 12px; }
  .badge-group-title {
    font-size: 10px; color: #7d8590;
    font-family: 'JetBrains Mono', monospace;
    margin-bottom: 6px;
    text-transform: uppercase; letter-spacing: .6px;
  }
  .badges { display: flex; flex-wrap: wrap; gap: 5px; }
  .badge  {
    display: inline-flex; align-items: center; gap: 4px;
    padding: 3px 9px; border-radius: 4px;
    font-size: 11px; font-weight: 500;
    font-family: 'JetBrains Mono', monospace; border: 1px solid;
  }
  .b-py { background:#1e3a5f; color:#79c0ff; border-color:#1e4a7a; }
  .b-sk { background:#3d2a0a; color:#f0883e; border-color:#5a3d12; }
  .b-xg { background:#2d1a0a; color:#ff7b72; border-color:#4a2810; }
  .b-tf { background:#3d2200; color:#ffa657; border-color:#5a3300; }
  .b-lc { background:#1a2a2a; color:#56d364; border-color:#1f3a3a; }
  .b-hf { background:#2d2a00; color:#f0e040; border-color:#3d3a00; }
  .b-ml { background:#0e2a4a; color:#58a6ff; border-color:#0e3a6a; }
  .b-dv { background:#2a1a3d; color:#c084fc; border-color:#3a2a55; }
  .b-dk { background:#0e1e3d; color:#60a5fa; border-color:#0e2a55; }
  .b-fa { background:#0d2010; color:#4ade80; border-color:#0d3015; }
  .b-ev { background:#3d0e0e; color:#f87171; border-color:#5a1515; }
  .b-gi { background:#1a2a1a; color:#56d364; border-color:#1f3a1f; }
  .b-ge { background:#0e1e3d; color:#7dd3fc; border-color:#0e2a55; }

  .project-card {
    background: #161b22; border: 1px solid #21262d;
    border-radius: 8px; padding: 16px 18px;
    margin-bottom: 12px; transition: border-color .2s;
  }
  .project-card:hover { border-color: #58a6ff; }
  .project-header {
    display: flex; align-items: flex-start;
    justify-content: space-between; gap: 8px; margin-bottom: 7px;
  }
  .project-name { font-size: 14px; font-weight: 600; color: #58a6ff; }
  .project-status {
    font-size: 10px; padding: 2px 9px; border-radius: 12px;
    font-family: 'JetBrains Mono', monospace; font-weight: 500;
    flex-shrink: 0; border: 1px solid;
  }
  .status-live { background:#0a2a0a; color:#56d364; border-color:#238636; }
  .status-wip  { background:#2a1a00; color:#ffa657; border-color:#3d2200; }
  .project-desc   { font-size: 12px; color: #7d8590; margin-bottom: 10px; line-height: 1.55; }
  .project-badges { display: flex; flex-wrap: wrap; gap: 4px; margin-bottom: 10px; }
  .project-links  { display: flex; gap: 12px; }
  .proj-link {
    font-size: 11px; color: #58a6ff; text-decoration: none;
    display: flex; align-items: center; gap: 3px;
    opacity: .8; font-family: 'JetBrains Mono', monospace;
  }
  .proj-link:hover { opacity: 1; }

  .stats-grid { display: grid; grid-template-columns: repeat(3,1fr); gap: 10px; }
  .stat-card {
    background: #161b22; border: 1px solid #21262d;
    border-radius: 8px; padding: 14px; text-align: center;
  }
  .stat-num   { font-size: 26px; font-weight: 600; font-family: 'JetBrains Mono', monospace; }
  .stat-label { font-size: 11px; color: #7d8590; margin-top: 3px; }

  .code-block {
    background: #161b22; border: 1px solid #21262d;
    border-radius: 8px; padding: 16px 18px;
    font-family: 'JetBrains Mono', monospace;
    font-size: 12px; line-height: 1.8;
  }
  .c-kw  { color: #ff7b72; }
  .c-str { color: #a5d6ff; }
  .c-val { color: #79c0ff; }
  .c-br  { color: #e6edf3; }

  .concepts-wrap { display: flex; flex-wrap: wrap; gap: 6px; }
  .concept-tag {
    background: #1c2128; border: 1px solid #30363d;
    border-radius: 20px; padding: 3px 11px;
    font-size: 11px; color: #8b949e;
    font-family: 'JetBrains Mono', monospace;
  }

  .divider { border: none; border-top: 1px solid #21262d; margin: 22px 0; }

  .footer {
    text-align: center; padding: 18px 28px;
    border-top: 1px solid #21262d;
    font-size: 12px; color: #7d8590; font-style: italic;
  }
  .footer small { font-size: 10px; color: #484f58; display: block; margin-top: 4px; }
</style>
</head>
<body>

<div class="gh-card">

  <!-- Banner -->
  <div class="banner">
    <img src="https://github.com/shivam-nayak-ds/shivam-nayak-ds/blob/main/Blue%20Beige%20Aesthetic%20Music%20Channel%20YouTube%20Banner.png" alt="Shivam Nayak Banner" />
  </div>

  <!-- Header -->
  <div class="gh-header">
    <div class="header-top">
      <div class="avatar">SN</div>
      <div class="user-info">
        <h1>Shivam Nayak</h1>
        <p>AI/ML Engineer · GenAI · MLOps · End-to-End ML Systems</p>
      </div>
    </div>
    <div class="social-links">
      <a class="social-badge badge-li" href="YOUR_LINKEDIN_URL">🔗 LinkedIn</a>
      <a class="social-badge badge-gm" href="mailto:YOUR_EMAIL">📧 Gmail</a>
      <a class="social-badge badge-hf" href="YOUR_HUGGINGFACE_URL">🤗 HuggingFace</a>
      <a class="social-badge badge-pt" href="#">🌐 Portfolio</a>
    </div>
  </div>

  <div class="content">

    <!-- About -->
    <div class="section">
      <div class="section-title">🧠 About Me</div>
      <div class="about-grid">
        <div class="about-item"><span class="about-icon">🔭</span><span>Building <strong style="color:#e6edf3">production-ready ML systems</strong> — fraud detection, RAG pipelines, MLOps workflows</span></div>
        <div class="about-item"><span class="about-icon">🤖</span><span>Specializing in <strong style="color:#e6edf3">Generative AI</strong> — LangChain, RAG, Vector Databases, LLM chaining</span></div>
        <div class="about-item"><span class="about-icon">⚙️</span><span>MLOps-first mindset — <strong style="color:#e6edf3">MLflow, DVC, Docker, CI/CD</strong> on every project</span></div>
        <div class="about-item"><span class="about-icon">🚀</span><span>Open to <strong style="color:#56d364">AI/ML Engineer roles</strong> (Remote / Hybrid) — targeting June 2026</span></div>
        <div class="about-item"><span class="about-icon">📍</span><span>Based in <strong style="color:#e6edf3">Bhopal, India</strong></span></div>
      </div>
    </div>

    <hr class="divider">

    <!-- Tech Stack -->
    <div class="section">
      <div class="section-title">🛠️ Tech Stack</div>

      <div class="badge-group">
        <div class="badge-group-title">Machine Learning & AI</div>
        <div class="badges">
          <span class="badge b-py">🐍 Python</span>
          <span class="badge b-sk">📊 scikit-learn</span>
          <span class="badge b-xg">⚡ XGBoost</span>
          <span class="badge b-xg">💡 LightGBM</span>
          <span class="badge b-tf">🧠 TensorFlow</span>
          <span class="badge b-tf">🔥 PyTorch</span>
          <span class="badge b-sk">🔢 NumPy</span>
          <span class="badge b-sk">🐼 Pandas</span>
          <span class="badge b-sk">📉 Matplotlib</span>
          <span class="badge b-sk">📈 Seaborn</span>
        </div>
      </div>

      <div class="badge-group">
        <div class="badge-group-title">Generative AI & LLMs</div>
        <div class="badges">
          <span class="badge b-lc">🔗 LangChain</span>
          <span class="badge b-hf">🤗 HuggingFace Transformers</span>
          <span class="badge b-ge">✨ Google Gemini</span>
          <span class="badge b-dk">🤖 OpenAI API</span>
          <span class="badge b-ml">🔍 FAISS</span>
          <span class="badge b-ev">🧬 ChromaDB</span>
          <span class="badge b-lc">🏗 RAG Architecture</span>
          <span class="badge b-hf">✍ Prompt Engineering</span>
        </div>
      </div>

      <div class="badge-group">
        <div class="badge-group-title">MLOps & Infrastructure</div>
        <div class="badges">
          <span class="badge b-ml">📊 MLflow</span>
          <span class="badge b-dv">📦 DVC</span>
          <span class="badge b-dk">🐳 Docker</span>
          <span class="badge b-gi">⚙ GitHub Actions</span>
          <span class="badge b-ev">🔍 Evidently AI</span>
          <span class="badge b-ev">📡 Prometheus</span>
          <span class="badge b-gi">🔀 Git</span>
        </div>
      </div>

      <div class="badge-group">
        <div class="badge-group-title">Backend & Deployment</div>
        <div class="badges">
          <span class="badge b-fa">⚡ FastAPI</span>
          <span class="badge b-ev">🎈 Streamlit</span>
          <span class="badge b-ml">🐬 MySQL</span>
          <span class="badge b-ml">🐘 PostgreSQL</span>
          <span class="badge b-ev">⚡ Redis</span>
          <span class="badge b-gi">🤗 HF Spaces</span>
        </div>
      </div>
    </div>

    <hr class="divider">

    <!-- Projects -->
    <div class="section">
      <div class="section-title">🚀 Featured Projects</div>

      <div class="project-card">
        <div class="project-header">
          <div class="project-name">🔍 Fraud Detection ML System</div>
          <span class="project-status status-live">✓ Deployed</span>
        </div>
        <div class="project-desc">End-to-end fraud detection on IEEE-CIS dataset (590K+ transactions). XGBoost + Random Forest with SMOTE for class imbalance. Feature selection 346→20 top features, 95%+ AUC. Production REST API via FastAPI with full src/ structure.</div>
        <div class="project-badges">
          <span class="badge b-py">Python</span>
          <span class="badge b-xg">XGBoost</span>
          <span class="badge b-sk">scikit-learn</span>
          <span class="badge b-fa">FastAPI</span>
          <span class="badge b-dk">Docker</span>
        </div>
        <div class="project-links">
          <a class="proj-link" href="https://github.com/shivam-nayak-ds/Fraud-detection-ml-system">📂 GitHub</a>
          <a class="proj-link" href="#">🎬 Demo Video</a>
        </div>
      </div>

      <div class="project-card">
        <div class="project-header">
          <div class="project-name">🤖 RAG Document Chatbot</div>
          <span class="project-status status-wip">⚡ In Progress</span>
        </div>
        <div class="project-desc">Upload any PDF → ask natural language questions → get contextual answers with source citations. LangChain + FAISS + Google Gemini Embeddings + multi-turn ConversationMemory. FastAPI backend + Streamlit UI.</div>
        <div class="project-badges">
          <span class="badge b-lc">LangChain</span>
          <span class="badge b-ml">FAISS</span>
          <span class="badge b-ge">Gemini API</span>
          <span class="badge b-fa">FastAPI</span>
          <span class="badge b-ev">Streamlit</span>
        </div>
        <div class="project-links">
          <a class="proj-link" href="#">📂 GitHub</a>
        </div>
      </div>

      <div class="project-card">
        <div class="project-header">
          <div class="project-name">📊 Customer CLV MLOps Pipeline</div>
          <span class="project-status status-live">✓ Deployed</span>
        </div>
        <div class="project-desc">Full MLOps pipeline for Customer Lifetime Value prediction. MLflow experiment tracking + model registry, scikit-learn models, FastAPI serving. Olist e-commerce dataset (100K+ orders), MySQL backend.</div>
        <div class="project-badges">
          <span class="badge b-ml">MLflow</span>
          <span class="badge b-dv">DVC</span>
          <span class="badge b-sk">scikit-learn</span>
          <span class="badge b-fa">FastAPI</span>
          <span class="badge b-ml">MySQL</span>
        </div>
        <div class="project-links">
          <a class="proj-link" href="#">📂 GitHub</a>
          <a class="proj-link" href="#">🎬 Demo Video</a>
        </div>
      </div>

      <div class="project-card">
        <div class="project-header">
          <div class="project-name">📄 AI Resume Analyzer</div>
          <span class="project-status status-live">✓ Live</span>
        </div>
        <div class="project-desc">AI-powered resume analysis — ATS score, skill gap analysis, improvement suggestions. Built with Claude API + structured prompt engineering. Single-file HTML deployment. 50+ beta users.</div>
        <div class="project-badges">
          <span class="badge b-xg">Claude API</span>
          <span class="badge b-hf">JavaScript</span>
          <span class="badge b-lc">Prompt Eng.</span>
        </div>
        <div class="project-links">
          <a class="proj-link" href="#">📂 GitHub</a>
          <a class="proj-link" href="#">🚀 Live Demo</a>
        </div>
      </div>

    </div>

    <hr class="divider">

    <!-- Stats -->
    <div class="section">
      <div class="section-title">📈 GitHub Stats</div>
      <div class="stats-grid">
        <div class="stat-card">
          <div class="stat-num" style="color:#56d364">4</div>
          <div class="stat-label">Production Projects</div>
        </div>
        <div class="stat-card">
          <div class="stat-num" style="color:#58a6ff">168</div>
          <div class="stat-label">Contributions</div>
        </div>
        <div class="stat-card">
          <div class="stat-num" style="color:#f0883e">15+</div>
          <div class="stat-label">Tools & Libraries</div>
        </div>
      </div>
    </div>

    <hr class="divider">

    <!-- Current Focus -->
    <div class="section">
      <div class="section-title">🎯 Current Focus</div>
      <div class="code-block">
        <span class="c-kw">current_focus</span> <span class="c-br">= {</span><br>
        &nbsp;&nbsp;<span class="c-str">"building"</span><span class="c-br">:</span>&nbsp;&nbsp; <span class="c-br">[</span><span class="c-val">"LangChain RAG Pipeline"</span><span class="c-br">,</span> <span class="c-val">"MLOps best practices"</span><span class="c-br">],</span><br>
        &nbsp;&nbsp;<span class="c-str">"learning"</span><span class="c-br">:</span>&nbsp;&nbsp; <span class="c-br">[</span><span class="c-val">"LLM fine-tuning"</span><span class="c-br">,</span> <span class="c-val">"Vector DB optimization"</span><span class="c-br">],</span><br>
        &nbsp;&nbsp;<span class="c-str">"dsa"</span><span class="c-br">:</span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span class="c-br">[</span><span class="c-val">"Arrays"</span><span class="c-br">,</span> <span class="c-val">"HashMap"</span><span class="c-br">,</span> <span class="c-val">"Sliding Window"</span><span class="c-br">],</span><br>
        &nbsp;&nbsp;<span class="c-str">"target"</span><span class="c-br">:</span>&nbsp;&nbsp;&nbsp; <span class="c-val">"AI/ML Engineer @ 10 LPA — June 2026"</span><br>
        <span class="c-br">}</span>
      </div>
    </div>

    <hr class="divider">

    <!-- Concepts -->
    <div class="section">
      <div class="section-title">📚 ML Concepts I Work With</div>
      <div class="concepts-wrap">
        <span class="concept-tag">Supervised Learning</span>
        <span class="concept-tag">Ensemble Methods</span>
        <span class="concept-tag">Feature Engineering</span>
        <span class="concept-tag">SMOTE / Imbalanced Data</span>
        <span class="concept-tag">Cross-Validation</span>
        <span class="concept-tag">Hyperparameter Tuning</span>
        <span class="concept-tag">RAG Architecture</span>
        <span class="concept-tag">Vector Embeddings</span>
        <span class="concept-tag">Prompt Engineering</span>
        <span class="concept-tag">LLM Chaining</span>
        <span class="concept-tag">Experiment Tracking</span>
        <span class="concept-tag">Model Versioning</span>
        <span class="concept-tag">Data Drift Detection</span>
        <span class="concept-tag">Model Monitoring</span>
        <span class="concept-tag">CI/CD for ML</span>
        <span class="concept-tag">Containerization</span>
        <span class="concept-tag">ANN / CNN / LSTM</span>
        <span class="concept-tag">NLP Pipelines</span>
      </div>
    </div>

  </div>

  <div class="footer">
    ⭐ Strong fundamentals + real projects beat fancy buzzwords ⭐
    <small>Profile views: 1,247 · Last updated: March 2026</small>
  </div>

</div>
</body>
</html>
