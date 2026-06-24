---
name: paper-writing-assistant
description: "Assist with research-paper writing and revision under local writing rules. Use when Codex is asked to draft, rewrite, polish, compress, expand, restructure, respond to reviewer comments, revise from an audit report, align with journal/conference requirements, write captions, improve experiment analysis, reduce overclaims, remove AI-like wording, or synchronize a manuscript, response letter, supplement, and final submission."
---

# Paper Writing Assistant

Use this skill for writing-side work on research papers. Its job is to turn intent, rules, review reports, reviewer comments, venue requirements, and manuscript material into precise paper text. Use `paper-pdf-review` instead when the primary task is PDF reading or issue discovery.

## Required Workflow

1. Identify the writing task: draft new text, revise existing text, respond to reviewers, convert a review report into edits, compress for length, adjust to venue style, or perform final synchronization.
2. Locate and read the applicable writing rules. Prefer the user-specified rule file; otherwise search the workspace for local paper/thesis writing-rule documents. Treat the full external rules file as authoritative. Use this skill's references only as routing checklists.
3. Gather constraints before writing:
   - target section, venue, word/page limit, language, style, and revision marking requirements;
   - source manuscript text, LaTeX, tables, figures, captions, review report, reviewer comments, response draft, or experiment logs;
   - facts and numbers that may be used.
4. Separate confirmed facts from missing facts. Do not invent experiments, numbers, citations, statistical claims, or baseline results.
5. Plan the local role of the text before drafting: what problem it solves, how it connects to neighboring paragraphs, and which contribution, figure, table, formula, or reviewer concern it supports.
6. Draft or revise with evidence boundaries. Use specific mechanisms, data, and figure/table references where available; downgrade claims when evidence is partial.
7. Run the relevant reference checklist before final output:
   - `references/section_writing_patterns.md` for paper sections, captions, and experiment analysis.
   - `references/reviewer_response_workflow.md` for responses and revision synchronization.
   - `references/final_self_check.md` for final submission or high-risk data-bearing edits.
8. Return the revised text plus a short change rationale and verification notes when the task involves facts, data, references, or reviewer promises.

## Writing Modes

- **Generate**: Create a section, paragraph, caption, contribution list, response, or revision note from provided facts.
- **Rewrite**: Improve logic, specificity, concision, tone, or flow while preserving factual content.
- **Surgical edit**: Modify only the requested span unless a neighboring sentence must change for coherence.
- **Audit-to-edit**: Convert findings from a review report into concrete manuscript edits and response-letter text.
- **Reviewer response**: Produce a professional response and matching manuscript revision plan.
- **Synchronization**: Check that manuscript, captions, tables, response letter, supplement, and final claims say the same thing.

## Non-Negotiable Boundaries

- Do not fabricate numeric results, citations, baselines, datasets, hardware, trial counts, statistical tests, or reviewer-requested experiments.
- Do not hide negative results, local reversals, limitations, protocol mismatches, or uncertainty to make the story smoother.
- Do not turn unchecked data into verified conclusions.
- Do not insert reviewer-response wording into the manuscript body, such as `following the reviewer's suggestion`.
- Do not write hard-coded figure/table/equation numbers in LaTeX source. Use maintainable cross-references when labels are known.
- Do not silently change terminology, symbols, dataset names, method names, metric direction, or units.

## Claim Calibration

Use strong language only when the evidence supports it.

- Use `shows`, `achieves`, or `outperforms` only with clear comparison scope and numbers.
- Use `suggests`, `indicates`, `is consistent with`, or `a possible reason is` for mechanism explanations without proof.
- Avoid unsupported `prove`, `fully solve`, `completely eliminate`, `superior`, `remarkably`, `comprehensive`, and `significantly`.
- Replace vague praise with a concrete mechanism, setting, metric, or limitation.

## Expected Output

For short writing tasks, output the revised text directly and then a compact note:

```text
Notes:
- What changed:
- Facts/numbers used:
- Items needing user verification:
```

For substantial edits, use:

```text
Revised text:

Change rationale:

Data and claim check:
- Inline numbers verified: yes/no/not applicable
- Figure/table references verified: yes/no/not applicable
- Derived values recalculated: yes/no/not applicable
- Baseline protocol consistency: yes/no/unknown/not applicable
- Claims downgraded or bounded:
- Needs user verification:
```

For reviewer responses, include both response text and manuscript edit instructions. See `references/reviewer_response_workflow.md`.

## Style

Write in a restrained academic style. Prefer short, precise sentences. Keep each paragraph centered on one claim. Remove empty bridge sentences and generic AI-like evaluation. Preserve the user's technical meaning even when polishing language.
