---
name: "make-no-mistakes"
description: "Make no mistakes / pre-merge QA: select risk-based checks, conditional Kun Chen pipeline, and independent Crosscheck with live UI evidence."
---

# Make No Mistakes

Use when the user says “make no mistakes”, invokes `$make-no-mistakes`, or requests risk-proportionate verification before completed-issue closure or PR merge. This is the 2x umbrella workflow, not Kun Chen's `no-mistakes` skill or CLI. Crosscheck remains the independent verification engine.

## 1. Bind the work

Read the original request, repository instructions, acceptance criteria, current diff and applicable execution policy. Record the exact target and permitted actions. Inspect an existing run or canonical worker before starting another; keep its custody and identity. This workflow adds verification, not commit, push, merge, deployment, installation or publication authority.

## 2. Select proportionate checks

Choose by risk AND complexity before execution. Record the selected checks and the reason for running or skipping the heavier pipeline.

- Tiny reversible copy, typo, documentation or metadata edits: inspect the final artifact and diff; run focused format/link/schema checks where relevant. Skip the heavy pipeline and independent process QA unless a concrete risk or source contract requires them.
- Non-trivial code, risky refactors, auth/security, routing, data flow, CI/build or behavior changes: run focused repository tests/build/lint, then Kun Chen's `no-mistakes` pipeline when the repository is eligible and its setup and actions are authorized; obtain fresh independent Crosscheck QA on the final immutable target.
- UI or interaction changes: require live browser journeys and visual evidence in the independent QA, even when the code diff is small.
- Documents, data, decisions and operational changes: use the applicable Crosscheck profiles when consequences or source criteria warrant independent verification; do not run a code pipeline on non-code artifacts.

An initialized and authorized pipeline is not an excuse to skip required behavior proof. In governed execution, honor project allowlisting and task-level delivery-gate selection. If the pipeline is warranted but unavailable or ineligible, record the exact reason and perform the authorized repository checks/review plus independent QA; if the source contract requires the pipeline itself, return BLOCKED instead. Do not silently install or initialize tools.

## 3. Complete the builder checks

Implement the requested work and verify the final diff against the acceptance criteria. Read and follow the installed `no-mistakes` skill before invoking its CLI; retain its gates, branch custody, synchronization and finding-disposition rules. Keep Kun Chen's attribution and upstream skill unchanged.

While that pipeline owns the mutable branch, no other worker edits or independently verifies it. Record the outcome, PR and final head. A successful pipeline is builder proof, not independent QA or merge authority. For paths that skip the pipeline, use the repository's required review process; record any unavailable check explicitly.

## 4. Independently verify when selected

Read and follow the installed `crosscheck` skill and its task-profile, evidence, publication and runtime references. Dispatch a fresh ephemeral read-only verifier that did not build or materially change the target, with task-local intent and criteria rather than trusted builder conclusions. Preserve its exact-target binding and PASS/FAIL/BLOCKED rules. Missing independence, capability, evidence or freshness is BLOCKED, never PASS.

For UI work, actually exercise the affected user journey, inspect desktop/mobile states and capture current named-viewport screenshots for visual claims. For multi-step flows, retain ordered trace/video evidence; pair server-side effects with persisted-state proof. Use the applicable browser skill and authorized test environment. Synthetic fixtures, static source checks and old producer screenshots do not establish live E2E success.

Return failures to the same builder, then reverify the changed target. Crosscheck never repairs the product. A later push, rebase, deployment or material configuration change invalidates prior QA.

## 5. Close the loop

Re-read the final target and inspect the actual report, evidence and any required receipt. Confirm every required criterion and review finding has an evidence-backed disposition. Publish only authorized safe summaries to the issue/PR/original worker, verifying delivery separately from the verdict.

Before an authorized merge or completed-issue closure, require the selected checks and any mandatory exact-head independent PASS. A lightweight path needs direct artifact proof, not a fabricated Crosscheck receipt. Report what was checked, why the heavier pipeline ran or was skipped, what remains unverified, and whether the user needs to act. Never claim universal automatic enforcement merely because this skill is installed.
