# Limitations and Claim Boundaries

This case study is intentionally conservative. It preserves what the historical PoC demonstrated without upgrading observations into claims that the evidence cannot support.

## Historical environment

The measurements were produced in a specific local environment with constrained hardware. They are useful as engineering evidence for that setup, but they are not current or portable performance benchmarks.

## Model naming and scope

The preserved source material refers to a local Gemma 4 PoC and documents the model/runtime used in that experiment. This public case study does not attempt to revalidate model naming, release status, or current product capabilities.

Its purpose is to preserve the Quality Engineering process and the observed experimental results.

## Prompt evaluation

Successful prompt execution demonstrates functional behavior in selected examples only.

It does not establish:

- generalized factual accuracy;
- low hallucination rate;
- production-grade consistency;
- robustness against adversarial input;
- domain-specific correctness.

## Coding assistance

The original evidence records five coding challenges whose outputs were syntactically valid.

No broader claim is made regarding:

- functional correctness;
- algorithmic optimality;
- security;
- maintainability;
- production readiness.

## Function calling

The function-calling experiment used a small number of tools and tasks.

The recorded success rate applies only to that limited sample. It should not be interpreted as an SLA, a reliability benchmark, or evidence that unrestricted autonomous agents are safe.

## Fine-tuning

The intended fine-tuning experiment did not complete as a Gemma fine-tuning result.

Because the local environment lacked suitable NVIDIA GPU resources, a TinyLlama fallback was used and the run reached approximately 60% completion after 34h 19m.

Therefore this case study makes **no claim of successful Gemma fine-tuning**.

## Production readiness

The original PoC explicitly identified missing controls, including:

- hallucination and accuracy benchmarks;
- regression automation;
- security validation;
- privacy review;
- load and throughput testing;
- inference-cost analysis;
- auditability and version governance.

For that reason, the historical recommendation was controlled continuation, not production approval.

## Evidence publication

The original evidence included screenshots, local machine paths, usernames, and organizational branding. Those raw artifacts are intentionally not published here.

Instead, this repository preserves a sanitized textual summary of the observations that matter to the engineering conclusion.

This reduces disclosure risk while keeping the case study auditable at the level appropriate for a public professional portfolio.
