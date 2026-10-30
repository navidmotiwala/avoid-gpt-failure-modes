# Context and instruction following

[Back to README](../README.md) | [Evaluation protocol](../evaluations/PROTOCOL.md)

This chapter expands failure modes 31–40. The examples below are **constructed test scenarios**, not observed failures. A model's behavior must be measured before claiming that a particular model fails any test.

**Common investigation approach:** Compare the final answer against an explicit requirements checklist and the original conversation.

## 31. Context loss

**Definition:** Forgets or overlooks relevant earlier information.

**Why it can happen:** Important constraints can be overlooked, misunderstood, displaced by long context, or confused with lower-trust text. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **context loss**. The assistant produces a plausible response but forgets or overlooks relevant earlier information. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare the final answer against an explicit requirements checklist and the original conversation. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Before answering, identify the applicable task constraints and follow them. Ask only when a missing detail prevents a reliable answer. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for context loss.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide three concrete constraints and one irrelevant distraction; score every constraint independently.

**Starter test input:** Follow these constraints: 60 words maximum, no bullets, include one limitation.

**Expected check:** All three constraints satisfied. Adapt this starter case to isolate **context loss**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 32. Instruction misinterpretation

**Definition:** Understands a request incorrectly.

**Why it can happen:** Important constraints can be overlooked, misunderstood, displaced by long context, or confused with lower-trust text. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **instruction misinterpretation**. The assistant produces a plausible response but understands a request incorrectly. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare the final answer against an explicit requirements checklist and the original conversation. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Before answering, identify the applicable task constraints and follow them. Ask only when a missing detail prevents a reliable answer. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for instruction misinterpretation.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide three concrete constraints and one irrelevant distraction; score every constraint independently.

**Starter test input:** Follow these constraints: 60 words maximum, no bullets, include one limitation.

**Expected check:** All three constraints satisfied. Adapt this starter case to isolate **instruction misinterpretation**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 33. Ignored constraints

**Definition:** Misses required length, style, scope, or format.

**Why it can happen:** Important constraints can be overlooked, misunderstood, displaced by long context, or confused with lower-trust text. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **ignored constraints**. The assistant produces a plausible response but misses required length, style, scope, or format. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare the final answer against an explicit requirements checklist and the original conversation. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Before answering, identify the applicable task constraints and follow them. Ask only when a missing detail prevents a reliable answer. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for ignored constraints.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide three concrete constraints and one irrelevant distraction; score every constraint independently.

**Starter test input:** Follow these constraints: 60 words maximum, no bullets, include one limitation.

**Expected check:** All three constraints satisfied. Adapt this starter case to isolate **ignored constraints**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 34. Inconsistent responses

**Definition:** Gives incompatible answers across turns.

**Why it can happen:** Important constraints can be overlooked, misunderstood, displaced by long context, or confused with lower-trust text. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **inconsistent responses**. The assistant produces a plausible response but gives incompatible answers across turns. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare the final answer against an explicit requirements checklist and the original conversation. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Before answering, identify the applicable task constraints and follow them. Ask only when a missing detail prevents a reliable answer. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for inconsistent responses.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide three concrete constraints and one irrelevant distraction; score every constraint independently.

**Starter test input:** Follow these constraints: 60 words maximum, no bullets, include one limitation.

**Expected check:** All three constraints satisfied. Adapt this starter case to isolate **inconsistent responses**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 35. Instruction conflicts

**Definition:** Handles competing instructions incorrectly.

**Why it can happen:** Important constraints can be overlooked, misunderstood, displaced by long context, or confused with lower-trust text. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **instruction conflicts**. The assistant produces a plausible response but handles competing instructions incorrectly. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare the final answer against an explicit requirements checklist and the original conversation. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Before answering, identify the applicable task constraints and follow them. Ask only when a missing detail prevents a reliable answer. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for instruction conflicts.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide three concrete constraints and one irrelevant distraction; score every constraint independently.

**Starter test input:** Follow these constraints: 60 words maximum, no bullets, include one limitation.

**Expected check:** All three constraints satisfied. Adapt this starter case to isolate **instruction conflicts**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 36. Overgeneralization

**Definition:** Applies a narrow rule too broadly.

**Why it can happen:** Important constraints can be overlooked, misunderstood, displaced by long context, or confused with lower-trust text. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **overgeneralization**. The assistant produces a plausible response but applies a narrow rule too broadly. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare the final answer against an explicit requirements checklist and the original conversation. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Before answering, identify the applicable task constraints and follow them. Ask only when a missing detail prevents a reliable answer. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for overgeneralization.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide three concrete constraints and one irrelevant distraction; score every constraint independently.

**Starter test input:** Follow these constraints: 60 words maximum, no bullets, include one limitation.

**Expected check:** All three constraints satisfied. Adapt this starter case to isolate **overgeneralization**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 37. Missing user intent

**Definition:** Answers the words but not the actual task.

**Why it can happen:** Important constraints can be overlooked, misunderstood, displaced by long context, or confused with lower-trust text. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **missing user intent**. The assistant produces a plausible response but answers the words but not the actual task. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare the final answer against an explicit requirements checklist and the original conversation. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Before answering, identify the applicable task constraints and follow them. Ask only when a missing detail prevents a reliable answer. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for missing user intent.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide three concrete constraints and one irrelevant distraction; score every constraint independently.

**Starter test input:** Follow these constraints: 60 words maximum, no bullets, include one limitation.

**Expected check:** All three constraints satisfied. Adapt this starter case to isolate **missing user intent**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 38. Context assumptions

**Definition:** Invents unstated background details.

**Why it can happen:** Important constraints can be overlooked, misunderstood, displaced by long context, or confused with lower-trust text. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **context assumptions**. The assistant produces a plausible response but invents unstated background details. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare the final answer against an explicit requirements checklist and the original conversation. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Before answering, identify the applicable task constraints and follow them. Ask only when a missing detail prevents a reliable answer. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for context assumptions.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide three concrete constraints and one irrelevant distraction; score every constraint independently.

**Starter test input:** Follow these constraints: 60 words maximum, no bullets, include one limitation.

**Expected check:** All three constraints satisfied. Adapt this starter case to isolate **context assumptions**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 39. Missing clarification

**Definition:** Guesses when an essential detail is unknown.

**Why it can happen:** Important constraints can be overlooked, misunderstood, displaced by long context, or confused with lower-trust text. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **missing clarification**. The assistant produces a plausible response but guesses when an essential detail is unknown. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare the final answer against an explicit requirements checklist and the original conversation. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Before answering, identify the applicable task constraints and follow them. Ask only when a missing detail prevents a reliable answer. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for missing clarification.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide three concrete constraints and one irrelevant distraction; score every constraint independently.

**Starter test input:** Follow these constraints: 60 words maximum, no bullets, include one limitation.

**Expected check:** All three constraints satisfied. Adapt this starter case to isolate **missing clarification**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 40. Unnecessary clarification

**Definition:** Asks questions despite having enough information.

**Why it can happen:** Important constraints can be overlooked, misunderstood, displaced by long context, or confused with lower-trust text. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **unnecessary clarification**. The assistant produces a plausible response but asks questions despite having enough information. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Compare the final answer against an explicit requirements checklist and the original conversation. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Before answering, identify the applicable task constraints and follow them. Ask only when a missing detail prevents a reliable answer. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for unnecessary clarification.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide three concrete constraints and one irrelevant distraction; score every constraint independently.

**Starter test input:** Follow these constraints: 60 words maximum, no bullets, include one limitation.

**Expected check:** All three constraints satisfied. Adapt this starter case to isolate **unnecessary clarification**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

