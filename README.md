# Paper Writing Assistant Skill

`paper-writing-assistant` is a Codex skill for rule-based research-paper writing and revision. It helps turn user intent, manuscript text, review reports, reviewer comments, venue requirements, and verified facts into restrained academic writing.

## What It Does

- Drafts and revises abstracts, introductions, contributions, related work, methods, experiment analysis, captions, conclusions, and revision notes
- Converts review-report findings into concrete manuscript edits
- Drafts reviewer responses and matching manuscript revision instructions
- Calibrates claim strength against available evidence
- Removes generic AI-like wording while preserving technical meaning
- Checks synchronization across manuscript, response letter, supplement, captions, and final submission

## Install

Copy the skill folder into your Codex skills directory:

```bash
mkdir -p ~/.codex/skills
cp -R paper-writing-assistant ~/.codex/skills/
```

Then ask Codex to use `$paper-writing-assistant` for writing or revision.

## Example Prompts

```text
Use $paper-writing-assistant to rewrite this experiment analysis using the verified table values.
Use $paper-writing-assistant to draft a reviewer response and matching manuscript revision for these comments.
Use $paper-writing-assistant to convert this review report into prioritized paper edits.
Use $paper-writing-assistant to compress this introduction for the target venue without weakening the logic.
```

## Notes

This skill does not replace your full local writing rules. When a user provides or references a writing-rule document, Codex should read that file first and use the bundled references only as writing checklists.

The skill should not invent experiments, numbers, citations, baseline results, reviewer-requested changes, or statistical conclusions. Data-bearing writing should remain bounded by verified evidence.

## License

MIT
