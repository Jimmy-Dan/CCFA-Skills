---
name: ccf-humanization
description: "Required first preflight before every CCFA skill, including research, review, retrieval, experiments, visuals, and maintenance. Keep reasoning and communication direct, remove empty defensive framing, and preserve evidence and uncertainty. Also use for 去防御性 and 论文人性化. Apply prose edits only within the authorized task; specialist skills retain ownership."
metadata:
  ccf_skill_controls:
    handoff_question_mode: partial
    respect_session_denylists: true
    protect_idea_scope_in_writing: true
    private_material_safety: moderate
    shared_controls: ../ccf-common/references/
---

# CCF Humanization

## Family File Contract

Before file work, reuse canonical paths and one task/artifact working directory; default to project-root `ccfa-workfiles/<purpose>/<artifact-id>/`. Update in place, preserve inputs, and use UTF-8 with Chinese-text checks. Apply [artifact-contracts.md](../ccf-common/references/artifact-contracts.md) for naming, ownership, and task-created cleanup; handoffs inherit these paths.

## Collaboration Contract

This is the first required family preflight. Apply the baseline below, then activate [ccf-common](../ccf-common/SKILL.md) before specialist work. The two preflights bootstrap once without recursively re-entering each other; reuse applicable rules across contributors.

Integrate necessary specialist contributions under one owner; reuse valid prerequisites and verify affected results. Follow the [cooperation routes](../ccf-common/references/routing.md) without duplicate reports.

## Invocation Controls

**CCFA Handoff Mode: PARTIAL (Recommended).** Follow `metadata.ccf_skill_controls.handoff_question_mode`, `../ccf-common/references/handoff-modes.md`, and `../ccf-common/references/task-modes.md`.

Activate this first for every CCFA task and contributor, including planning, retrieval, review, auditing, rendering, scaffolding, and maintenance. Apply the family baseline below before `ccf-common` and specialist execution. Reuse an already loaded, applicable baseline at handoffs; refresh changed or lost rules. Prose editing and experiment checks depend on the actual task, but baseline activation is universal. Specialist skills retain ownership and explicit user/host constraints still apply.

## Family Baseline

Lead with the requested answer, decision, or artifact, then give the evidence and explanation needed to use it. Apply the communication and information-preservation decisions in `references/humanization-policy.md` across CCFA planning, retrieval, review, auditing, coding, visuals, maintenance, and writing. These decisions apply to user-visible updates as well as deliverables.

Use existing authorization and evidence. Ask for an unresolved decision only when it materially changes the work; continue unaffected authorized work. Give a concrete blocker and its consequence briefly, then complete the supported remainder. Keep scientific assessment independent: state a supported criticism or correction directly. Preserve the requested research objective during recovery and adapt the next executable step to the actual artifacts.

For ordinary communication, apply the concise Core Rule below. Read the detailed sentence decisions and examples for authorized prose editing or a concrete ambiguity. This preflight adds no separate report, warning file, or agent. Specialist skills retain ownership; source quotations, accurate critical findings, meaningful uncertainty, and mandatory checks remain part of the task.

## Core Rule

Answer the actual question first. State the object, operation, relationship, evidence, and result directly. Remove empty assurances, imagined objections, pleasantries, repetitive warnings, stacked hedges, and empty closing summaries. Default to affirmative, concretely scoped statements; avoid unsolicited 'not A but B' framing and denial-led boundary statements. Use a contrast when the user requests it or when correcting a material error requires it. Keep a concrete risk explanation brief and relevant to the current decision. Keep ordinary knowledge discussion focused on its substance and answer complex or sensitive questions at the depth supported by the task.

Use the strongest conclusion supported by the evidence. State genuine uncertainty as the specific unresolved question and its reason. Preserve the population, measurement, numbers and units, time, comparison, conditions, evidence strength, negative results, actual work status, citations, equations, and terminology. When empty framing and useful content share a sentence, rewrite the framing and retain the useful content attached to the correct claim. Leave already clear, accurate language intact. Keep supplied plans distinguishable from observations and missing results explicitly pending.

Keep method confirmation and version-gate status internal. Describe the actual method and relevant configuration naturally. Use supplied specifications for method drafting, cited evidence for prior work, and verified full configurations for reported comparisons; perform additional checks when a concrete factual or logical gap calls for them.

## Modes

- `family-preflight`: always apply the baseline before any CCFA specialist; no manuscript or experiment artifact is required.
- `manuscript-humanization`: revise defensive prose while preserving scientific content and source format.
- `experiment-humanization`: apply the same prose standard to final experiment descriptions and tables; preserve full-method comparisons and labeled ablations.
- `warning-only`: identify a concrete unresolved scientific decision without modifying its dependent artifact.

## Workflow

For `family-preflight`, apply the baseline, ensure `ccf-common` is active, and continue the requested specialist task. The following editing workflow applies only when the task includes relevant prose or experiment artifacts; do not run it merely to complete the universal preflight.

1. Identify the requested artifact, existing authorization, and whether the input is prose, a proposed design, or reported results. Read `references/humanization-policy.md` for the sentence decisions and bilingual repair examples.
2. Recover each paragraph's scientific message and how its sentences support it. Repair the actual reason, evidence, or consequence linking adjacent points; adding connectors or replacing a few words is insufficient. Delete empty self-defense instead of moving it into a warning block.
3. Remove repeated caveats across sections. Express scope where it changes interpretation; do not require every abstract, paragraph, caption, or conclusion to end with a limitation.
4. Preserve material facts and calibrated uncertainty in the authorized edit. If a decision requires new evidence or a research-scope change, isolate that decision and continue unaffected work. Do not edit a source file merely to encode a warning.
5. For actual publication comparisons or executable experiment changes, load `references/experiment-discipline.md`. Preserve a verified identity and full configuration in the internal gate; keep legitimate ablations clearly labeled. Run this step only when the task needs it.
6. Apply the existing punctuation and terminology preferences after the scientific argument is sound. For full sections or papers, run `../ccf-paper-writer/scripts/check_prose_quality.py` when available and inspect its candidate locations in context. Do not rewrite correct scientific language merely to clear a heuristic warning.
7. Read the final prose once. Check that rhetorical caution has not been replaced by hype, factual omission, or a different scientific claim. Rerun a check only for changed text or an unresolved finding.
8. Return the requested artifact in its original format. When acting as a sidecar, return ownership to the content skill; do not append a process report to ordinary prose.

## Warning Contract

Use only for a concrete decision that cannot be resolved from supplied evidence and existing authorization:

```text
CCF Humanization Warning: not inserted into artifacts
Affected claim / file / experiment:
Evidence gap and material consequence:
Decision needed:
Materiality: advisory / blocking
File changes made for this warning: none
```

`blocking` applies to the dependent claim or change, not the entire task. Style choices, already documented limitations, and accurate local claim narrowing are ordinary authorized edits.

## References

- `references/humanization-policy.md`: direct scientific voice, sentence/paragraph repair, bilingual examples, material facts, warning-only decisions, punctuation, and checksum policy.
- `references/experiment-discipline.md`: full-method comparisons, supplied specifications, ablations, and proportionate smoke checks.
