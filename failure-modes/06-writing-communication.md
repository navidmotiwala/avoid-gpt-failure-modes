# Writing and communication

[Back to README](../README.md) | [Evaluation protocol](../evaluations/PROTOCOL.md)

This chapter expands failure modes 51–60. The examples below are **constructed test scenarios**, not observed failures. A model's behavior must be measured before claiming that a particular model fails any test.

**Common investigation approach:** Compare output against the requested audience, tone, factual content, constraints and information density.

## 51. Formulaic AI language

**Definition:** Uses repetitive, generic phrasing.

**Why it can happen:** Generic patterns and completion incentives can produce fluent but repetitive, vague or poorly targeted writing. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **formulaic ai language**. The assistant produces a plausible response but uses repetitive, generic phrasing. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare output against the requested audience, tone, factual content, constraints and information density. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Use plain language, remove filler, retain concrete facts and prioritize the reader's actual question. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for formulaic ai language.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Request a short, audience-specific explanation with banned phrases and a word limit; check every requirement.

**Starter test input:** Explain this technical concept to a beginner in 80 words.

**Expected check:** Plain, accurate, nonrepetitive explanation within limit. Adapt this starter case to isolate **formulaic ai language**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 52. Generic advice

**Definition:** Offers recommendations without relevant specifics.

**Why it can happen:** Generic patterns and completion incentives can produce fluent but repetitive, vague or poorly targeted writing. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **generic advice**. The assistant produces a plausible response but offers recommendations without relevant specifics. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare output against the requested audience, tone, factual content, constraints and information density. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Use plain language, remove filler, retain concrete facts and prioritize the reader's actual question. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for generic advice.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Request a short, audience-specific explanation with banned phrases and a word limit; check every requirement.

**Starter test input:** Explain this technical concept to a beginner in 80 words.

**Expected check:** Plain, accurate, nonrepetitive explanation within limit. Adapt this starter case to isolate **generic advice**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 53. Repetitive explanations

**Definition:** Restates the same point unnecessarily.

**Why it can happen:** Generic patterns and completion incentives can produce fluent but repetitive, vague or poorly targeted writing. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **repetitive explanations**. The assistant produces a plausible response but restates the same point unnecessarily. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare output against the requested audience, tone, factual content, constraints and information density. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Use plain language, remove filler, retain concrete facts and prioritize the reader's actual question. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for repetitive explanations.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Request a short, audience-specific explanation with banned phrases and a word limit; check every requirement.

**Starter test input:** Explain this technical concept to a beginner in 80 words.

**Expected check:** Plain, accurate, nonrepetitive explanation within limit. Adapt this starter case to isolate **repetitive explanations**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 54. Excessive verbosity

**Definition:** Adds detail that does not help the task.

**Why it can happen:** Generic patterns and completion incentives can produce fluent but repetitive, vague or poorly targeted writing. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **excessive verbosity**. The assistant produces a plausible response but adds detail that does not help the task. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare output against the requested audience, tone, factual content, constraints and information density. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Use plain language, remove filler, retain concrete facts and prioritize the reader's actual question. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for excessive verbosity.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Request a short, audience-specific explanation with banned phrases and a word limit; check every requirement.

**Starter test input:** Explain this technical concept to a beginner in 80 words.

**Expected check:** Plain, accurate, nonrepetitive explanation within limit. Adapt this starter case to isolate **excessive verbosity**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 55. Unnecessary jargon

**Definition:** Uses technical terms without need or explanation.

**Why it can happen:** Generic patterns and completion incentives can produce fluent but repetitive, vague or poorly targeted writing. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **unnecessary jargon**. The assistant produces a plausible response but uses technical terms without need or explanation. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare output against the requested audience, tone, factual content, constraints and information density. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Use plain language, remove filler, retain concrete facts and prioritize the reader's actual question. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for unnecessary jargon.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Request a short, audience-specific explanation with banned phrases and a word limit; check every requirement.

**Starter test input:** Explain this technical concept to a beginner in 80 words.

**Expected check:** Plain, accurate, nonrepetitive explanation within limit. Adapt this starter case to isolate **unnecessary jargon**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 56. Overly formal writing

**Definition:** Sounds stiff in contexts requiring plain language.

**Why it can happen:** Generic patterns and completion incentives can produce fluent but repetitive, vague or poorly targeted writing. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **overly formal writing**. The assistant produces a plausible response but sounds stiff in contexts requiring plain language. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare output against the requested audience, tone, factual content, constraints and information density. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Use plain language, remove filler, retain concrete facts and prioritize the reader's actual question. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for overly formal writing.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Request a short, audience-specific explanation with banned phrases and a word limit; check every requirement.

**Starter test input:** Explain this technical concept to a beginner in 80 words.

**Expected check:** Plain, accurate, nonrepetitive explanation within limit. Adapt this starter case to isolate **overly formal writing**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 57. Artificial enthusiasm

**Definition:** Uses exaggerated praise or excitement.

**Why it can happen:** Generic patterns and completion incentives can produce fluent but repetitive, vague or poorly targeted writing. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **artificial enthusiasm**. The assistant produces a plausible response but uses exaggerated praise or excitement. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare output against the requested audience, tone, factual content, constraints and information density. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Use plain language, remove filler, retain concrete facts and prioritize the reader's actual question. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for artificial enthusiasm.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Request a short, audience-specific explanation with banned phrases and a word limit; check every requirement.

**Starter test input:** Explain this technical concept to a beginner in 80 words.

**Expected check:** Plain, accurate, nonrepetitive explanation within limit. Adapt this starter case to isolate **artificial enthusiasm**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 58. Filler sentences

**Definition:** Adds text with little informational value.

**Why it can happen:** Generic patterns and completion incentives can produce fluent but repetitive, vague or poorly targeted writing. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **filler sentences**. The assistant produces a plausible response but adds text with little informational value. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare output against the requested audience, tone, factual content, constraints and information density. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Use plain language, remove filler, retain concrete facts and prioritize the reader's actual question. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for filler sentences.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Request a short, audience-specific explanation with banned phrases and a word limit; check every requirement.

**Starter test input:** Explain this technical concept to a beginner in 80 words.

**Expected check:** Plain, accurate, nonrepetitive explanation within limit. Adapt this starter case to isolate **filler sentences**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 59. Repetitive structures

**Definition:** Uses the same sentence pattern repeatedly.

**Why it can happen:** Generic patterns and completion incentives can produce fluent but repetitive, vague or poorly targeted writing. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **repetitive structures**. The assistant produces a plausible response but uses the same sentence pattern repeatedly. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare output against the requested audience, tone, factual content, constraints and information density. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Use plain language, remove filler, retain concrete facts and prioritize the reader's actual question. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for repetitive structures.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Request a short, audience-specific explanation with banned phrases and a word limit; check every requirement.

**Starter test input:** Explain this technical concept to a beginner in 80 words.

**Expected check:** Plain, accurate, nonrepetitive explanation within limit. Adapt this starter case to isolate **repetitive structures**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 60. Style over substance

**Definition:** Prioritizes polished wording over correctness.

**Why it can happen:** Generic patterns and completion incentives can produce fluent but repetitive, vague or poorly targeted writing. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **style over substance**. The assistant produces a plausible response but prioritizes polished wording over correctness. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare output against the requested audience, tone, factual content, constraints and information density. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Use plain language, remove filler, retain concrete facts and prioritize the reader's actual question. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for style over substance.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Request a short, audience-specific explanation with banned phrases and a word limit; check every requirement.

**Starter test input:** Explain this technical concept to a beginner in 80 words.

**Expected check:** Plain, accurate, nonrepetitive explanation within limit. Adapt this starter case to isolate **style over substance**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

