# Section Writing Patterns

Use this reference when drafting or revising paper sections, captions, contribution bullets, or experiment analysis.

## Argument Chain

Every section should fit this chain:

```text
problem or context -> gap -> challenge -> design choice -> evidence -> mechanism -> boundary
```

Every paragraph should answer:

- What issue does this paragraph solve?
- How does it connect to the previous and next paragraph?
- Which contribution, figure, table, formula, or claim does it support?
- What should the reader believe after reading it?

## Abstract

Recommended structure:

```text
application problem -> concrete limitation of existing work -> one-sentence method -> key mechanisms -> main evidence -> bounded significance
```

Rules:

- Start with the concrete research problem, not a generic trend.
- Define core abbreviations on first use.
- Include only results that can be supported by the manuscript.
- Avoid reviewer-response context.
- Do not overload the abstract with table-like numbers.

## Introduction

Recommended structure:

```text
real scenario and importance -> existing routes and limits -> unresolved tension -> research challenge -> paper idea -> contributions
```

Rules:

- Group prior routes logically rather than listing papers.
- Explain what each route solves and what it leaves open.
- Make challenges match later method modules and experiments.
- Make contributions specific, checkable, and non-overlapping.

## Contributions

Write each contribution as:

```text
We propose/introduce/design ... to address ...; it is supported by ...
```

Each contribution should map to at least one method component, formula, figure, table, experiment, or deployment result.

Avoid unsupported priority claims such as `first`, `novel`, or `state-of-the-art`.

## Related Work

Use grouped mini-arguments:

```text
Direction A: representative work -> solved issue -> remaining limitation.
Direction B: representative work -> solved issue -> remaining limitation.
Relation to this work: specific distinction.
```

Be fair and specific. Do not turn related work into a second introduction or a list of summaries.

## Method

For each module, write:

```text
motivation -> input/output -> core operation or formula -> interface to neighboring modules -> design rationale -> limitations if needed
```

Rules:

- Do not write as code commentary.
- Define symbols before or immediately after formulas.
- Explain what a formula does in the algorithm.
- Keep experimental results out of the method unless needed to motivate a design constraint.

## Experiment Analysis

Use:

```text
purpose -> setting/metric -> observed result -> mechanism explanation -> contribution relation -> boundary
```

Rules:

- A table or figure must be used as evidence for a clear question.
- Move from numbers to mechanism; do not merely restate rankings.
- State local reversals, negative results, or trade-offs when they exist.
- Explain hardware, trials, seeds, data split, or protocol when relevant.

## Captions

Good captions explain:

- comparison objects;
- metrics and units;
- conditions or protocol;
- subfigure meaning;
- the main phenomenon readers should notice.

Captions should be self-contained but not a substitute for main-text analysis.

## Conclusion

Use:

```text
what was addressed -> what was designed -> what evidence supports it -> where it applies -> remaining boundary
```

Do not expand a limited experimental scope into a general claim.
