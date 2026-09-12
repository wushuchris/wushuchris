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

- **Goal:** Build an autonomous agent that evaluates context and recommends a bounded next action.
- **Approach:** Combined rule-based scoring, structured Pydantic schemas, Hugging Face LLM explanations, guardrail checks, batch processing, and auditable JSON/CSV logs.
- **Outcome:** Delivered a GitHub-ready agent project using the pattern: **Rules decide. The LLM explains. Guardrails review.**
- **Tech:** Python, Pydantic, pandas, matplotlib, Hugging Face Inference Providers, OpenAI-compatible API client
- **Repo:** [GitHub Repository](https://github.com/wushuchris/01-autonomous-decision-agent)
- **Focus:** Agent engineering, bounded autonomy, structured outputs, guardrails, evaluation

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

### 03. Memory-Augmented Agent — Personal Project Memory Assistant

- **Goal:** Build an agent that uses persistent memory and context recall to support an ongoing project.
- **Approach:** Combined structured memory storage, sentence-transformer embeddings, cosine-similarity retrieval, semantic and episodic memory, context compression, memory write policy, and auditable memory logs.
- **Outcome:** Deployed a working Hugging Face Space that demonstrates persistent project memory, visible memory retrieval, context compression, session learning, saved-memory inspection, and audit logging.
- **Tech:** Python, Pydantic, pandas, sentence-transformers, scikit-learn, Gradio, Hugging Face Spaces
- **Repo:** [GitHub Repository](https://github.com/wushuchris/03-memory-augmented-agent)
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/03-memory-augmented-agent)
- **Focus:** Memory-augmented agents, retrieval, context recall, semantic memory, episodic memory, context compression, agent auditability

---

### 04. Knowledge Retrieval Agent — Source-Cited RAG Assistant

- **Goal:** Build a source-cited knowledge assistant that retrieves relevant evidence before answering.
- **Approach:** Combined markdown/text ingestion, overlapping chunking, sentence-transformer embeddings, BM25 keyword scoring, hybrid retrieval ranking, cited evidence panels, and confidence-labeled extractive answers.
- **Outcome:** Delivered a GitHub-ready and Hugging Face-deployed RAG agent using the pattern: **Retrieve first. Answer second. Cite always.**
- **Tech:** Python, Streamlit, sentence-transformers, scikit-learn, rank-bm25, Docker, GitHub Actions, Hugging Face Spaces
- **Repo:** [GitHub Repository](https://github.com/wushuchris/04-knowledge-retrieval-agent)
- **Live Demo:** [Hugging Face Space](https://huggingface.co/spaces/FlyingNunchucks/04-knowledge-retrieval-agent)
- **Focus:** RAG, retrieval quality, source grounding, citation discipline, evidence ranking, deployment workflow

---

### 05. Document Intelligence Agent — Structured PDF Intelligence System

- **Goal:** Build a document intelligence agent that converts PDFs and text files into structured summaries, searchable chunks, and exportable data.
- **Approach:** Combined PyMuPDF document parsing, Pydantic schemas, page-aware chunking, lightweight local extraction rules, keyword search, Streamlit UI, Docker deployment, and JSON/CSV export workflows.
- **Outcome:** Delivered a GitHub-ready and Hugging Face-deployed document intelligence prototype using the pattern: **Parse → Structure → Validate → Search → Export.**
- **Tech:** Python, Streamlit, PyMuPDF, Pydantic, pandas, Docker, GitHub Actions, Hugging Face Spaces
- **Repo:** [GitHub Repository](https://github.com/wushuchris/05-document-intelligence-agent)
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