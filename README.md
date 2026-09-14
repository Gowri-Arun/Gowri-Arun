<h1 align="center">Hi, I'm Gowri Arun 👋🏽</h1>

<p align="center">
  <b>Computer Science @ IIIT Kottayam · AI/ML · Software Engineering</b>
</p>

<p align="center">
  I like working on problems where there is something interesting to figure out -  not just another interface to build or model to fine-tune.
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

I'm a third-year Computer Science student at **IIIT Kottayam**.

Most of what I build falls somewhere between **ML research and software engineering**. I've worked on adaptive systems that learn from user behaviour, passive network threat detection, visible–infrared person re-identification, knowledge graphs + RAG, and a slightly unreasonable number of ML experiments.

I enjoy the parts of a project where things are still uncertain: figuring out what to measure, designing an experiment, tracing why a model behaves differently, or turning something that works in a notebook into an actual system.

These days, that usually means some combination of **Python, PyTorch, FastAPI, React, databases, Docker, and many terminal tabs**.

---

## 🚀 Selected Projects

| Project                | What I worked on                                                                                                                                                       | Link                                                              |
| ---------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| 🧠 **NeuroBridge**     | Built the **support + learning layer** behind its adaptive loop — persistence, reflection/memory, outcome tracking, and user-specific adaptation across support tools. | [Repository](https://github.com/Civora-Forge/NeuroBridge)         |
| 🛰️ **Astra-Q**        | Worked on the **backend retrieval architecture**, combining Neo4j knowledge graphs with RAG and vector search to ground queries over ISRO MOSDAC workflows.            | [Repository](https://github.com/Gowri-Arun/Astra_Q_Backend_fork)  |
| 🛡️ **Aegis**          | Building the **traffic → features** side of passive threat detection: attack simulation and behavioural feature engineering for ML over mirrored network traffic.      | Private repository                                                |
| 🛡️ **Vanta AI**       | Built the **deepfake detection pipeline end-to-end** — React image handling → FastAPI → SigLIP/PyTorch inference → confidence results.                                 | [Repository](https://github.com/AnitaGeorge404/VantaAI)           |
| 👁️ **ST-HF VVI-ReID** | Researching **visible ↔ infrared person Re-ID**, working on cross-modal representations and evaluating retrieval with mAP and Rank-1.                                  | [Repository](https://github.com/Gowri-Arun/ST-HF-VVI-ReID)        |
| 🔬 **ToN-IoT IDS**     | Explored **rare-class intrusion detection** under severe class imbalance, using imbalance-aware sampling and ML to improve minority-attack detection.                  | [Repository](https://github.com/Gowri-Arun/ToN-IoT-rareclass-IDS) |

### 🧠 NeuroBridge — Adaptive Neuro-Inclusive Support Platform

NeuroBridge started from a fairly simple question: **can a support system actually learn what works for an individual instead of repeatedly giving everyone the same advice?**

I worked on the **support and learning layer** of the system — recording intervention outcomes, reflection and memory, persisting evidence, and feeding that history back into future adaptations.

For example, Focus Sessions can learn which session lengths actually work better for a user, while Task Breakdown can adapt the size of future plans from previous completion behaviour. The important part for me was making that a real closed loop rather than a hardcoded recommendation disguised as personalization.

```text
Context → Support → Observe → Learn → Adapt
```

🏆 **Runner-Up — Girlathon 2026**

`React` `Supabase` `PostgreSQL` `Adaptive Systems` `RLS` `Testing`

---

### 🛰️ Astra-Q — Knowledge Graph + RAG Assistant

Astra-Q explores using **knowledge graphs + retrieval** to make scientific-data discovery less painful across **ISRO MOSDAC workflows**.

I worked across the backend retrieval pipeline, using **Neo4j/Cypher for structured relationships** and **FAISS + LangChain + Gemini** for retrieval and generation.

What interested me here was grounding the answer in both structured relationships and retrieved context rather than treating RAG as simply “put documents in a vector database and ask an LLM.”

`Python` `Neo4j` `Cypher` `LangChain` `FAISS` `Gemini` `RAG`

---

### 🛡️ Aegis — Passive AI/ML Network Threat Detection

Aegis is a network-security system built around a constraint I found particularly interesting: **detect threats without actively interacting with the network at all**.

The system works from mirrored traffic. My part has involved generating attack traffic and building the feature-engineering pipeline that converts raw network behaviour into useful ML signals.

That includes SYN/UDP floods, port scans and DNS-based threats, along with features such as traffic rates, fan-in/fan-out, entropy, inter-arrival statistics, connection frequency and periodicity.

```text
Mirrored Traffic → Behavioural Features → ML → Threat Analysis
```

`Python` `Zeek` `Kafka` `Docker` `Network Security` `Feature Engineering`

---

### 🛡️ Vanta AI — Digital Safety Platform for Women

Vanta was one of the first projects where I built an ML feature **all the way from the UI to inference**.

I built the image deepfake-classification prototype: React handles image selection, previews and multipart upload; a FastAPI service preprocesses the image and runs a **Hugging Face SigLIP classifier through PyTorch**; the prediction and confidence score then flow back into the interface.

I also built the project's browser-based legal Q&A interface and FIR draft-generation workflow.

🏆 **Runner-Up — Girlathon 2025**

`React` `FastAPI` `PyTorch` `Hugging Face Transformers` `SigLIP` `Pillow`

---

### 👁️ ST-HF VVI-ReID — Visible–Infrared Person Re-Identification

This is my current computer-vision research work around a problem that sounds simple until you look at the images: **matching the same person between visible and infrared cameras**.

Because colour and appearance cues change dramatically across modalities, the interesting part is learning representations that preserve identity despite that shift.

I'm working on **video-based visible–infrared ReID** and evaluating retrieval using standard metrics such as **mAP and Rank-1**.

`PyTorch` `ResNet-50` `Computer Vision` `Deep Learning` `Person Re-ID`

---

### 🔬 ToN-IoT IDS — Rare-Class Intrusion Detection

This project is where I became particularly interested in the fact that **accuracy can tell a very misleading story in cybersecurity ML**.

The problem was rare attack detection in heavily imbalanced IoT traffic: a model can perform extremely well overall while doing badly on exactly the attacks we care about.

I experimented with imbalance-aware approaches including **KMeansSMOTE, LightGBM and XGBoost**, focusing on improving minority-attack detection rather than optimizing headline accuracy alone.

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

## 🔭 What I'm Exploring Now

Right now I'm spending most of my time around **adaptive AI, cybersecurity ML and computer vision**.

I'm especially interested in systems that have some feedback loop or difficult evaluation problem hiding underneath them — personalization from actual outcomes, learning under extreme class imbalance, passive behavioural modelling, cross-modal retrieval, or figuring out whether an apparent ML improvement survives a proper experiment.

On the engineering side, I want to get better at taking these ideas beyond experiments: **cleaner architectures, stronger backends, real deployment, and systems people can actually use**.

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
