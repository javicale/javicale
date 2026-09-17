# Methodology

## Evaluation approach

The PoC was executed as an exploratory Quality Engineering assessment rather than as a formal model benchmark.

The working sequence was:

```text
Environment setup
   ↓
Local model execution
   ↓
Prompt-behavior checks
   ↓
Reasoning experiments
   ↓
Multimodal experiments
   ↓
Coding-assistance checks
   ↓
Function-calling workflow
   ↓
Fine-tuning feasibility
   ↓
Risk assessment
   ↓
Go / No-Go recommendation
```

## What was measured

The preserved evidence contains a mixture of qualitative and quantitative observations:

- successful or failed execution;
- end-to-end completion;
- execution time;
- limited token-count observations;
- memory observations;
- structured-output behavior;
- constrained-prompt behavior;
- function-calling completion;
- hardware limitations.

## What was not measured rigorously

The PoC did not establish a statistically meaningful benchmark for:

- factual accuracy;
- hallucination rate;
- semantic correctness of generated code;
- model consistency across repeated runs;
- robustness under adversarial prompts;
- security posture;
- privacy risk;
- throughput under concurrent load;
- cost per inference;
- long-term tool-calling reliability.

These gaps are intentional parts of the public case study because they explain why the final recommendation stopped at controlled expansion rather than production approval.

## Quality Engineering decision model

The PoC can be represented as four evidence levels:

### Level 1 — Technical viability

Question: can the local stack install, load and execute?

Evidence used:

- successful runtime setup;
- successful local inference;
- repeatable Python environment;
- GUI execution.

### Level 2 — Capability observation

Question: can selected model behaviors be exercised?

Evidence used:

- prompting scenarios;
- structured outputs;
- reasoning execution;
- multimodal execution;
- coding assistance;
- function calling.

### Level 3 — Operational suitability

Question: are latency, infrastructure dependency and execution behavior acceptable for the intended use case?

Evidence used:

- execution timing;
- CPU constraints;
- multimodal and reasoning latency;
- fine-tuning blockage.

### Level 4 — Production readiness

Question: is there sufficient repeatable evidence to trust the capability in production?

The PoC did not satisfy this level because formal benchmarks, regression controls, security/privacy validation, load testing and governance controls were still missing.

## Why this methodology matters

A common failure mode in AI experimentation is collapsing these four levels into one:

> “The demo worked, therefore the solution is ready.”

This case study deliberately keeps them separate.

For Quality Engineering, the transition from prototype to trusted capability requires explicit acceptance criteria, reproducibility, regression evidence, operational thresholds and governance—not only successful prompts.
