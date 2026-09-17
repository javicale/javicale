# Javier Capa

### Senior Quality Software Engineer · Quality Engineering · Test Automation · AI-assisted QA

I build quality systems, not just test cases.

**[Explore my Quality Engineering portfolio ↗](https://www.javiercapa.com/)**  
Project case studies, engineering decisions, verified evidence and R&D learning notes.

With **17+ years in Software Quality Assurance and Quality Engineering**, I focus on turning quality into an engineering capability: clear strategy, risk-based validation, automation, observability, evidence, and release decisions that teams can trust.

Currently exploring how **agentic workflows, MCP, AI-assisted testing, local/private LLM evaluation, test observability and evidence-driven release decisions** could complement established Quality Engineering practices.

---

## What I work on

- **Quality Engineering Strategy** — QA governance, test strategy, STLC, shift-left and risk-based testing.
- **Test Automation** — Playwright, API testing, regression strategy and maintainable automation architecture.
- **Data & ETL Quality** — source-to-target validation, SQL/database reconciliation, transformation rules and differential testing.
- **CI/CD Quality Gates** — automated validation, evidence collection and release-readiness signals.
- **Performance & API Testing** — JMeter, Locust, Postman and service-level validation.
- **Observability for Testing** — traces, logs, metrics, test evidence and failure diagnostics.
- **AI / LLM Quality Evaluation** — local model assessment, prompt behavior, structured outputs, reasoning latency, multimodal evaluation, tool calling and production-readiness boundaries.
- **AI-assisted QE research** — experiments with agents, MCP, deterministic evals, execution gating, plan-to-execution traceability and human-governed release decisions.
- **QA Leadership** — scalable processes, quality metrics, mentoring and cross-functional quality ownership.

---

## Featured portfolio

### 🧪 [Agentic Quality Engineering Lab](https://github.com/javicale/agentic-quality-engineering)
An exploratory R&D / learning lab investigating how probabilistic agent planning can coexist with deterministic Quality Engineering controls. The current baseline covers MCP context, agent evals, CSV and SQL/database differential testing, schema/key reconciliation, SQLAlchemy portability, structured evidence and **plan-to-execution traceability**. In the final verified live `gpt-5.6-luna` SQL experiment, the agent produced a **90/100 PASS** plan whose **5/5 executable scenarios mapped to registered capabilities and passed**, with 0 deferred/unsupported scenarios before the pipeline reached **GO / LOW**. A negative control proves that an unsupported HIGH scenario forces `NO_GO` even when another differential is green. The repository remains explicitly an R&D lab rather than a production-ready Agentic AI framework.

### 🔎 [Quality Observability Lab](https://github.com/javicale/quality-observability-lab)
A completed R&D / learning lab connecting Playwright execution with OpenTelemetry traces, correlated logs, bounded metrics, structured browser evidence and deterministic failure diagnosis. The lab now has two independently verified contracts: local JSON/JSONL evidence with a fail-closed gate, and real **OTLP/HTTP ingestion into a local Grafana LGTM stack**. The final `main` CI run validates both `deterministic-evidence` and `otel-stack-contract`; Tempo returns the exact success/error traces, Loki preserves trace/run correlation, Prometheus exposes the request metric, and Grafana serves the provisioned Quality Observability dashboard. The deliberate HTTP 500 remains a business `FAIL` even when the experiment gate passes. The repository is intentionally closed at this reproducible portfolio scope rather than positioned as a production observability platform.

### 🧠 [Local LLM Quality Assessment — Evidence-Based QE Case Study](./case-studies/local-llm-quality-assessment/)
A historical Quality Engineering case study evaluating a locally hosted open LLM across deployment, reproducible execution, prompt behavior, structured outputs, reasoning latency, multimodal analysis, coding assistance, function calling and fine-tuning feasibility. The preserved evidence includes real execution timings and hardware constraints, then translates those observations into an explicit engineering boundary: **continue controlled experimentation, but do not infer production readiness from a successful demo**. The public version is deliberately sanitized and distinguishes observed behavior from unsupported reliability or scale claims.

### 🎭 [Playwright Quality Engineering Framework](https://github.com/javicale/playwright-quality-engineering)
A production-minded Playwright + TypeScript reference framework demonstrating UI and API testing, Page Objects, reusable fixtures, evidence, CI execution, cross-browser coverage and maintainable test architecture.

### 🧭 [Quality Engineering Strategy & Playbook](https://github.com/javicale/quality-engineering-playbook)
A practical collection of QA/QE strategy material: test strategy, validation framework, risk-based testing, evidence standards and an Agentic Quality Engineering roadmap.

---

## R&D — Agentic Quality Engineering

This is an **active learning direction**, not a claim of mature Agentic AI expertise.

The research question is:

> **Where can probabilistic AI increase validation capacity without weakening deterministic controls, evidence or human accountability?**

The completed V4 learning baseline implements this boundary:

```text
Change / Risk
   ↓
Read-only Context / MCP Tools
   ↓
Agent proposes Validation Plan
   ↓
Deterministic Eval
   ↓
Pre-execution Gate
   ↓
Scenario → Capability Mapping
   ↓
CSV / SQL Deterministic Validation
   ↓
Plan-to-Execution Traceability
   ↓
Coverage Gate
   ↓
Observability + Evidence
   ↓
Risk-based Release Signal
   ↓
Human Decision
```

The key conclusion is that **plan quality, permission to execute, actual execution coverage and release authority are different claims** and should be independently testable. HIGH/CRITICAL planned scenarios that are unsupported or not executed block release rather than being hidden behind an overall green result.

The public [Agentic Quality Engineering Lab](https://github.com/javicale/agentic-quality-engineering) preserves the experiments, negative controls, live model evidence, findings and limitations.

---

## Technology stack

**Automation & Testing**  
Playwright · Postman · JMeter · Locust · BrowserStack · API Testing · E2E Testing · Performance Testing

**Engineering**  
TypeScript · JavaScript · C# · Python · Java · SQL · PL/SQL · HTML

**Data & Database Quality**  
Source-to-target Reconciliation · SQL Differential Testing · Schema Drift · Data Integrity · SQLAlchemy

**Platform & Delivery**  
Docker · GitHub Actions · GitLab CI/CD · CircleCI · Linux · Windows · macOS

**Observability & Analytics**  
OpenTelemetry · Grafana · Tempo · Loki · Prometheus · Power BI · Logs · Metrics · Traces · Test Evidence

**AI / Local Model Evaluation**  
Ollama · LM Studio · Hugging Face Transformers · Prompt Evaluation · Structured Output · Function Calling · Multimodal Evaluation

**Quality & Delivery**  
Jira · Azure DevOps · STLC · Shift-left · Risk-based Testing · Quality Gates · QA Governance

---

## Engineering principles

```text
Quality is not the last step before release.
Quality is the system that makes a release decision explainable.
```

I value:

- evidence over assumptions;
- risk coverage over test-count vanity metrics;
- maintainable automation over brittle scripts;
- observability over unexplained failures;
- fast feedback over late defect discovery;
- human accountability even when AI participates in validation.

---

## Current focus

- Quality Engineering strategy and governance
- Playwright and maintainable test automation
- ETL, SQL and data-quality validation
- Test observability and evidence
- Local/private LLM quality evaluation
- AI-assisted QA
- Agentic QE learning and experimentation
- MCP and testing-agent boundaries
- Deterministic evals and execution gating
- Plan-to-execution traceability
- Human-in-the-loop release governance

---

## Connect

- GitHub: [@javicale](https://github.com/javicale)
- Email: [ljavier.capa@gmail.com](mailto:ljavier.capa@gmail.com)

---

> **Portfolio philosophy:** every public repository here should demonstrate a Quality Engineering decision, technique, experiment or capability — not exist only to increase the repository count.
