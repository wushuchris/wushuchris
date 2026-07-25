## Hi, I’m Christopher Mendoza (he/him) 👋

I’m an investor and applied AI builder based in San Diego, CA. I lead research at an institutional money manager and I recently completed my **M.S. in Applied Artificial Intelligence** at the University of San Diego. I like turning messy, real-world problems into working prototypes: clear objective, clean data, measurable evaluation, and a deployable workflow.

## Focus Areas

- Real-time AI systems (IoT telemetry, decision engines, LLM integration)  
- Applied machine learning (classification, forecasting, NLP, computer vision)  
- AI-driven decision support systems (finance, strategy, analytics)  
- MLOps and production workflows (reproducibility, monitoring, CI/CD)  
- Agent-based AI workflows (retrieval, structured outputs, evaluation)  

## 🎓 Education

**M.S. Applied Artificial Intelligence** — University of San Diego  

**MBA, International Business & Finance** — Rollins College

**B.S. Finance** — University of Florida  
*Minor in Economics*

---

## 🚀 Featured Projects

---

### 🏎️ F1 AI Strategy Advisor – IoT + AI Decision System
- **Goal:** Build a real-time race strategy system using simulated IoT telemetry and AI-driven decision-making  
- **Approach:** Developed a modular pipeline combining telemetry simulation, rule-based strategy logic, and LLM-powered recommendations using Hugging Face  
- **Outcome:** Delivered a cloud-deployed interactive dashboard that generates context-aware race strategies based on live telemetry and historical trends  
- **Tech:** Python, Streamlit, pandas, Hugging Face (Llama 3), time-series simulation  
- **Repo:** https://github.com/wushuchris/f1-ai-strategy-advisor  
- **Focus:** Real-time AI systems, IoT simulation, hybrid decision engines
- **Live App:** https://f1-ai-strategy-advisor-ekkzao7ckhtbv3sfh5v4nd.streamlit.app/ 

---

### 🧠 **CKD Interpretable AI – Chronic Kidney Disease Prediction**

- **Goal:** Build a machine learning system to predict Chronic Kidney Disease using clinical laboratory measurements while maintaining model transparency through explainable AI.
- **Approach:** Performed full data science workflow including data auditing, cleaning, exploratory analysis, supervised learning (Logistic Regression, Random Forest, Gradient Boosting), and SHAP-based interpretability.
- **Outcome:** Developed a highly accurate CKD prediction model (Random Forest ROC-AUC = 1.0) and applied SHAP explainability to identify medically relevant predictors such as hemoglobin, packed cell volume, and kidney filtration rate.
- **Tech:** Python, pandas, scikit-learn, NumPy, SHAP, matplotlib, seaborn, Jupyter
- **Repo:** https://github.com/wushuchris/ckd-interpretable-ai
- Focus: Interpretable AI for healthcare decision support

---

### 🧠 BeautyScoreCV – Computer Vision Regression

- **Goal:** Build an exploratory computer vision pipeline to predict a continuous aesthetic score from facial images.
- **Approach:** Image preprocessing and CNN-based feature learning to map facial images to a numeric regression target.
- **Outcome:** Delivered an end-to-end CV regression prototype demonstrating image-to-continuous-target modeling, with documented limitations around subjectivity and dataset bias.
- **Tech:** Python, Jupyter, NumPy, pandas, OpenCV, TensorFlow / PyTorch
- **Repo:** https://github.com/wushuchris/beautyscorecv

---

### 🧠 Sex Classification ML – Supervised Binary Classification

- **Goal:** Train and evaluate a binary classifier to predict sex from structured input features.
- **Approach:** Data preprocessing, feature engineering, model training, and evaluation using standard supervised learning techniques.
- **Outcome:** Produced a fully evaluated binary classification pipeline with interpretable metrics including accuracy, confusion matrix, and ROC analysis.
- **Tech:** Python, scikit-learn, pandas, Jupyter
- **Repo:** https://github.com/wushuchris/sexclassifyML

---

### 🧠 AI Values Discovery Assistant — AI-Powered Reflection Tool

- Goal: Build an interactive AI application that helps users identify core values and generate a structured personal values statement  
- Approach: Designed a multi-step workflow capturing user inputs (values, motivations, decisions, behaviors) and applied prompt engineering to synthesize responses using a Hugging Face LLM  
- Outcome: Delivered a cloud-deployed Streamlit app that generates clear, personalized values statements in real time  
- Tech: Python, Streamlit, Hugging Face, prompt engineering  
- Repo: https://github.com/wushuchris/ai-values-discovery-assistant  
- Focus: Human-centered AI, decision support systems, structured prompting  
- Live App: https://ai-values-discovery-assistant-bqfylytoes3jnzynziycue.streamlit.app

---

## 🧠 30 Agents for AI Engineers

A portfolio-building series where I design, build, evaluate, and document 30 practical AI agents. Each project focuses on a different agent engineering pattern, including structured outputs, tool use, retrieval, memory, planning, guardrails, evaluation, and deployment.

### 01. Autonomous Decision-Making Agent — Bounded Decision System

- **Goal:** Build an autonomous agent that evaluates context and recommends a bounded next action.
- **Agent Pattern:** Bounded decision-making, rule-based scoring, structured outputs, guardrail review, and auditable decision logs.
- **Implementation:** Combined rule-based scoring, Pydantic schemas, Hugging Face LLM explanations, guardrail checks, batch processing, and JSON/CSV logging.
- **Outcome:** Delivered a GitHub-ready agent project using the pattern: **Rules decide. The LLM explains. Guardrails review.**
- **Tech Stack:** Python, Pydantic, pandas, matplotlib, Hugging Face Inference Providers, OpenAI-compatible API client
- **Repo:** [GitHub Repository](https://github.com/wushuchris/01-autonomous-decision-agent)
- **Focus:** Agent engineering, bounded autonomy, structured outputs, guardrails, evaluation

---

### 02. Planning Agent — Search and Rescue Mission Planner

- **Goal:** Build a planning agent that decomposes a high-level objective into a structured, human-in-the-loop execution plan.
- **Agent Pattern:** Planning, task decomposition, dependency mapping, risk-aware sequencing, assumptions, checkpoints, and next-best-action generation.
- **Implementation:** Created a search and rescue mission planning assistant that converts rescue intent into structured mission phases, asset allocation, risk assessment, human approval checkpoints, and safe response recommendations.
- **Outcome:** Deployed a working Hugging Face Space that demonstrates how a planning agent can turn ambiguous user intent into an organized, safety-focused plan for humanitarian and emergency-response scenarios.
- **Tech Stack:** Python, Streamlit, Hugging Face Inference API, Qwen/Qwen2.5-7B-Instruct
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/search-and-rescue-mission-planner) *(Hugging Face login required)*
- **Code:** Private repository; happy to provide a walkthrough or selected excerpts upon request
- **Focus:** Planning agents, task decomposition, human-in-the-loop oversight, safety constraints, mission planning

---

### 03. Memory-Augmented Agent — Personal Project Memory Assistant

- **Goal:** Build an agent that uses persistent memory and context recall to support an ongoing project.
- **Agent Pattern:** Memory-augmented retrieval, episodic memory, semantic memory, context compression, memory write policy, and auditable memory logs.
- **Implementation:** Created a project memory assistant that stores structured memories, embeds them with sentence-transformers, retrieves relevant prior context using cosine similarity, separates semantic and episodic memory, compresses retrieved context, generates a memory-informed response, and decides whether new information should be saved.
- **Outcome:** Deployed a working Hugging Face Space that demonstrates persistent project memory, visible memory retrieval, context compression, session learning, saved-memory inspection, and audit logging.
- **Tech Stack:** Python, Pydantic, pandas, sentence-transformers, scikit-learn, Gradio, Hugging Face Spaces
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/03-memory-augmented-agent)
- **Repo:** [GitHub Repository](https://github.com/wushuchris/03-memory-augmented-agent)
- **Focus:** memory-augmented agents, retrieval, context recall, semantic memory, episodic memory, context compression, agent auditability

---

### 04. Knowledge Retrieval Agent — Source-Cited RAG Assistant

A retrieval-augmented generation agent that answers questions from a private document collection using chunking, embeddings, hybrid vector/keyword retrieval, source citations, and evidence-grounded responses.

- **Goal:** Build a source-cited knowledge assistant that retrieves relevant evidence before answering.
- **Approach:** Combined markdown/text ingestion, overlapping chunking, sentence-transformer embeddings, BM25 keyword scoring, hybrid retrieval ranking, cited evidence panels, and confidence-labeled extractive answers.
- **Outcome:** Delivered a GitHub-ready and Hugging Face-deployed RAG agent using the pattern: Retrieve first. Answer second. Cite always.
- **Tech:** Python, Streamlit, sentence-transformers, scikit-learn, rank-bm25, Docker, GitHub Actions, Hugging Face Spaces
- **Repo:** https://github.com/wushuchris/04-knowledge-retrieval-agent
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/04-knowledge-retrieval-agent)
- **Focus:** RAG, retrieval quality, source grounding, citation discipline, evidence ranking, deployment workflow

---

### 05. Document Intelligence Agent — Structured PDF Intelligence System

- **Goal:** Build a document intelligence agent that converts PDFs and text files into structured summaries, searchable chunks, and exportable data.
- **Approach:** Combined PyMuPDF document parsing, Pydantic schemas, page-aware chunking, lightweight local extraction rules, keyword search, Streamlit UI, Docker deployment, and JSON/CSV export workflows.
- **Outcome:** Delivered a GitHub-ready and Hugging Face-deployed document intelligence prototype using the pattern: Parse → Structure → Validate → Search → Export.
- **Tech:** Python, Streamlit, PyMuPDF, Pydantic, pandas, Docker, GitHub Actions, Hugging Face Spaces
- **Repo:** https://github.com/wushuchris/05-document-intelligence-agent
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/05-document-intelligence-agent)
- **Focus:** Document intelligence, PDF parsing, structured extraction, schema validation, searchable chunks, auditable outputs

---

### 06. Verification, Validation, and Evidence Agent — Auditable Claim Verification System

- **Goal:** Build an agent that audits AI-generated claims against supplied evidence and identifies when human review is required.
- **Approach:** Combined deterministic claim extraction, semantic and lexical evidence matching, citation-aware ranking, rule-based verification, contradiction detection, confidence scoring, human-review escalation, and JSON/CSV/Markdown audit exports.
- **Outcome:** Delivered a GitHub-ready and Hugging Face-deployed verification agent that classifies claims as supported, partially supported, unsupported, contradicted, or not verifiable. The project passed 16 automated tests and all 6 synthetic evaluation cases.
- **Tech:** Python, Gradio, Pydantic, sentence-transformers, scikit-learn, pandas, pytest, GitHub Actions, Hugging Face Spaces
- **Repo:** [GitHub Repository](https://github.com/wushuchris/06-verification-validation-evidence-agent)
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/06-verification-validation-evidence-agent)
- **Focus:** AI verification, evidence grounding, contradiction detection, citation validation, deterministic guardrails, human-in-the-loop review, auditable outputs

---

## Languages & Tools

**Core:** Python, pandas, scikit-learn, PyTorch/TensorFlow  
**AI & LLM:** Hugging Face, LLM APIs  
**Applications:** Streamlit, Jupyter  
**Data & Cloud:** SQL, AWS  
**DevOps:** GitHub Actions

---
