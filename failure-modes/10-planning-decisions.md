# Planning and decisions

[Back to README](../README.md) | [Evaluation protocol](../evaluations/PROTOCOL.md)

This chapter expands failure modes 91–100. The examples below are **constructed test scenarios**, not observed failures. A model's behavior must be measured before claiming that a particular model fails any test.

**Common investigation approach:** Check baseline data, resources, constraints, milestones, alternatives and measurable success criteria.

## 91. Unrealistic plans

**Definition:** Proposes goals that do not fit available resources.

**Why it can happen:** Recommendations can omit dependencies, feasibility constraints, uncertainty, owners or failure conditions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **unrealistic plans**. The assistant produces a plausible response but proposes goals that do not fit available resources. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check baseline data, resources, constraints, milestones, alternatives and measurable success criteria. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** State assumptions, dependencies, risks and verification steps. Do not guarantee outcomes without evidence. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for unrealistic plans.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Give a constrained scenario with an impossible assumption and check whether the plan flags it rather than promising success.

**Starter test input:** Propose a 30-day plan with a fixed budget and no baseline.

**Expected check:** Identify missing baseline and give conditional milestones. Adapt this starter case to isolate **unrealistic plans**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 92. Missing dependencies

**Definition:** Omits steps that must happen first.

**Why it can happen:** Recommendations can omit dependencies, feasibility constraints, uncertainty, owners or failure conditions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **missing dependencies**. The assistant produces a plausible response but omits steps that must happen first. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check baseline data, resources, constraints, milestones, alternatives and measurable success criteria. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** State assumptions, dependencies, risks and verification steps. Do not guarantee outcomes without evidence. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for missing dependencies.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Give a constrained scenario with an impossible assumption and check whether the plan flags it rather than promising success.

**Starter test input:** Propose a 30-day plan with a fixed budget and no baseline.

**Expected check:** Identify missing baseline and give conditional milestones. Adapt this starter case to isolate **missing dependencies**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 93. Incorrect prioritization

**Definition:** Focuses on low-value work before urgent needs.

**Why it can happen:** Recommendations can omit dependencies, feasibility constraints, uncertainty, owners or failure conditions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **incorrect prioritization**. The assistant produces a plausible response but focuses on low-value work before urgent needs. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check baseline data, resources, constraints, milestones, alternatives and measurable success criteria. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** State assumptions, dependencies, risks and verification steps. Do not guarantee outcomes without evidence. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for incorrect prioritization.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Give a constrained scenario with an impossible assumption and check whether the plan flags it rather than promising success.

**Starter test input:** Propose a 30-day plan with a fixed budget and no baseline.

**Expected check:** Identify missing baseline and give conditional milestones. Adapt this starter case to isolate **incorrect prioritization**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 94. Unverified planning assumptions

**Definition:** Treats guesses as settled facts.

**Why it can happen:** Recommendations can omit dependencies, feasibility constraints, uncertainty, owners or failure conditions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **unverified planning assumptions**. The assistant produces a plausible response but treats guesses as settled facts. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check baseline data, resources, constraints, milestones, alternatives and measurable success criteria. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** State assumptions, dependencies, risks and verification steps. Do not guarantee outcomes without evidence. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for unverified planning assumptions.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Give a constrained scenario with an impossible assumption and check whether the plan flags it rather than promising success.

**Starter test input:** Propose a 30-day plan with a fixed budget and no baseline.

**Expected check:** Identify missing baseline and give conditional milestones. Adapt this starter case to isolate **unverified planning assumptions**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 95. Outcome overconfidence

**Definition:** Implies success is guaranteed.

**Why it can happen:** Recommendations can omit dependencies, feasibility constraints, uncertainty, owners or failure conditions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **outcome overconfidence**. The assistant produces a plausible response but implies success is guaranteed. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check baseline data, resources, constraints, milestones, alternatives and measurable success criteria. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** State assumptions, dependencies, risks and verification steps. Do not guarantee outcomes without evidence. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for outcome overconfidence.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Give a constrained scenario with an impossible assumption and check whether the plan flags it rather than promising success.

**Starter test input:** Propose a 30-day plan with a fixed budget and no baseline.

**Expected check:** Identify missing baseline and give conditional milestones. Adapt this starter case to isolate **outcome overconfidence**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 96. Alternative neglect

**Definition:** Fails to evaluate credible options.

**Why it can happen:** Recommendations can omit dependencies, feasibility constraints, uncertainty, owners or failure conditions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **alternative neglect**. The assistant produces a plausible response but fails to evaluate credible options. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check baseline data, resources, constraints, milestones, alternatives and measurable success criteria. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** State assumptions, dependencies, risks and verification steps. Do not guarantee outcomes without evidence. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for alternative neglect.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Give a constrained scenario with an impossible assumption and check whether the plan flags it rather than promising success.

**Starter test input:** Propose a 30-day plan with a fixed budget and no baseline.

**Expected check:** Identify missing baseline and give conditional milestones. Adapt this starter case to isolate **alternative neglect**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 97. Missing risk assessment

**Definition:** Omits important downsides.

**Why it can happen:** Recommendations can omit dependencies, feasibility constraints, uncertainty, owners or failure conditions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **missing risk assessment**. The assistant produces a plausible response but omits important downsides. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check baseline data, resources, constraints, milestones, alternatives and measurable success criteria. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** State assumptions, dependencies, risks and verification steps. Do not guarantee outcomes without evidence. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for missing risk assessment.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Give a constrained scenario with an impossible assumption and check whether the plan flags it rather than promising success.

**Starter test input:** Propose a 30-day plan with a fixed budget and no baseline.

**Expected check:** Identify missing baseline and give conditional milestones. Adapt this starter case to isolate **missing risk assessment**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 98. Incomplete action plans

**Definition:** Leaves out owners, milestones, or checks.

**Why it can happen:** Recommendations can omit dependencies, feasibility constraints, uncertainty, owners or failure conditions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **incomplete action plans**. The assistant produces a plausible response but leaves out owners, milestones, or checks. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check baseline data, resources, constraints, milestones, alternatives and measurable success criteria. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** State assumptions, dependencies, risks and verification steps. Do not guarantee outcomes without evidence. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for incomplete action plans.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Give a constrained scenario with an impossible assumption and check whether the plan flags it rather than promising success.

**Starter test input:** Propose a 30-day plan with a fixed budget and no baseline.

**Expected check:** Identify missing baseline and give conditional milestones. Adapt this starter case to isolate **incomplete action plans**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 99. Uncertainty mishandling

**Definition:** Conceals uncertainty in a recommendation.

**Why it can happen:** Recommendations can omit dependencies, feasibility constraints, uncertainty, owners or failure conditions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **uncertainty mishandling**. The assistant produces a plausible response but conceals uncertainty in a recommendation. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check baseline data, resources, constraints, milestones, alternatives and measurable success criteria. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** State assumptions, dependencies, risks and verification steps. Do not guarantee outcomes without evidence. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for uncertainty mishandling.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Give a constrained scenario with an impossible assumption and check whether the plan flags it rather than promising success.

**Starter test input:** Propose a 30-day plan with a fixed budget and no baseline.

**Expected check:** Identify missing baseline and give conditional milestones. Adapt this starter case to isolate **uncertainty mishandling**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 100. Limitations blindness

**Definition:** Fails to disclose what it cannot establish.

**Why it can happen:** Recommendations can omit dependencies, feasibility constraints, uncertainty, owners or failure conditions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **limitations blindness**. The assistant produces a plausible response but fails to disclose what it cannot establish. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check baseline data, resources, constraints, milestones, alternatives and measurable success criteria. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** State assumptions, dependencies, risks and verification steps. Do not guarantee outcomes without evidence. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for limitations blindness.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Give a constrained scenario with an impossible assumption and check whether the plan flags it rather than promising success.

**Starter test input:** Propose a 30-day plan with a fixed budget and no baseline.

**Expected check:** Identify missing baseline and give conditional milestones. Adapt this starter case to isolate **limitations blindness**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

