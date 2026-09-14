<h1 align="center">Hi, I'm Gowri Arun 👋🏽</h1>

<p align="center">
  <b>Applied Machine Learning · AI Systems · Software Engineering</b>
</p>

<p align="center">
  Computer Science @ IIIT Kottayam · working across adaptive AI, cybersecurity ML, computer vision, and retrieval systems.
</p>

<p align="center">
  <a href="https://gowri-arun-portfolio.vercel.app/">
    <img src="https://img.shields.io/badge/Portfolio-FF7139?style=for-the-badge&logo=firefox-browser&logoColor=white" alt="Portfolio" />
  </a>
  <a href="https://www.linkedin.com/in/gowri-arun-/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:gowriarun2006@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
</p>

---

## 👩🏽‍💻 About Me

I'm a third-year Computer Science student at **IIIT Kottayam**, primarily interested in **applied machine learning and the systems around it**.

My recent work spans fairly different problem domains, but usually involves more than training a model in isolation:

* 🧠 **Adaptive AI** — persistent user models, outcome tracking, reflection/memory, and feedback-driven personalization
* 🛡️ **Cybersecurity ML** — passive traffic analysis, behavioural feature engineering, class imbalance, and intrusion detection
* 👁️ **Computer Vision** — visible–infrared person re-identification and image deepfake classification
* 🛰️ **Retrieval Systems** — knowledge graphs, vector retrieval, and RAG over scientific data
* ⚙️ **ML Systems** — inference APIs, persistence layers, data pipelines, testing, and frontend integration

I particularly enjoy projects where I can work across both the **experimental and engineering sides of ML** — from designing features or evaluating model behaviour to building the backend and infrastructure needed to turn the result into a working system.

---

## 🚀 Selected Projects

| Project                | What I worked on                                                                                                                                                       | Link                                                              |
| ---------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| 🧠 **NeuroBridge**     | Built the **support + learning layer** behind its adaptive loop — persistence, reflection/memory, outcome tracking, and user-specific adaptation across support tools. | [Repository](https://github.com/Civora-Forge/NeuroBridge)         |
| 🛰️ **Astra-Q**        | Worked on the **backend retrieval architecture**, combining Neo4j knowledge graphs with RAG and vector search to ground queries over ISRO MOSDAC workflows.            | [Repository](https://github.com/Gowri-Arun/Astra_Q_Backend_fork)  |
| 🛡️ **Aegis**          | Building the **traffic → features** side of passive threat detection: attack simulation and behavioural feature engineering for ML over mirrored network traffic.      | Private repository                                                |
| 🛡️ **Vanta AI**       | Built the **deepfake detection pipeline end-to-end** — React image handling → FastAPI → SigLIP/PyTorch inference → confidence results.                                 | [Repository](https://github.com/AnitaGeorge404/VantaAI)           |
| 👁️ **ST-HF VVI-ReID** | Researching **visible ↔ infrared person Re-ID**, working on cross-modal representations and evaluating retrieval with mAP and Rank-1.                                  | [Repository](https://github.com/Gowri-Arun/ST-HF-VVI-ReID)        |
| 🔬 **ToN-IoT IDS**     | Explored **rare-class intrusion detection** under severe class imbalance using imbalance-aware sampling and ML for minority-attack detection.                          | [Repository](https://github.com/Gowri-Arun/ToN-IoT-rareclass-IDS) |

### 🧠 NeuroBridge — Adaptive Neuro-Inclusive Support Platform

NeuroBridge is a neuro-inclusive support platform with a **closed adaptive loop** for learning which interventions work better for an individual over time.

My work focuses on the **support and learning layer**: intervention lifecycle tracking, outcome capture, reflection and memory, persistent user-specific evidence, and adaptation of future recommendations.

Built persistence and learning workflows around **Task Breakdown** and **Focus Sessions**. For example, Focus Sessions can learn preferred session duration from completion and abandonment history, while Task Breakdown can adapt future plan size from previous completion behaviour.

```text id="yhl88n"
Context → Support → Observe → Learn → Adapt
```

The persistence layer uses **Supabase/PostgreSQL with row-level security**, with repository abstractions and local fallback paths for support evidence and memory.

🏆 **Runner-Up — Girlathon 2026**

`React` `Supabase` `PostgreSQL` `Adaptive Systems` `RLS` `Testing`

---

### 🛰️ Astra-Q — Knowledge Graph + RAG Assistant

Astra-Q is a knowledge-grounded assistant for **ISRO MOSDAC scientific-data workflows**, combining graph-based knowledge representation with retrieval-augmented generation.

Worked on the backend retrieval architecture using **Neo4j and Cypher** for structured relationships and **FAISS/LangChain** for vector retrieval, integrating retrieved context with Gemini for grounded responses.

The system combines structured graph traversal with semantic retrieval rather than relying solely on unconstrained LLM generation.

`Python` `Neo4j` `Cypher` `LangChain` `FAISS` `Gemini` `RAG`

---

### 🛡️ Aegis — Passive AI/ML Network Threat Detection

Aegis is a passive network-security pipeline designed to detect suspicious behaviour from **mirrored network traffic without active probing or mitigation**.

My work covers attack simulation and the **traffic feature-engineering pipeline**. I implemented traffic generation for **SYN floods, UDP floods, port scans, and DNS-based threats**, then derived behavioural features for downstream detection.

Features include **packet and byte rates, fan-in/fan-out, unique destination counts, inter-arrival-time statistics, connection frequency, source-IP entropy, and periodicity**.

```text id="8u6tmr"
Mirrored Traffic → Passive Capture → Behavioural Features → ML Detection
```

The wider architecture uses **Zeek for network telemetry, Kafka for streaming, and Docker for the isolated traffic lab**.

`Python` `Zeek` `Kafka` `Docker` `Network Security` `Feature Engineering` `ML`

---

### 🛡️ Vanta AI — Digital Safety Platform for Women

Vanta AI is a digital-safety platform addressing image-based abuse through detection, legal guidance, reporting, and support tools.

I built the **image deepfake-classification prototype end-to-end**. The React frontend handles drag-and-drop image selection, local previews, loading/error state, multipart upload, and result rendering.

On the backend, I implemented a **FastAPI inference endpoint** that converts uploaded images to RGB, preprocesses them with a Hugging Face image processor, runs a **SigLIP image-classification model with PyTorch**, applies softmax to the logits, and returns the classification and confidence score.

I also implemented the project's **browser-based legal Q&A interface** and **FIR draft generator**, including validation, generated previews, editing/reset flows, and browser-based text export.

🏆 **Runner-Up — Girlathon 2025**

`React` `FastAPI` `PyTorch` `Hugging Face Transformers` `SigLIP` `Pillow` `Fetch API`

---

### 👁️ ST-HF VVI-ReID — Visible–Infrared Person Re-Identification

Research project on **video-based visible–infrared person re-identification**, where identity has to be preserved across cameras operating in substantially different visual modalities.

The work focuses on **cross-modal representation learning** for matching visible and infrared observations of the same identity despite the modality gap.

Performance is evaluated using standard person-ReID retrieval metrics including **mean Average Precision (mAP) and Rank-1 accuracy**.

`PyTorch` `ResNet-50` `Computer Vision` `Deep Learning` `Person Re-ID`

---

### 🔬 ToN-IoT IDS — Rare-Class Intrusion Detection

Intrusion-detection research focused on **rare attack detection under severe class imbalance** in IoT network traffic.

The central problem is minority-class performance: aggregate accuracy can remain high while rare attacks are poorly detected.

Experimented with **KMeansSMOTE and tree-based models including LightGBM and XGBoost** to improve minority-attack detection under the imbalanced ToN-IoT distribution.

`LightGBM` `XGBoost` `KMeansSMOTE` `scikit-learn` `Cybersecurity ML`

---

## 🧰 Tech Stack

### Languages

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/C++-00599C?style=flat&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL-4479A1?style=flat&logo=mysql&logoColor=white" />
</p>

### Machine Learning & AI

<p>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white" />
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white" />
  <img src="https://img.shields.io/badge/XGBoost-EB5B28?style=flat" />
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=chainlink&logoColor=white" />
  <img src="https://img.shields.io/badge/FAISS-111827?style=flat&logo=meta&logoColor=white" />
</p>

### Backend & Data

<p>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Supabase-3FCF8E?style=flat&logo=supabase&logoColor=white" />
  <img src="https://img.shields.io/badge/Neo4j-4581C3?style=flat&logo=neo4j&logoColor=white" />
  <img src="https://img.shields.io/badge/DuckDB-FFF000?style=flat&logo=duckdb&logoColor=black" />
</p>

### Frontend & Infrastructure

<p>
  <img src="https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Apache_Kafka-231F20?style=flat&logo=apachekafka&logoColor=white" />
  <img src="https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black" />
</p>

---

## 🔭 Current Focus

I'm currently interested in:

* **Adaptive AI** — persistent user modelling, outcome-driven personalization, and feedback loops
* **Cybersecurity ML** — passive traffic analysis, behavioural feature engineering, imbalanced classification, and explainability
* **Computer Vision** — cross-modal representation learning and person re-identification
* **ML Experimentation** — ablation studies, leakage-aware evaluation, reproducibility, and robust validation
* **AI Systems Engineering** — inference pipelines, retrieval infrastructure, APIs, persistence, testing, and deployment

---

## 📊 GitHub

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Gowri-Arun&show_icons=true&theme=github_dark&hide_border=true&card_width=480" alt="GitHub Stats" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Gowri-Arun&layout=compact&theme=github_dark&hide_border=true&card_width=480" alt="Top Languages" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Gowri-Arun&theme=github-dark-blue&hide_border=true" alt="GitHub Streak" />
</p>

---

## 📈 Activity

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Gowri-Arun&bg_color=0d1117&color=58a6ff&line=7ee787&point=f78166&area=true&hide_border=true" width="100%" alt="GitHub Activity Graph" />
</p>

---

## 🤝 Connect

<p align="center">
  <a href="https://gowri-arun-portfolio.vercel.app/">
    <img src="https://img.shields.io/badge/Portfolio-FF7139?style=for-the-badge&logo=firefox-browser&logoColor=white" />
  </a>
  <a href="https://www.linkedin.com/in/gowri-arun-/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:gowriarun2006@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake-dark.svg" width="100%" alt="Contribution Snake" />
</p>
