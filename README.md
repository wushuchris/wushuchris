## Hi, I’m Christopher Mendoza 👋

I’m an investor and applied AI builder based in San Diego, CA. I lead research at an institutional money manager and recently completed my **M.S. in Applied Artificial Intelligence** at the University of San Diego. I like turning messy, real-world problems into working AI systems: clear objectives, structured data and interfaces, measurable evaluation, guardrails, and deployable workflows.

**Currently building:** a 30-agent portfolio focused on practical AI engineering patterns including planning, retrieval, memory, tool use, verification, multi-agent orchestration, peer-to-peer coordination, distributed task allocation, guardrails, evaluation, and deployment.  
**Progress:** **11 of 30 agents completed.**

## Focus Areas

- Agent engineering (retrieval, memory, tool use, multi-agent orchestration, structured outputs, guardrails, evaluation)
- Real-time AI systems (IoT telemetry, decision engines, LLM integration)
- Applied machine learning (classification, forecasting, NLP, computer vision)
- AI-driven decision support systems (finance, strategy, analytics)
- MLOps and production workflows (reproducibility, monitoring, CI/CD)

## 🎓 Education

**M.S. Applied Artificial Intelligence** — University of San Diego  

**MBA, International Business & Finance** — Rollins College

**B.S. Finance** — University of Florida  
*Minor in Economics*

---

## 🧠 30 Agents for AI Engineers

A portfolio-building series where I design, build, evaluate, deploy, and document 30 practical AI agents. Each project focuses on a different agent-engineering pattern, including structured outputs, planning, memory, retrieval, verification, tool use, orchestration, guardrails, evaluation, and deployment.

Each agent is designed as a reusable engineering primitive. As the portfolio progresses, later projects increasingly compose and extend patterns established by earlier agents.

### 01. Autonomous Decision-Making Agent — Bounded Decision System

- **Goal:** Build an autonomous decision system that can recommend a bounded next action without allowing the LLM to invent the action space or bypass mandatory review.
- **Approach:** Combined typed Pydantic inputs, deterministic application-owned factor scoring, a fixed four-action set, mandatory human-review gates, real `run_decision_iter()` observability, runtime-configured Hugging Face LLM explanations, explanation publication guardrails, deterministic fallback, public-repository hygiene checks, and GitHub Actions deployment gating.
- **Outcome:** Rebuilt the original Colab-era project into a production-validated bounded-autonomy demo using the pattern: **Application code decides. The LLM explains. Guardrails decide what gets published.** The final project passed **28 automated tests** and **7/7 decision/guardrail evaluation cases**, live-validated `Qwen/Qwen3.8-27B:ovhcloud` through Hugging Face Inference Providers, preserves the application-selected action when the model fails or violates the explanation boundary, deploys from a sanitized public GitHub history, and passed final human presentation review with a centered 1080px business-first interface.
- **Tech:** Python, Pydantic, Gradio, OpenAI-compatible API client, Hugging Face Inference Providers, Qwen3.8, pytest, GitHub Actions, Hugging Face Spaces
- **Repo:** [GitHub Repository](https://github.com/wushuchris/01-autonomous-decision-agent)
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/01-autonomous-decision-agent)
- **Focus:** Bounded autonomy, deterministic decision authority, human-review gates, LLM explanation, publication guardrails, fallback behavior, runtime configuration, evaluation, public-demo hygiene, live observability

---

### 02. Planning Agent — Search and Rescue Mission Planner

- **Goal:** Build a planning agent that decomposes a high-level objective into a structured, human-in-the-loop execution plan.
- **Approach:** Combined task decomposition, dependency mapping, risk-aware sequencing, assumptions, checkpoints, asset allocation, human approval gates, and next-best-action generation in a search-and-rescue scenario.
- **Outcome:** Deployed a working Hugging Face Space that demonstrates how a planning agent can turn ambiguous user intent into an organized, safety-focused plan for humanitarian and emergency-response scenarios.
- **Tech:** Python, Streamlit, Hugging Face Inference API, Qwen/Qwen2.5-7B-Instruct
- **Repo:** Private repository; happy to provide a walkthrough or selected excerpts upon request
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/search-and-rescue-mission-planner) *(Hugging Face login required)*
- **Focus:** Planning agents, task decomposition, human-in-the-loop oversight, safety constraints, mission planning

---

### 03. Memory-Augmented Agent — Governed Project Continuity

- **Goal:** Build a memory-augmented agent that carries useful project context across turns without treating every interaction as permanent storage.
- **Approach:** Combined synthetic session-scoped memory, sentence-transformer retrieval, semantic and episodic memory, context compression, a deterministic **SAVE / SKIP / BLOCK** retention policy, metadata-only audit, real memory-pipeline observability, per-session isolation, and automated public-repository hygiene checks.
- **Outcome:** Delivered a production-validated governed continuity demo using the pattern: **Retrieve → Compress → Answer → Evaluate memory write → SAVE / SKIP / BLOCK.** The project passed **26 automated tests**, **5/5 retrieval benchmark cases ranked the expected memory #1** with **MRR = 1.0**, and **3/3 memory-write policy cases**. The public demo was rebuilt around a fictional Harborlight enterprise-pilot handoff, the repository and Hugging Face history were sanitized before redeployment, and the final centered 1080px business-first presentation passed human review.
- **Tech:** Python, Pydantic, sentence-transformers, scikit-learn, pandas, Gradio, pytest, GitHub Actions, Hugging Face Spaces
- **Repo:** [GitHub Repository](https://github.com/wushuchris/03-memory-augmented-agent)
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/03-memory-augmented-agent)
- **Focus:** Governed memory, project continuity, semantic memory, episodic memory, context compression, retention policy, session isolation, privacy-aware auditability, public-demo hygiene, live observability

---

### 04. Knowledge Retrieval Agent — Approved-Corpus Evidence Retrieval

- **Goal:** Build a retrieval agent that answers from an approved knowledge base, shows the evidence it used, and abstains when the retrieved evidence is too weak.
- **Approach:** Combined approved Markdown/text ingestion, overlapping source-aware chunking, sentence-transformer semantic search, BM25 lexical search, deterministic hybrid ranking, an explicit evidence-strength gate, source-cited extractive answers, and a real `search_iter()` event stream that exposes semantic scoring, keyword scoring, hybrid ranking, and evidence assessment while retrieval runs.
- **Outcome:** Delivered a production-validated retrieval demo using the pattern: **Approved corpus → Retrieve → Rank → Assess evidence → Answer or abstain.** The project passed **16 automated tests** and an **8-question retrieval benchmark** with **Hit@1 = 87.5%**, **Hit@3 = 100%**, and **MRR = 0.9375**. Deployment is gated on both pytest and retrieval quality, the Streamlit entrypoint has smoke coverage, CPU-only PyTorch avoids unnecessary CUDA dependencies, and the final centered 1080px business-first presentation passed human review. The project explicitly preserves the boundary that retrieval relevance is **not** independent truth verification.
- **Tech:** Python, Streamlit, sentence-transformers, scikit-learn, rank-bm25, pandas, pytest, Docker, GitHub Actions, Hugging Face Spaces
- **Repo:** [GitHub Repository](https://github.com/wushuchris/04-knowledge-retrieval-agent)
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/04-knowledge-retrieval-agent)
- **Focus:** Hybrid retrieval, approved-corpus grounding, evidence sufficiency, abstention, retrieval evaluation, source citations, live retrieval observability, deployment gates

---

### 05. Document Intelligence Agent — Source-Linked Document Intelligence

- **Goal:** Turn PDFs and text files into structured, searchable work products while preserving traceability back to the source document.
- **Approach:** Combined PyMuPDF parsing, typed Pydantic schemas, page-aware chunking, deterministic local extraction, stable source-linked findings, page/chunk provenance, keyword search over original chunks, JSON/CSV exports, and a real `parse_document_iter()` event stream that exposes the document-processing pipeline while it runs.
- **Outcome:** Delivered a production-validated document-intelligence demo using the pattern: **Parse → Structure → Preserve provenance → Search → Export.** The project passed **17 automated tests** and **4/4 deterministic evaluation cases**, added a Streamlit application smoke test, gates Hugging Face deployment on both pytest and the document benchmark, and passed final human presentation review with a centered 1080px business-first experience. The evaluation suite also caught and blocked a real legacy false positive where “completed” was incorrectly treated as a pending action item, and that failure became a permanent regression test.
- **Tech:** Python, Streamlit, PyMuPDF, Pydantic, pandas, pytest, Docker, GitHub Actions, Hugging Face Spaces
- **Repo:** [GitHub Repository](https://github.com/wushuchris/05-document-intelligence-agent)
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/05-document-intelligence-agent)
- **Focus:** Document intelligence, source provenance, PDF parsing, structured extraction, page-aware chunking, deterministic evaluation, searchable evidence, auditable outputs, live processing observability

---

### 06. Verification, Validation, and Evidence Agent — AI Evidence Review Gate

- **Goal:** Build an evidence-review boundary that checks AI-generated factual claims against supplied evidence before someone relies on the answer, while clearly separating evidence alignment from independent truth certification.
- **Approach:** Combined deterministic claim extraction, semantic and lexical evidence matching, citation-aware retrieval, explicit numeric and negation contradiction checks, reliability-aware rule evaluation, PASS/REVIEW/FAIL aggregation, human-review escalation, JSON/CSV/Markdown audit exports, and a real `verify_iter()` event stream that exposes the verification workflow while it runs.
- **Outcome:** Delivered a production-validated evidence-review demo using the pattern: **Semantic matching retrieves. Deterministic rules decide. Humans resolve uncertainty.** The project passed **20 automated tests** and **6/6 synthetic evaluation cases**, gates Hugging Face deployment on both pytest and the verification benchmark, and passed final human presentation review with a centered 1080px business-first experience, visible Live Evidence Review, readable claim-level findings, and an explicit **PASS ≠ independently proven truth** boundary.
- **Tech:** Python, Gradio, Pydantic, sentence-transformers, scikit-learn, pandas, pytest, GitHub Actions, Hugging Face Spaces
- **Repo:** [GitHub Repository](https://github.com/wushuchris/06-verification-validation-evidence-agent)
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/06-verification-validation-evidence-agent)
- **Focus:** AI verification, evidence alignment, contradiction detection, citation validation, deterministic guardrails, uncertainty escalation, human-in-the-loop review, auditability, live verification observability

---

### 07. Governed Tool-Using Agent — Application-Controlled Capability Boundary

- **Goal:** Let an LLM use useful business capabilities without allowing the model to grant itself unrestricted authority over code, databases, filesystems, or arbitrary network resources.
- **Approach:** Combined model-selected tool requests, a deterministic application-owned capability registry, typed arguments, explicit authorization, controlled execution, bounded tool rounds, normalized `success` / `blocked` / `error` outcomes, current-run audit logging, multi-tool reasoning, and a real `run_agent_iter()` event stream that exposes the model/application trust boundary while the request runs.
- **Outcome:** Delivered a production-validated governed tool-use demo using the pattern: **The model proposes. Application code owns authorization, validation, execution, and auditability.** The project passed **23 automated tests**, distinguishes requests blocked before execution from authorized tools that fail at runtime, uses a test-gated GitHub → Hugging Face deployment workflow, and passed final human presentation review with a centered business-first experience, an explicit Model Controls / Application Controls boundary, visible live execution events, and the raw engineering audit underneath.
- **Tech:** Python, Pydantic, OpenAI-compatible API client, Hugging Face Inference Providers, Cerebras, Gradio, SQLite, World Bank API, pytest, GitHub Actions, Hugging Face Spaces
- **Repo:** [GitHub Repository](https://github.com/wushuchris/07-tool-using-agent)
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/07-tool-using-agent)
- **Focus:** Governed tool use, function calling, capability authorization, tool allowlists, structured execution, multi-tool reasoning, failure semantics, auditability, agent security, live observability

---

### 08. Centralized Multi-Agent Orchestrator — Supervised AI Decision Team

- **Goal:** Build a centralized orchestrator that coordinates specialized Research, Analysis, Verification, and Synthesis agents while keeping routing, shared state, handoffs, failure containment, and publication under supervisor control.
- **Approach:** Combined Pydantic handoff schemas, deterministic analysis IDs, centralized routing, shared workflow state, verification gates, bounded schema normalization, quarantine of uncited analysis, source/analysis separation, orchestrator-controlled final rendering, auditable history, a reusable `run_iter()` supervisor-state stream, and a business-first live multi-agent presentation.
- **Outcome:** Delivered a production-validated supervised AI decision-team demo using the pattern: **Sources establish facts. Agents interpret. The orchestrator controls what gets published.** The project passed **18 automated tests**, converted live grounding and schema-drift failures into regression-tested control boundaries, and passed final human presentation review with a centered 1080px business-first workspace, real stage-by-stage supervisor activity, readable specialist work products, an explicit publication boundary, and the raw engineering audit underneath.
- **Tech:** Python, Pydantic, Gradio, OpenAI-compatible API client, Hugging Face Inference Providers, Cerebras, pytest, GitHub Actions, Hugging Face Spaces
- **Repo:** [GitHub Repository](https://github.com/wushuchris/08-centralized-multi-agent-orchestrator)
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/08-centralized-multi-agent-orchestrator)
- **Focus:** Multi-agent orchestration, supervisor-agent architecture, routing, agent handoffs, shared state, verification gates, failure containment, publication boundaries, real-time observability, evidence boundaries, auditability

---

### 09. Agentic Workflow System — Wealth Management Operations Workflow Dashboard

- **Goal:** Build a deterministic, resumable, and auditable workflow runtime that can coordinate AI-assisted business processes with bounded retries, persistence, conditional routing, and human escalation.
- **Approach:** Combined Pydantic workflow schemas, DAG validation, an allowlisted handler registry, deterministic execution, SQLite checkpoints, bounded retry policies, append-only workflow events, human approval gates, idempotent resume behavior, deterministic branching, a tightly bounded AI Intake Organizer, and live workflow-event playback derived from the real audit log inside a fictional wealth-management onboarding workflow.
- **Outcome:** Delivered a production-validated operations workflow dashboard using the pattern: **AI contributes work. Application code governs the process. Humans retain authority over consequential exceptions.** The project passed **127 automated tests** and a 10-case system evaluation, with live Hugging Face validation across standard completion, retry recovery, human approval/rejection, evaluation, persisted reload paths, and final human presentation review of a centered 1120px dashboard with visible paced workflow activity and a complete scrollable event transcript.
- **Tech:** Python, Pydantic, SQLite, Gradio, pytest, huggingface-hub, GitHub Actions, Hugging Face Spaces
- **Repo:** [GitHub Repository](https://github.com/wushuchris/09-agentic-workflow-sys)
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/09-agentic-workflow-sys)
- **Focus:** Agentic workflows, DAG execution, workflow state, persistence, bounded retries, human-in-the-loop escalation, idempotency, deterministic routing, bounded AI authority, auditability

---

### 10. Peer-to-Peer Coordination Agent — Decentralized Research Team

- **Goal:** Build a typed peer-to-peer coordination system where specialized agents can discover one another, self-select bounded work, exchange validated work products, challenge peers, and complete a shared mission without a central semantic orchestrator assigning the work.
- **Approach:** Combined typed Pydantic message contracts, passive peer discovery, a validated message bus, independent local state, deterministic role-claim rules, locally authorized work execution, challenge/revision protocols, failure containment, a centralized comparison baseline, bounded structured LLM work handlers, adversarial evaluations, and auditable protocol-derived live peer activity and coordination transcripts.
- **Outcome:** Delivered a production-validated multi-agent research demo using the pattern: **The agents reason with LLMs. The agents coordinate through an engineered protocol.** The project passed **115 automated tests**, completed deterministic and live LLM-assisted Hugging Face production checks, and passed final human presentation review with a centered business-first reading path, visible paced peer activity, a complete traceable transcript, and the full engineering audit underneath.
- **Tech:** Python, Pydantic, Gradio, OpenAI-compatible API client, Hugging Face Inference Providers, Qwen3.8, pytest, GitHub Actions, Hugging Face Spaces
- **Repo:** [GitHub Repository](https://github.com/wushuchris/10-peer-to-peer-coordination-agent)
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/10-peer-to-peer-coordination-agent)
- **Focus:** Peer-to-peer agents, decentralized coordination, typed messaging, local state, role self-selection, verification, disagreement handling, failure containment, bounded LLM authority, multi-agent evaluation, auditability

---

### 11. Distributed Auction Task Allocation Agent — Multi-Agent Task Marketplace

- **Goal:** Build a distributed task-allocation system where multiple qualified peers can compete for work based on capability, confidence, availability, and cost without a permanent semantic manager assigning each task.
- **Approach:** Combined typed task announcements, local BID/ABSTAIN policies, an application-owned capability registry, strict auction admission, deterministic weighted settlement and tie-breaking, bounded task reauction after explicit failure, allocation-efficiency and message-complexity metrics, a centralized comparison baseline, stress evaluation, bounded structured LLM work handlers after award, and a business-first live protocol playback derived from the real audit log.
- **Outcome:** Delivered a production-validated multi-agent due-diligence marketplace using the pattern: **Peers decide whether to compete. The protocol decides who wins.** The project passed **150 automated tests**, completed deterministic and live LLM-assisted Hugging Face production checks, preserved the same deterministic allocation boundary in both modes, quantified the coordination cost of decentralized allocation against an equivalent centralized baseline, and passed final human presentation review with visible paced auction activity and a complete scrollable protocol transcript.
- **Tech:** Python, Pydantic, Gradio, OpenAI-compatible API client, Hugging Face Inference Providers, Qwen3.8, pytest, GitHub Actions, Hugging Face Spaces
- **Repo:** [GitHub Repository](https://github.com/wushuchris/11-distributed-auction-task-allocation-agent)
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/11-distributed-auction-task-allocation-agent)
- **Focus:** Distributed task allocation, multi-agent auctions, capability matching, local bidding policy, deterministic settlement, bounded reauction, allocation efficiency, message complexity, bounded LLM authority, auditability

---

## 🚀 Other Featured Projects

### 🏎️ F1 AI Strategy Advisor — IoT + AI Decision System

- **Goal:** Build a real-time race strategy system using simulated IoT telemetry and AI-driven decision-making.
- **Approach:** Developed a modular pipeline combining telemetry simulation, rule-based strategy logic, and LLM-powered recommendations using Hugging Face.
- **Outcome:** Delivered a cloud-deployed interactive dashboard that generates context-aware race strategies based on live telemetry and historical trends.
- **Tech:** Python, Streamlit, pandas, Hugging Face (Llama 3), time-series simulation
- **Repo:** [GitHub Repository](https://github.com/wushuchris/f1-ai-strategy-advisor)
- **Live App:** [Streamlit App](https://f1-ai-strategy-advisor-ekkzao7ckhtbv3sfh5v4nd.streamlit.app/)
- **Focus:** Real-time AI systems, IoT simulation, hybrid decision engines

---

### 🧠 CKD Interpretable AI — Chronic Kidney Disease Prediction

- **Goal:** Build a machine learning system to predict Chronic Kidney Disease using clinical laboratory measurements while maintaining model transparency through explainable AI.
- **Approach:** Performed a full data science workflow including data auditing, cleaning, exploratory analysis, supervised learning (Logistic Regression, Random Forest, Gradient Boosting), and SHAP-based interpretability.
- **Outcome:** Developed a highly accurate CKD prediction model (Random Forest ROC-AUC = 1.0) and applied SHAP explainability to identify medically relevant predictors such as hemoglobin, packed cell volume, and kidney filtration rate.
- **Tech:** Python, pandas, scikit-learn, NumPy, SHAP, matplotlib, seaborn, Jupyter
- **Repo:** [GitHub Repository](https://github.com/wushuchris/ckd-interpretable-ai)
- **Focus:** Interpretable AI for healthcare decision support

---

### 🧠 BeautyScoreCV — Computer Vision Regression

- **Goal:** Build an exploratory computer vision pipeline to predict a continuous aesthetic score from facial images.
- **Approach:** Image preprocessing and CNN-based feature learning to map facial images to a numeric regression target.
- **Outcome:** Delivered an end-to-end CV regression prototype demonstrating image-to-continuous-target modeling, with documented limitations around subjectivity and dataset bias.
- **Tech:** Python, Jupyter, NumPy, pandas, OpenCV, TensorFlow / PyTorch
- **Repo:** [GitHub Repository](https://github.com/wushuchris/beautyscorecv)

---

### 🧠 Sex Classification ML — Supervised Binary Classification

- **Goal:** Train and evaluate a binary classifier to predict sex from structured input features.
- **Approach:** Data preprocessing, feature engineering, model training, and evaluation using standard supervised learning techniques.
- **Outcome:** Produced a fully evaluated binary classification pipeline with interpretable metrics including accuracy, confusion matrix, and ROC analysis.
- **Tech:** Python, scikit-learn, pandas, Jupyter
- **Repo:** [GitHub Repository](https://github.com/wushuchris/sexclassifyML)

---

### 🧠 AI Values Discovery Assistant — AI-Powered Reflection Tool

- **Goal:** Build an interactive AI application that helps users identify core values and generate a structured personal values statement.
- **Approach:** Designed a multi-step workflow capturing user inputs (values, motivations, decisions, behaviors) and applied prompt engineering to synthesize responses using a Hugging Face LLM.
- **Outcome:** Delivered a cloud-deployed Streamlit app that generates clear, personalized values statements in real time.
- **Tech:** Python, Streamlit, Hugging Face, prompt engineering
- **Repo:** [GitHub Repository](https://github.com/wushuchris/ai-values-discovery-assistant)
- **Live App:** [Streamlit App](https://ai-values-discovery-assistant-bqfylytoes3jnzynziycue.streamlit.app/)
- **Focus:** Human-centered AI, decision support systems, structured prompting

---

## Languages & Tools

**Core:** Python, pandas, scikit-learn, Pydantic, PyTorch/TensorFlow  
**AI & LLM:** Hugging Face, sentence-transformers, RAG, LLM APIs  
**Applications:** Streamlit, Gradio, Jupyter  
**Data & Cloud:** SQL, AWS, Hugging Face Spaces  
**Testing & DevOps:** pytest, Docker, GitHub Actions

---