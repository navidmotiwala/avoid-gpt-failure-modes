# Accuracy and factual errors

[Back to README](../README.md) | [Evaluation protocol](../evaluations/PROTOCOL.md)

This chapter expands failure modes 1–10. The examples below are **constructed test scenarios**, not observed failures. A model's behavior must be measured before claiming that a particular model fails any test.

**Common investigation approach:** Locate the original primary record and compare the exact claim, name, number, date and scope.

## 1. Hallucination

**Definition:** Generates false or unsupported information.

**Why it can happen:** The model may rely on learned associations instead of checking a primary source. Retrieval, source quality, ambiguous entities and missing dates can also contribute. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **hallucination**. The assistant produces a plausible response but generates false or unsupported information. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Locate the original primary record and compare the exact claim, name, number, date and scope. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not assert facts that are unsupported by available evidence. Label unverified statements, and abstain when the answer cannot be established. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for hallucination.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Ask for the source of each checkable claim; independently open the original source and record whether it supports the statement.

**Starter test input:** What is the exact publication date and primary source for this claim?

**Expected check:** Verified date, authentic source or an explicit inability to verify. Adapt this starter case to isolate **hallucination**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 2. Fabricated facts

**Definition:** Invents details about events, people, or products.

**Why it can happen:** The model may rely on learned associations instead of checking a primary source. Retrieval, source quality, ambiguous entities and missing dates can also contribute. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **fabricated facts**. The assistant produces a plausible response but invents details about events, people, or products. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Locate the original primary record and compare the exact claim, name, number, date and scope. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not assert facts that are unsupported by available evidence. Label unverified statements, and abstain when the answer cannot be established. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for fabricated facts.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Ask for the source of each checkable claim; independently open the original source and record whether it supports the statement.

**Starter test input:** What is the exact publication date and primary source for this claim?

**Expected check:** Verified date, authentic source or an explicit inability to verify. Adapt this starter case to isolate **fabricated facts**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 3. Invented statistics

**Definition:** Provides numbers without evidence.

**Why it can happen:** The model may rely on learned associations instead of checking a primary source. Retrieval, source quality, ambiguous entities and missing dates can also contribute. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **invented statistics**. The assistant produces a plausible response but provides numbers without evidence. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Locate the original primary record and compare the exact claim, name, number, date and scope. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not assert facts that are unsupported by available evidence. Label unverified statements, and abstain when the answer cannot be established. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for invented statistics.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Ask for the source of each checkable claim; independently open the original source and record whether it supports the statement.

**Starter test input:** What is the exact publication date and primary source for this claim?

**Expected check:** Verified date, authentic source or an explicit inability to verify. Adapt this starter case to isolate **invented statistics**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 4. Fake citations

**Definition:** Makes up publications, URLs, or references.

**Why it can happen:** The model may rely on learned associations instead of checking a primary source. Retrieval, source quality, ambiguous entities and missing dates can also contribute. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **fake citations**. The assistant produces a plausible response but makes up publications, URLs, or references. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Locate the original primary record and compare the exact claim, name, number, date and scope. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not assert facts that are unsupported by available evidence. Label unverified statements, and abstain when the answer cannot be established. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for fake citations.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Ask for the source of each checkable claim; independently open the original source and record whether it supports the statement.

**Starter test input:** What is the exact publication date and primary source for this claim?

**Expected check:** Verified date, authentic source or an explicit inability to verify. Adapt this starter case to isolate **fake citations**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 5. Outdated information

**Definition:** Treats old facts as current.

**Why it can happen:** The model may rely on learned associations instead of checking a primary source. Retrieval, source quality, ambiguous entities and missing dates can also contribute. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **outdated information**. The assistant produces a plausible response but treats old facts as current. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Locate the original primary record and compare the exact claim, name, number, date and scope. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not assert facts that are unsupported by available evidence. Label unverified statements, and abstain when the answer cannot be established. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for outdated information.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Ask for the source of each checkable claim; independently open the original source and record whether it supports the statement.

**Starter test input:** What is the exact publication date and primary source for this claim?

**Expected check:** Verified date, authentic source or an explicit inability to verify. Adapt this starter case to isolate **outdated information**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 6. Unsupported claims

**Definition:** States conclusions without sufficient support.

**Why it can happen:** The model may rely on learned associations instead of checking a primary source. Retrieval, source quality, ambiguous entities and missing dates can also contribute. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **unsupported claims**. The assistant produces a plausible response but states conclusions without sufficient support. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Locate the original primary record and compare the exact claim, name, number, date and scope. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not assert facts that are unsupported by available evidence. Label unverified statements, and abstain when the answer cannot be established. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for unsupported claims.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Ask for the source of each checkable claim; independently open the original source and record whether it supports the statement.

**Starter test input:** What is the exact publication date and primary source for this claim?

**Expected check:** Verified date, authentic source or an explicit inability to verify. Adapt this starter case to isolate **unsupported claims**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 7. False precision

**Definition:** Gives overly exact figures despite uncertainty.

**Why it can happen:** The model may rely on learned associations instead of checking a primary source. Retrieval, source quality, ambiguous entities and missing dates can also contribute. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **false precision**. The assistant produces a plausible response but gives overly exact figures despite uncertainty. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Locate the original primary record and compare the exact claim, name, number, date and scope. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not assert facts that are unsupported by available evidence. Label unverified statements, and abstain when the answer cannot be established. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for false precision.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Ask for the source of each checkable claim; independently open the original source and record whether it supports the statement.

**Starter test input:** What is the exact publication date and primary source for this claim?

**Expected check:** Verified date, authentic source or an explicit inability to verify. Adapt this starter case to isolate **false precision**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 8. Incorrect attribution

**Definition:** Credits a statement or work to the wrong source.

**Why it can happen:** The model may rely on learned associations instead of checking a primary source. Retrieval, source quality, ambiguous entities and missing dates can also contribute. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **incorrect attribution**. The assistant produces a plausible response but credits a statement or work to the wrong source. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Locate the original primary record and compare the exact claim, name, number, date and scope. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not assert facts that are unsupported by available evidence. Label unverified statements, and abstain when the answer cannot be established. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for incorrect attribution.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Ask for the source of each checkable claim; independently open the original source and record whether it supports the statement.

**Starter test input:** What is the exact publication date and primary source for this claim?

**Expected check:** Verified date, authentic source or an explicit inability to verify. Adapt this starter case to isolate **incorrect attribution**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 9. Misleading summaries

**Definition:** Changes the meaning of source material.

**Why it can happen:** The model may rely on learned associations instead of checking a primary source. Retrieval, source quality, ambiguous entities and missing dates can also contribute. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **misleading summaries**. The assistant produces a plausible response but changes the meaning of source material. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Locate the original primary record and compare the exact claim, name, number, date and scope. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not assert facts that are unsupported by available evidence. Label unverified statements, and abstain when the answer cannot be established. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for misleading summaries.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Ask for the source of each checkable claim; independently open the original source and record whether it supports the statement.

**Starter test input:** What is the exact publication date and primary source for this claim?

**Expected check:** Verified date, authentic source or an explicit inability to verify. Adapt this starter case to isolate **misleading summaries**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 10. Confidently incorrect answers

**Definition:** Expresses unjustified certainty.

**Why it can happen:** The model may rely on learned associations instead of checking a primary source. Retrieval, source quality, ambiguous entities and missing dates can also contribute. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **confidently incorrect answers**. The assistant produces a plausible response but expresses unjustified certainty. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Locate the original primary record and compare the exact claim, name, number, date and scope. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not assert facts that are unsupported by available evidence. Label unverified statements, and abstain when the answer cannot be established. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for confidently incorrect answers.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Ask for the source of each checkable claim; independently open the original source and record whether it supports the statement.

**Starter test input:** What is the exact publication date and primary source for this claim?

**Expected check:** Verified date, authentic source or an explicit inability to verify. Adapt this starter case to isolate **confidently incorrect answers**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

