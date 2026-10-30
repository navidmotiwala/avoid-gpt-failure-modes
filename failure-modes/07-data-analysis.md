# Data and analysis

[Back to README](../README.md) | [Evaluation protocol](../evaluations/PROTOCOL.md)

This chapter expands failure modes 61–70. The examples below are **constructed test scenarios**, not observed failures. A model's behavior must be measured before claiming that a particular model fails any test.

**Common investigation approach:** Recompute from source rows or a trusted calculator and document denominators, date windows and assumptions.

## 61. Incorrect calculations

**Definition:** Gets totals, ratios, or differences wrong.

**Why it can happen:** Incorrect metric definitions, units, denominator choices, missing values or arithmetic can distort conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **incorrect calculations**. The assistant produces a plausible response but gets totals, ratios, or differences wrong. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Recompute from source rows or a trusted calculator and document denominators, date windows and assumptions. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Show the formula, define each metric, check units and recompute important numbers independently. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for incorrect calculations.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Supply a tiny dataset with a known result and an intentional trap involving denominators, missing values or units.

**Starter test input:** Calculate conversion rate for 18 conversions from 240 visits.

**Expected check:** 7.5%, with denominator and formula. Adapt this starter case to isolate **incorrect calculations**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 62. Misleading percentages

**Definition:** Uses incorrect denominators or baselines.

**Why it can happen:** Incorrect metric definitions, units, denominator choices, missing values or arithmetic can distort conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **misleading percentages**. The assistant produces a plausible response but uses incorrect denominators or baselines. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Recompute from source rows or a trusted calculator and document denominators, date windows and assumptions. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Show the formula, define each metric, check units and recompute important numbers independently. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for misleading percentages.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Supply a tiny dataset with a known result and an intentional trap involving denominators, missing values or units.

**Starter test input:** Calculate conversion rate for 18 conversions from 240 visits.

**Expected check:** 7.5%, with denominator and formula. Adapt this starter case to isolate **misleading percentages**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 63. Data misinterpretation

**Definition:** Draws conclusions not supported by data.

**Why it can happen:** Incorrect metric definitions, units, denominator choices, missing values or arithmetic can distort conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **data misinterpretation**. The assistant produces a plausible response but draws conclusions not supported by data. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Recompute from source rows or a trusted calculator and document denominators, date windows and assumptions. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Show the formula, define each metric, check units and recompute important numbers independently. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for data misinterpretation.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Supply a tiny dataset with a known result and an intentional trap involving denominators, missing values or units.

**Starter test input:** Calculate conversion rate for 18 conversions from 240 visits.

**Expected check:** 7.5%, with denominator and formula. Adapt this starter case to isolate **data misinterpretation**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 64. Invalid comparisons

**Definition:** Compares unlike populations or periods.

**Why it can happen:** Incorrect metric definitions, units, denominator choices, missing values or arithmetic can distort conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **invalid comparisons**. The assistant produces a plausible response but compares unlike populations or periods. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Recompute from source rows or a trusted calculator and document denominators, date windows and assumptions. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Show the formula, define each metric, check units and recompute important numbers independently. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for invalid comparisons.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Supply a tiny dataset with a known result and an intentional trap involving denominators, missing values or units.

**Starter test input:** Calculate conversion rate for 18 conversions from 240 visits.

**Expected check:** 7.5%, with denominator and formula. Adapt this starter case to isolate **invalid comparisons**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 65. Hidden missing-data assumptions

**Definition:** Fills gaps without disclosure.

**Why it can happen:** Incorrect metric definitions, units, denominator choices, missing values or arithmetic can distort conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **hidden missing-data assumptions**. The assistant produces a plausible response but fills gaps without disclosure. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Recompute from source rows or a trusted calculator and document denominators, date windows and assumptions. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Show the formula, define each metric, check units and recompute important numbers independently. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for hidden missing-data assumptions.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Supply a tiny dataset with a known result and an intentional trap involving denominators, missing values or units.

**Starter test input:** Calculate conversion rate for 18 conversions from 240 visits.

**Expected check:** 7.5%, with denominator and formula. Adapt this starter case to isolate **hidden missing-data assumptions**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 66. Statistical misunderstandings

**Definition:** Misuses averages, significance, or uncertainty.

**Why it can happen:** Incorrect metric definitions, units, denominator choices, missing values or arithmetic can distort conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **statistical misunderstandings**. The assistant produces a plausible response but misuses averages, significance, or uncertainty. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Recompute from source rows or a trusted calculator and document denominators, date windows and assumptions. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Show the formula, define each metric, check units and recompute important numbers independently. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for statistical misunderstandings.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Supply a tiny dataset with a known result and an intentional trap involving denominators, missing values or units.

**Starter test input:** Calculate conversion rate for 18 conversions from 240 visits.

**Expected check:** 7.5%, with denominator and formula. Adapt this starter case to isolate **statistical misunderstandings**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 67. Inconsistent units

**Definition:** Mixes currencies, timeframes, or measurement scales.

**Why it can happen:** Incorrect metric definitions, units, denominator choices, missing values or arithmetic can distort conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **inconsistent units**. The assistant produces a plausible response but mixes currencies, timeframes, or measurement scales. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Recompute from source rows or a trusted calculator and document denominators, date windows and assumptions. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Show the formula, define each metric, check units and recompute important numbers independently. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for inconsistent units.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Supply a tiny dataset with a known result and an intentional trap involving denominators, missing values or units.

**Starter test input:** Calculate conversion rate for 18 conversions from 240 visits.

**Expected check:** 7.5%, with denominator and formula. Adapt this starter case to isolate **inconsistent units**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 68. Wrong metric definitions

**Definition:** Confuses metrics with different meanings.

**Why it can happen:** Incorrect metric definitions, units, denominator choices, missing values or arithmetic can distort conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **wrong metric definitions**. The assistant produces a plausible response but confuses metrics with different meanings. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Recompute from source rows or a trusted calculator and document denominators, date windows and assumptions. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Show the formula, define each metric, check units and recompute important numbers independently. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for wrong metric definitions.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Supply a tiny dataset with a known result and an intentional trap involving denominators, missing values or units.

**Starter test input:** Calculate conversion rate for 18 conversions from 240 visits.

**Expected check:** 7.5%, with denominator and formula. Adapt this starter case to isolate **wrong metric definitions**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 69. Unjustified forecasts

**Definition:** Makes projections without defensible assumptions.

**Why it can happen:** Incorrect metric definitions, units, denominator choices, missing values or arithmetic can distort conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **unjustified forecasts**. The assistant produces a plausible response but makes projections without defensible assumptions. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Recompute from source rows or a trusted calculator and document denominators, date windows and assumptions. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Show the formula, define each metric, check units and recompute important numbers independently. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for unjustified forecasts.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Supply a tiny dataset with a known result and an intentional trap involving denominators, missing values or units.

**Starter test input:** Calculate conversion rate for 18 conversions from 240 visits.

**Expected check:** 7.5%, with denominator and formula. Adapt this starter case to isolate **unjustified forecasts**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 70. Unsupported predictions

**Definition:** Treats speculation as a likely outcome.

**Why it can happen:** Incorrect metric definitions, units, denominator choices, missing values or arithmetic can distort conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **unsupported predictions**. The assistant produces a plausible response but treats speculation as a likely outcome. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Recompute from source rows or a trusted calculator and document denominators, date windows and assumptions. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Show the formula, define each metric, check units and recompute important numbers independently. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for unsupported predictions.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Supply a tiny dataset with a known result and an intentional trap involving denominators, missing values or units.

**Starter test input:** Calculate conversion rate for 18 conversions from 240 visits.

**Expected check:** 7.5%, with denominator and formula. Adapt this starter case to isolate **unsupported predictions**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

