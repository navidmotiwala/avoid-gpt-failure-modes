# Coding and technical work

[Back to README](../README.md) | [Evaluation protocol](../evaluations/PROTOCOL.md)

This chapter expands failure modes 71–80. The examples below are **constructed test scenarios**, not observed failures. A model's behavior must be measured before claiming that a particular model fails any test.

**Common investigation approach:** Check current official documentation, execute tests in a controlled environment and review errors and security implications.

## 71. Nonexistent APIs

**Definition:** Invents endpoints, functions, or parameters.

**Why it can happen:** The model may infer APIs from naming patterns, assume dependencies, overlook edge cases or produce code without running it. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **nonexistent apis**. The assistant produces a plausible response but invents endpoints, functions, or parameters. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check current official documentation, execute tests in a controlled environment and review errors and security implications. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not invent APIs. State environment assumptions, use documented interfaces and include runnable tests and error handling. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for nonexistent apis.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a minimal reproducible task with explicit versions and automated tests; record execution rather than judging by appearance.

**Starter test input:** Implement this function for the specified runtime and test edge cases.

**Expected check:** Code compiles/runs in specified environment and passes tests. Adapt this starter case to isolate **nonexistent apis**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 72. Deprecated methods

**Definition:** Recommends outdated technical approaches.

**Why it can happen:** The model may infer APIs from naming patterns, assume dependencies, overlook edge cases or produce code without running it. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **deprecated methods**. The assistant produces a plausible response but recommends outdated technical approaches. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check current official documentation, execute tests in a controlled environment and review errors and security implications. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not invent APIs. State environment assumptions, use documented interfaces and include runnable tests and error handling. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for deprecated methods.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a minimal reproducible task with explicit versions and automated tests; record execution rather than judging by appearance.

**Starter test input:** Implement this function for the specified runtime and test edge cases.

**Expected check:** Code compiles/runs in specified environment and passes tests. Adapt this starter case to isolate **deprecated methods**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 73. Incorrect syntax

**Definition:** Produces code that cannot parse or run.

**Why it can happen:** The model may infer APIs from naming patterns, assume dependencies, overlook edge cases or produce code without running it. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **incorrect syntax**. The assistant produces a plausible response but produces code that cannot parse or run. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check current official documentation, execute tests in a controlled environment and review errors and security implications. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not invent APIs. State environment assumptions, use documented interfaces and include runnable tests and error handling. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for incorrect syntax.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a minimal reproducible task with explicit versions and automated tests; record execution rather than judging by appearance.

**Starter test input:** Implement this function for the specified runtime and test edge cases.

**Expected check:** Code compiles/runs in specified environment and passes tests. Adapt this starter case to isolate **incorrect syntax**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 74. Insecure code

**Definition:** Introduces security weaknesses.

**Why it can happen:** The model may infer APIs from naming patterns, assume dependencies, overlook edge cases or produce code without running it. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **insecure code**. The assistant produces a plausible response but introduces security weaknesses. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check current official documentation, execute tests in a controlled environment and review errors and security implications. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not invent APIs. State environment assumptions, use documented interfaces and include runnable tests and error handling. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for insecure code.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a minimal reproducible task with explicit versions and automated tests; record execution rather than judging by appearance.

**Starter test input:** Implement this function for the specified runtime and test edge cases.

**Expected check:** Code compiles/runs in specified environment and passes tests. Adapt this starter case to isolate **insecure code**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 75. Missing error handling

**Definition:** Ignores predictable failures.

**Why it can happen:** The model may infer APIs from naming patterns, assume dependencies, overlook edge cases or produce code without running it. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **missing error handling**. The assistant produces a plausible response but ignores predictable failures. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check current official documentation, execute tests in a controlled environment and review errors and security implications. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not invent APIs. State environment assumptions, use documented interfaces and include runnable tests and error handling. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for missing error handling.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a minimal reproducible task with explicit versions and automated tests; record execution rather than judging by appearance.

**Starter test input:** Implement this function for the specified runtime and test edge cases.

**Expected check:** Code compiles/runs in specified environment and passes tests. Adapt this starter case to isolate **missing error handling**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 76. Unverified dependencies

**Definition:** Assumes libraries or versions are available.

**Why it can happen:** The model may infer APIs from naming patterns, assume dependencies, overlook edge cases or produce code without running it. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **unverified dependencies**. The assistant produces a plausible response but assumes libraries or versions are available. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check current official documentation, execute tests in a controlled environment and review errors and security implications. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not invent APIs. State environment assumptions, use documented interfaces and include runnable tests and error handling. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for unverified dependencies.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a minimal reproducible task with explicit versions and automated tests; record execution rather than judging by appearance.

**Starter test input:** Implement this function for the specified runtime and test edge cases.

**Expected check:** Code compiles/runs in specified environment and passes tests. Adapt this starter case to isolate **unverified dependencies**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 77. Environment assumptions

**Definition:** Ignores operating system or runtime differences.

**Why it can happen:** The model may infer APIs from naming patterns, assume dependencies, overlook edge cases or produce code without running it. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **environment assumptions**. The assistant produces a plausible response but ignores operating system or runtime differences. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check current official documentation, execute tests in a controlled environment and review errors and security implications. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not invent APIs. State environment assumptions, use documented interfaces and include runnable tests and error handling. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for environment assumptions.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a minimal reproducible task with explicit versions and automated tests; record execution rather than judging by appearance.

**Starter test input:** Implement this function for the specified runtime and test edge cases.

**Expected check:** Code compiles/runs in specified environment and passes tests. Adapt this starter case to isolate **environment assumptions**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 78. Incorrect debugging

**Definition:** Misidentifies the cause of an error.

**Why it can happen:** The model may infer APIs from naming patterns, assume dependencies, overlook edge cases or produce code without running it. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **incorrect debugging**. The assistant produces a plausible response but misidentifies the cause of an error. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check current official documentation, execute tests in a controlled environment and review errors and security implications. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not invent APIs. State environment assumptions, use documented interfaces and include runnable tests and error handling. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for incorrect debugging.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a minimal reproducible task with explicit versions and automated tests; record execution rather than judging by appearance.

**Starter test input:** Implement this function for the specified runtime and test edge cases.

**Expected check:** Code compiles/runs in specified environment and passes tests. Adapt this starter case to isolate **incorrect debugging**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 79. Incomplete implementations

**Definition:** Omits required logic or integration steps.

**Why it can happen:** The model may infer APIs from naming patterns, assume dependencies, overlook edge cases or produce code without running it. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **incomplete implementations**. The assistant produces a plausible response but omits required logic or integration steps. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check current official documentation, execute tests in a controlled environment and review errors and security implications. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not invent APIs. State environment assumptions, use documented interfaces and include runnable tests and error handling. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for incomplete implementations.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a minimal reproducible task with explicit versions and automated tests; record execution rather than judging by appearance.

**Starter test input:** Implement this function for the specified runtime and test edge cases.

**Expected check:** Code compiles/runs in specified environment and passes tests. Adapt this starter case to isolate **incomplete implementations**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

## 80. Untested code

**Definition:** Presents plausible code as if execution were confirmed.

**Why it can happen:** The model may infer APIs from naming patterns, assume dependencies, overlook edge cases or produce code without running it. This is a possible contributing explanation, not a proven diagnosis of any single output.

**Illustrative failure:** A user requests a reliable answer involving **untested code**. The assistant produces a plausible response but presents plausible code as if execution were confirmed. The response is not automatically a verified failure until checked against the task's expected behavior.

**How to detect it:** Check current official documentation, execute tests in a controlled environment and review errors and security implications. Record the original prompt, full response, source evidence, and the precise span that fails.

**Mitigation:** Do not invent APIs. State environment assumptions, use documented interfaces and include runnable tests and error handling. Treat this as a risk-reduction instruction, not a guarantee.

**Reusable audit prompt:**

```text
Review the answer specifically for untested code.
State the claim or step at risk, the supporting evidence,
what independent check would resolve it, and a corrected
answer if the evidence is sufficient. Do not invent checks.
```

**Reproducible test design:** Provide a minimal reproducible task with explicit versions and automated tests; record execution rather than judging by appearance.

**Starter test input:** Implement this function for the specified runtime and test edge cases.

**Expected check:** Code compiles/runs in specified environment and passes tests. Adapt this starter case to isolate **untested code**; the same generic case is not proof of every failure in this chapter.

**Residual risk:** The model may repeat its original mistake during self-review. Prefer an independent source, calculation, test runner or human reviewer. Report unresolved cases as uncertain.

---

