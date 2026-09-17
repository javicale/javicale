# Evidence Summary

This document preserves the key observations from the original PoC while removing screenshots, local usernames, machine paths, employer branding, and other details that are unnecessary for a public portfolio.

## 1. Local deployment

### Ollama

Observed:

- Ollama installed successfully on Windows;
- local model pull completed;
- basic prompt execution returned a response;
- no installation or initial inference errors were documented.

### Python runtime

Observed:

- a Python virtual environment was created;
- the environment was reproducible;
- the model execution path was adapted to CPU because of laptop limitations;
- an end-to-end script returned responses;
- memory usage was observed during execution.

### LM Studio

Observed:

- the model ran through LM Studio without documented crashes;
- a chat transcript was persisted as evidence.

## 2. Prompt-behavior evaluation

The original evidence exercised multiple prompting patterns, including:

- closed-context question answering;
- inference from supplied information;
- controlled ambiguity;
- executive summarization;
- extreme compression;
- reformulation for non-technical audiences;
- constrained formatting;
- creative generation with explicit rules;
- strict JSON output;
- hierarchical JSON;
- multi-rule instruction following;
- intentionally conflicting constraints.

Observed sampling parameters recorded in the evidence:

- `temperature = 1.0`
- `top_p = 0.95`
- `top_k = 64`

### Historical timing snapshot

| Prompting strategy | Time |
| --- | ---: |
| Multi-turn chat | 02:47 |
| Persona injection | 00:21 |
| Q&A | 00:10 |
| Summarization | 00:19 |
| Creative writing | 00:55 |
| Structured output | 00:13 |
| Instruction following | 00:20 |

These measurements describe the original local setup only and should not be interpreted as current model benchmarks.

## 3. Reasoning-mode experiment

The evidence compared execution with reasoning/thinking enabled and disabled.

| Mode | Historical execution time |
| --- | ---: |
| Thinking ON | 2h 40m |
| Thinking OFF | 23m |

The original executive report characterized this as an approximately sevenfold latency increase in the tested environment.

QE interpretation: deeper reasoning behavior may be technically available while still being operationally unsuitable under constrained infrastructure.

## 4. Multimodal experiment

The evidence contains an image + text evaluation with reasoning enabled and disabled.

Observed:

- three prompts completed;
- latency data was captured;
- token-count data was captured;
- total documented execution time: **6h 05m**.

QE interpretation: successful completion did not establish operational efficiency.

## 5. Coding-assistance experiment

Observed:

- five coding challenges were executed;
- outputs were documented as syntactically valid;
- IDE integration was exercised end-to-end;
- total documented execution time: **4h 20m**.

Important boundary: syntactic validity is not equivalent to functional correctness, maintainability, security, or production suitability. The preserved evidence does not support broader claims.

## 6. Function-calling / agentic-workflow experiment

The original evidence documents a small tool-calling loop.

Observed:

- two tools were implemented and callable;
- four multi-step tasks were executed;
- the recorded sample reported 100% task completion;
- fallback behavior was exercised without documented crashes;
- total documented execution time: **9 minutes**.

Important boundary: four successful tasks are evidence of PoC feasibility only. They are not evidence of enterprise reliability or unrestricted autonomous operation.

## 7. Fine-tuning feasibility

The evidence documents a QLoRA-oriented experiment but also records a critical limitation:

- no suitable NVIDIA GPU was available;
- a TinyLlama fallback was used;
- the run reached approximately **60%** completion;
- partial execution time was **34h 19m**.

Therefore the public claim is intentionally narrow:

> Fine-tuning feasibility was explored, but the intended local-model fine-tuning experiment was not completed because of infrastructure constraints.

## 8. Evidence-to-decision mapping

| Evidence | Supported conclusion | Unsupported conclusion |
| --- | --- | --- |
| Successful local inference | Local execution is technically feasible | Production readiness |
| Successful prompt scenarios | Selected behaviors can be exercised | Generalized accuracy |
| Reasoning completed | Reasoning mode can execute | Acceptable production latency |
| Multimodal completed | Image + text processing is feasible | Scalable multimodal service |
| Five coding outputs syntactically valid | Coding assistance can be explored | Code correctness benchmark |
| Four tool-driven tasks completed | Function calling can work in a constrained loop | Enterprise autonomous-agent reliability |
| Fine-tuning run incomplete | Hardware is a material dependency | Successful Gemma fine-tuning |

## 9. Preserved professional lesson

The evidence demonstrates a useful QE principle:

> A capability should not be promoted from **“observed working”** to **“trusted for production”** without explicit quality metrics, regression controls, operational thresholds, security/privacy validation, and repeatable evidence.
