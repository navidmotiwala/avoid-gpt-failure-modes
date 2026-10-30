# Reproducible Evaluation Protocol

[Back to README](../README.md)

## What this project can and cannot claim

A **test case** is a proposed experiment. A **verified failure** requires a captured model output and independently checked reference evidence. No model accuracy, failure rate, or improvement is claimed until runs are recorded. Prompts can help, but cannot guarantee factuality, security, or instruction adherence.

## Required test record

| Field | What to record |
|---|---|
| Case ID | Stable identifier |
| Failure mode | Exact numbered category |
| Hypothesis | What behavior might fail |
| Model/provider | Exact model identifier and version when available |
| Run date | UTC timestamp |
| Settings | Temperature, seed, system instructions, tools and retrieval settings when known |
| Input | Complete user prompt and relevant context |
| Reference | Source, calculation, executable assertion, or adjudication protocol |
| Raw output | Full unedited response |
| Tool trace | Actual retrieval and tool results, if any |
| Verdict | Pass, fail, partial, unscorable |
| Evidence | Exact failing span and independently checked reference |
| Reviewer | Who assessed the result and how disputes were resolved |

## Method

1. Define a narrow, falsifiable behavior before running the model.
2. Write an expected result independently, using authoritative evidence or deterministic calculations.
3. Prepare a baseline prompt and a single intervention prompt. Change only one variable at a time.
4. Test multiple paraphrases and repeated runs; record the sampling procedure.
5. Preserve raw prompts, responses, tool traces, timestamps and model configuration.
6. Score factuality, citation support, constraint adherence, calibration and refusal/abstention only when relevant.
7. Blind reviewers to condition where practical; use two reviewers for subjective labels and resolve disagreement.
8. Report denominator, failures, partials and unscorable cases. Do not silently drop inconvenient outputs.
9. Document dataset provenance and whether prompts could have appeared in training or public benchmarks.
10. Publish a limitations section describing sample size, model drift, unavailable settings and domain coverage.

## Scoring

- **Pass:** Meets every required criterion for the specified case.
- **Fail:** Violates at least one essential criterion, with a traceable explanation.
- **Partial:** Some nonessential criteria are met; essential success is not fully established.
- **Unscorable:** Missing reference, inaccessible evidence or insufficient trace.

For a binary metric: pass rate = passes / (passes + failures). Report partial and unscorable counts separately. Do not call this overall model accuracy unless the sample is representative.

## Citation audit

Check that the source exists, resolves, is relevant, supports the exact attached claim, and is not contradicted by a stronger primary source. A working URL alone is not proof.

## Prompt-injection safety

Use synthetic secrets and sandbox-only tools. Never run destructive or credential-exfiltration tests against real accounts. Record whether untrusted text was treated as data rather than an instruction.

## Publication rules

Clearly label synthetic cases, unexecuted tests, illustrative responses and actual observations. Do not present a constructed example as a real transcript. Do not publish personal data, credentials or private documents.

## Reproducibility limits

Hosted models change, sampling is stochastic, hidden instructions may differ and tools may return different data later. Re-running the same prompt may not reproduce the same output. Preserve enough metadata to explain the limits.
