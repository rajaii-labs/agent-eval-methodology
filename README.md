# Recall, Negation, Abstention

![Cover of Recall, Negation, Abstention, Article I of the Substrate series](./Substrate_Recall_Negation_Abstention_Cover.png)

**A false answer from an agent with months of memory, traced to two defects in its data, and the rule that followed: look it up, or say it cannot.**

Rajaii Labs · Substrate Series · Article I · November 2026

This paper traces one false sentence from a production AI agent to its causes: the agent said a business engagement was still pending days after it had been declined, because two defects in its data, a stale stored fact and a size limit in its memory pipeline that silently cut the stretch of the day's conversation where the engagement was declined, had kept the change out of both its memories. Substrate is a production AI agent built on Claude that I have run for one user, me, since April 2026; its memory, its record of facts and its standing instructions live outside the model, so the model can be replaced and the agent stays. From failures like this one came a method small enough to copy: seven kinds of failure that all look alike to the user; after every material change, three kinds of question asked cold, in a fresh session (recall of a stored fact, negation of what its records mark false, abstention where nothing is stored); and a read-only tool over the agent's own records, so that for anything it can check it looks the answer up or says it cannot. It is one agent with one user, described as of July 2026, with what the later papers found through November 2026.

**[Read the PDF, second edition](./Substrate_Eval_Methodology.pdf)** · **[Read the full text (Markdown)](./Substrate_Recall_Negation_Abstention.md)** · **[The first edition](./archive/first-edition/README.md)**

**Second edition, November 2026.** The findings are the first edition's (July 2026), told as a story, with the seven corrections later articles printed applied in place. The first edition is kept as it stood before this edition, its PDF exactly as first published, at the tag [`first-edition`](https://github.com/rajaii-labs/agent-eval-methodology/tree/first-edition) and in [`archive/first-edition/`](./archive/first-edition/README.md); references to its sections still land.

**The Substrate series:** Article I, this paper · [Article II](https://github.com/rajaii-labs/agent-cost-forensics) · [Article III](https://github.com/rajaii-labs/substrate-preconditions) · [Article IV](https://github.com/rajaii-labs/substrate-choices) · [Article V](https://github.com/rajaii-labs/substrate-recursion)\
**How to cite:** Rajaii, R. (2026). *Recall, Negation, Abstention: A false answer from an agent with months of memory, traced to two defects in its data, and the rule that followed: look it up, or say it cannot* (2nd ed.). Rajaii Labs, Substrate series, Article I. [BibTeX](#citation) · [CITATION.cff](./CITATION.cff)

---

## What is in the paper

**The story**, sections 1–7, about 5,100 words:

- **The opening.** The false sentence of May 2026, the main point in one minute, the thesis, and one observation per finding that would prove it wrong.
- **1. Agents with long memories fail in ways a single question to a model with no past cannot reach.** Why this matters now: assistants that remember, tests that ask single questions, and the first memory benchmarks.
- **2. Substrate keeps its memory outside the model, and the checks the later papers rely on begin here.** What Substrate is, the setting as of July 2026, and the series, a line each.
- **3. Behind one confident false sentence were two defects in the data, and both of the agent's memories agreed on the wrong answer.** The investigation (Figure 1), the model's own part, the fixes, and the paper's main lesson.
- **4. Seven kinds of failure all reach the user as "the agent is wrong", and most failures showed only when the agent was asked cold.** The seven classes (Figure 2), the three probes and a worked example on abstention; then the voice, measured.
- **5. For anything it can check, the agent stopped answering from memory: it looks the answer up, or it says it cannot.** The six layers in the order built (Figure 3), and what lookup gave for free.
- **6. The method is small enough to copy, and its evidence is one system with one user.** What it means for builders, the limits, autonomy in shadow, and the three open problems.
- **7. No claim is refuted: two of fifteen held, four remain open, and nine are limited, reported from practice without the evidence printed.** Every claim graded, and what the later papers found.
- **The ending.** The record in counts, and my interpretation of it.

**Technical sections**, T1–T11: the system as of July 2026; the seven failure classes; the six layers, with the schema and the synthetic example row; the probes and their grading; the measured voice; the incident and its fixes; shadow mode and its four conditions; the three open problems and what later papers did with them; the lessons; the glossary; and what changed in this edition, with the corrections, the open errata and a map from every first-edition section.

**Beside the paper.** The [first edition](./archive/first-edition/README.md), its [PDF](./archive/first-edition/Substrate_Eval_Methodology.pdf) and its cover, archived as they stood before this edition; the figures' sources in [`figures/`](./figures/).

## The Substrate series

1. **Recall, Negation, Abstention** — Rajaii Labs, July 2026 · second edition, November 2026. *This paper.*
2. **Do Not Trust My Labels** — Rajaii Labs, July 2026 · second edition, November 2026. [Repository](https://github.com/rajaii-labs/agent-cost-forensics)
3. **Preconditions** — Rajaii Labs, August 2026 · second edition, November 2026. [Repository](https://github.com/rajaii-labs/substrate-preconditions)
4. **Choices** — Rajaii Labs, October 2026 · second edition, November 2026. [Repository](https://github.com/rajaii-labs/substrate-choices)
5. **Recursion** — Rajaii Labs, November 2026. [Repository](https://github.com/rajaii-labs/substrate-recursion)

## Citation

```bibtex
@techreport{rajaii2026recall,
  author      = {Rajaii, Ramin},
  title       = {Recall, Negation, Abstention: A false answer from an agent with months of memory, traced to two defects in its data, and the rule that followed: look it up, or say it cannot},
  institution = {Rajaii Labs},
  year        = {2026},
  month       = nov,
  edition     = {Second},
  note        = {Substrate series, Article I. Second edition, November 2026; first published July 2026.}
}
```

The same metadata is in [`CITATION.cff`](./CITATION.cff), which GitHub's "Cite this repository" reads.

## Contact

Substrate is a production system of Rajaii Labs, built on Claude. Architecture and methodology questions welcome: **ramin@raminrajaii.com** · [linkedin.com/in/raminrajaii1](https://www.linkedin.com/in/raminrajaii1) · ORCID [0009-0009-5517-6701](https://orcid.org/0009-0009-5517-6701)

© 2026 Ramin Rajaii. All rights reserved. Terms of use: [LICENSE.md](./LICENSE.md).
