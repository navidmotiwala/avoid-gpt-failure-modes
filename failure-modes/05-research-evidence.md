# Research and evidence

[Back to README](../README.md) | [Evaluation protocol](../evaluations/PROTOCOL.md)

This chapter expands failure modes 41–50. The examples below are **constructed test scenarios**, not observed failures. A model's behavior must be measured before claiming that a particular model fails any test.

**Common investigation approach:** Open original publications, verify quotations and inspect whether each source actually supports its attached claim.

## 41. Fabricated sources

**Definition:** Invents research or documents.

**Why it can happen:** Retrieved snippets, citations and paraphrases may be mistaken for direct proof; the model can blend sources or overstate what they show. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **fabricated sources**. The assistant produces a plausible response but invents research or documents. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Open original publications, verify quotations and inspect whether each source actually supports its attached claim. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Tie each factual claim to a relevant original source. Distinguish the source's finding from your interpretation. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for fabricated sources.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a source with a narrow conclusion and ask a broader question; check whether the response overstates the evidence.

**Starter test input:** Does the cited article actually support the stated conclusion?

**Expected check:** Quote or pinpoint relevant evidence; otherwise mark unsupported. Adapt this starter case to isolate **fabricated sources**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 42. Broken references

**Definition:** Supplies links that do not resolve.

**Why it can happen:** Retrieved snippets, citations and paraphrases may be mistaken for direct proof; the model can blend sources or overstate what they show. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **broken references**. The assistant produces a plausible response but supplies links that do not resolve. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Open original publications, verify quotations and inspect whether each source actually supports its attached claim. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Tie each factual claim to a relevant original source. Distinguish the source's finding from your interpretation. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for broken references.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a source with a narrow conclusion and ask a broader question; check whether the response overstates the evidence.

**Starter test input:** Does the cited article actually support the stated conclusion?

**Expected check:** Quote or pinpoint relevant evidence; otherwise mark unsupported. Adapt this starter case to isolate **broken references**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 43. Misrepresented studies

**Definition:** Overstates or distorts findings.

**Why it can happen:** Retrieved snippets, citations and paraphrases may be mistaken for direct proof; the model can blend sources or overstate what they show. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **misrepresented studies**. The assistant produces a plausible response but overstates or distorts findings. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Open original publications, verify quotations and inspect whether each source actually supports its attached claim. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Tie each factual claim to a relevant original source. Distinguish the source's finding from your interpretation. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for misrepresented studies.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a source with a narrow conclusion and ask a broader question; check whether the response overstates the evidence.

**Starter test input:** Does the cited article actually support the stated conclusion?

**Expected check:** Quote or pinpoint relevant evidence; otherwise mark unsupported. Adapt this starter case to isolate **misrepresented studies**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 44. Incorrect quotations

**Definition:** Changes or invents quoted text.

**Why it can happen:** Retrieved snippets, citations and paraphrases may be mistaken for direct proof; the model can blend sources or overstate what they show. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **incorrect quotations**. The assistant produces a plausible response but changes or invents quoted text. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Open original publications, verify quotations and inspect whether each source actually supports its attached claim. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Tie each factual claim to a relevant original source. Distinguish the source's finding from your interpretation. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for incorrect quotations.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a source with a narrow conclusion and ask a broader question; check whether the response overstates the evidence.

**Starter test input:** Does the cited article actually support the stated conclusion?

**Expected check:** Quote or pinpoint relevant evidence; otherwise mark unsupported. Adapt this starter case to isolate **incorrect quotations**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 45. Cherry-picked evidence

**Definition:** Omits evidence that challenges a claim.

**Why it can happen:** Retrieved snippets, citations and paraphrases may be mistaken for direct proof; the model can blend sources or overstate what they show. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **cherry-picked evidence**. The assistant produces a plausible response but omits evidence that challenges a claim. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Open original publications, verify quotations and inspect whether each source actually supports its attached claim. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Tie each factual claim to a relevant original source. Distinguish the source's finding from your interpretation. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for cherry-picked evidence.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a source with a narrow conclusion and ask a broader question; check whether the response overstates the evidence.

**Starter test input:** Does the cited article actually support the stated conclusion?

**Expected check:** Quote or pinpoint relevant evidence; otherwise mark unsupported. Adapt this starter case to isolate **cherry-picked evidence**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 46. Missing source verification

**Definition:** Does not confirm that a source exists.

**Why it can happen:** Retrieved snippets, citations and paraphrases may be mistaken for direct proof; the model can blend sources or overstate what they show. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **missing source verification**. The assistant produces a plausible response but does not confirm that a source exists. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Open original publications, verify quotations and inspect whether each source actually supports its attached claim. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Tie each factual claim to a relevant original source. Distinguish the source's finding from your interpretation. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for missing source verification.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a source with a narrow conclusion and ask a broader question; check whether the response overstates the evidence.

**Starter test input:** Does the cited article actually support the stated conclusion?

**Expected check:** Quote or pinpoint relevant evidence; otherwise mark unsupported. Adapt this starter case to isolate **missing source verification**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 47. Evidence inflation

**Definition:** Presents weak evidence as decisive.

**Why it can happen:** Retrieved snippets, citations and paraphrases may be mistaken for direct proof; the model can blend sources or overstate what they show. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **evidence inflation**. The assistant produces a plausible response but presents weak evidence as decisive. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Open original publications, verify quotations and inspect whether each source actually supports its attached claim. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Tie each factual claim to a relevant original source. Distinguish the source's finding from your interpretation. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for evidence inflation.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a source with a narrow conclusion and ask a broader question; check whether the response overstates the evidence.

**Starter test input:** Does the cited article actually support the stated conclusion?

**Expected check:** Quote or pinpoint relevant evidence; otherwise mark unsupported. Adapt this starter case to isolate **evidence inflation**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 48. Unsupported comparisons

**Definition:** Compares items without comparable data.

**Why it can happen:** Retrieved snippets, citations and paraphrases may be mistaken for direct proof; the model can blend sources or overstate what they show. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **unsupported comparisons**. The assistant produces a plausible response but compares items without comparable data. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Open original publications, verify quotations and inspect whether each source actually supports its attached claim. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Tie each factual claim to a relevant original source. Distinguish the source's finding from your interpretation. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for unsupported comparisons.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a source with a narrow conclusion and ask a broader question; check whether the response overstates the evidence.

**Starter test input:** Does the cited article actually support the stated conclusion?

**Expected check:** Quote or pinpoint relevant evidence; otherwise mark unsupported. Adapt this starter case to isolate **unsupported comparisons**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 49. Stale research

**Definition:** Uses evidence that no longer answers the question.

**Why it can happen:** Retrieved snippets, citations and paraphrases may be mistaken for direct proof; the model can blend sources or overstate what they show. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **stale research**. The assistant produces a plausible response but uses evidence that no longer answers the question. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Open original publications, verify quotations and inspect whether each source actually supports its attached claim. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Tie each factual claim to a relevant original source. Distinguish the source's finding from your interpretation. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for stale research.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a source with a narrow conclusion and ask a broader question; check whether the response overstates the evidence.

**Starter test input:** Does the cited article actually support the stated conclusion?

**Expected check:** Quote or pinpoint relevant evidence; otherwise mark unsupported. Adapt this starter case to isolate **stale research**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 50. Fact–opinion confusion

**Definition:** Presents judgments as established facts.

**Why it can happen:** Retrieved snippets, citations and paraphrases may be mistaken for direct proof; the model can blend sources or overstate what they show. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **fact–opinion confusion**. The assistant produces a plausible response but presents judgments as established facts. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Open original publications, verify quotations and inspect whether each source actually supports its attached claim. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Tie each factual claim to a relevant original source. Distinguish the source's finding from your interpretation. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for fact–opinion confusion.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a source with a narrow conclusion and ask a broader question; check whether the response overstates the evidence.

**Starter test input:** Does the cited article actually support the stated conclusion?

**Expected check:** Quote or pinpoint relevant evidence; otherwise mark unsupported. Adapt this starter case to isolate **fact–opinion confusion**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

