# Reasoning and logic

[Back to README](../README.md) | [Evaluation protocol](../evaluations/PROTOCOL.md)

This chapter expands failure modes 11–20. The examples below are **constructed test scenarios**, not observed failures. A model's behavior must be measured before claiming that a particular model fails any test.

**Common investigation approach:** Write down the premises, inference steps, counterexamples and independently verified conclusion.

## 11. Logical fallacies

**Definition:** Draws conclusions using invalid reasoning.

**Why it can happen:** The response may skip intermediate checks, use an invalid inference, or carry a false premise into later conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **logical fallacies**. The assistant produces a plausible response but draws conclusions using invalid reasoning. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Write down the premises, inference steps, counterexamples and independently verified conclusion. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Check premises and intermediate results. Look for counterexamples before making the final claim. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for logical fallacies.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Create a small case with a known answer; ask for the conclusion, then check each premise and intermediate result.

**Starter test input:** A value increased from 100 to 120. Is the increase 120%?

**Expected check:** Correct calculation: 20% increase; reject the false premise. Adapt this starter case to isolate **logical fallacies**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 12. Circular reasoning

**Definition:** Uses the conclusion as its own support.

**Why it can happen:** The response may skip intermediate checks, use an invalid inference, or carry a false premise into later conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **circular reasoning**. The assistant produces a plausible response but uses the conclusion as its own support. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Write down the premises, inference steps, counterexamples and independently verified conclusion. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Check premises and intermediate results. Look for counterexamples before making the final claim. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for circular reasoning.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Create a small case with a known answer; ask for the conclusion, then check each premise and intermediate result.

**Starter test input:** A value increased from 100 to 120. Is the increase 120%?

**Expected check:** Correct calculation: 20% increase; reject the false premise. Adapt this starter case to isolate **circular reasoning**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 13. False assumptions

**Definition:** Builds an answer on an unverified premise.

**Why it can happen:** The response may skip intermediate checks, use an invalid inference, or carry a false premise into later conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **false assumptions**. The assistant produces a plausible response but builds an answer on an unverified premise. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Write down the premises, inference steps, counterexamples and independently verified conclusion. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Check premises and intermediate results. Look for counterexamples before making the final claim. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for false assumptions.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Create a small case with a known answer; ask for the conclusion, then check each premise and intermediate result.

**Starter test input:** A value increased from 100 to 120. Is the increase 120%?

**Expected check:** Correct calculation: 20% increase; reject the false premise. Adapt this starter case to isolate **false assumptions**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 14. Premature conclusions

**Definition:** Decides before evaluating enough evidence.

**Why it can happen:** The response may skip intermediate checks, use an invalid inference, or carry a false premise into later conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **premature conclusions**. The assistant produces a plausible response but decides before evaluating enough evidence. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Write down the premises, inference steps, counterexamples and independently verified conclusion. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Check premises and intermediate results. Look for counterexamples before making the final claim. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for premature conclusions.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Create a small case with a known answer; ask for the conclusion, then check each premise and intermediate result.

**Starter test input:** A value increased from 100 to 120. Is the increase 120%?

**Expected check:** Correct calculation: 20% increase; reject the false premise. Adapt this starter case to isolate **premature conclusions**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 15. Correlation–causation confusion

**Definition:** Treats association as proof of cause.

**Why it can happen:** The response may skip intermediate checks, use an invalid inference, or carry a false premise into later conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **correlation–causation confusion**. The assistant produces a plausible response but treats association as proof of cause. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Write down the premises, inference steps, counterexamples and independently verified conclusion. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Check premises and intermediate results. Look for counterexamples before making the final claim. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for correlation–causation confusion.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Create a small case with a known answer; ask for the conclusion, then check each premise and intermediate result.

**Starter test input:** A value increased from 100 to 120. Is the increase 120%?

**Expected check:** Correct calculation: 20% increase; reject the false premise. Adapt this starter case to isolate **correlation–causation confusion**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 16. Contradictory reasoning

**Definition:** Makes claims that cannot all be true.

**Why it can happen:** The response may skip intermediate checks, use an invalid inference, or carry a false premise into later conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **contradictory reasoning**. The assistant produces a plausible response but makes claims that cannot all be true. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Write down the premises, inference steps, counterexamples and independently verified conclusion. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Check premises and intermediate results. Look for counterexamples before making the final claim. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for contradictory reasoning.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Create a small case with a known answer; ask for the conclusion, then check each premise and intermediate result.

**Starter test input:** A value increased from 100 to 120. Is the increase 120%?

**Expected check:** Correct calculation: 20% increase; reject the false premise. Adapt this starter case to isolate **contradictory reasoning**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 17. Missing intermediate steps

**Definition:** Skips reasoning needed to support a result.

**Why it can happen:** The response may skip intermediate checks, use an invalid inference, or carry a false premise into later conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **missing intermediate steps**. The assistant produces a plausible response but skips reasoning needed to support a result. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Write down the premises, inference steps, counterexamples and independently verified conclusion. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Check premises and intermediate results. Look for counterexamples before making the final claim. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for missing intermediate steps.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Create a small case with a known answer; ask for the conclusion, then check each premise and intermediate result.

**Starter test input:** A value increased from 100 to 120. Is the increase 120%?

**Expected check:** Correct calculation: 20% increase; reject the false premise. Adapt this starter case to isolate **missing intermediate steps**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 18. Calculation errors

**Definition:** Produces incorrect arithmetic or formulas.

**Why it can happen:** The response may skip intermediate checks, use an invalid inference, or carry a false premise into later conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **calculation errors**. The assistant produces a plausible response but produces incorrect arithmetic or formulas. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Write down the premises, inference steps, counterexamples and independently verified conclusion. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Check premises and intermediate results. Look for counterexamples before making the final claim. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for calculation errors.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Create a small case with a known answer; ask for the conclusion, then check each premise and intermediate result.

**Starter test input:** A value increased from 100 to 120. Is the increase 120%?

**Expected check:** Correct calculation: 20% increase; reject the false premise. Adapt this starter case to isolate **calculation errors**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 19. Oversimplification

**Definition:** Ignores important complexity or exceptions.

**Why it can happen:** The response may skip intermediate checks, use an invalid inference, or carry a false premise into later conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **oversimplification**. The assistant produces a plausible response but ignores important complexity or exceptions. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Write down the premises, inference steps, counterexamples and independently verified conclusion. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Check premises and intermediate results. Look for counterexamples before making the final claim. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for oversimplification.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Create a small case with a known answer; ask for the conclusion, then check each premise and intermediate result.

**Starter test input:** A value increased from 100 to 120. Is the increase 120%?

**Expected check:** Correct calculation: 20% increase; reject the false premise. Adapt this starter case to isolate **oversimplification**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 20. Missed counterexamples

**Definition:** Fails to test whether a claim has exceptions.

**Why it can happen:** The response may skip intermediate checks, use an invalid inference, or carry a false premise into later conclusions. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **missed counterexamples**. The assistant produces a plausible response but fails to test whether a claim has exceptions. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Write down the premises, inference steps, counterexamples and independently verified conclusion. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Check premises and intermediate results. Look for counterexamples before making the final claim. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for missed counterexamples.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Create a small case with a known answer; ask for the conclusion, then check each premise and intermediate result.

**Starter test input:** A value increased from 100 to 120. Is the increase 120%?

**Expected check:** Correct calculation: 20% increase; reject the false premise. Adapt this starter case to isolate **missed counterexamples**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

