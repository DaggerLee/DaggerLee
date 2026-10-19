# Ratchet Agent

*A self-improving agent harness. Its repository is private; this page explains what it is for and where it is going. Updated October 2026.*

Everyone is talking about recursive self-improvement. Then what? Ratchet is built to answer three questions about an agent that improves itself:

1. **Did it really get smarter?** Does the next round repeat the last round's mistake, and does a lesson it learned hold on tasks it has not seen?
2. **Did it learn anything bad?** When one score rises, did anything else break?
3. **How long will it keep working?** When a stronger model or a new tool arrives, is an adopted change still worth keeping?

## The rule

A change to the harness is adopted only after it proves better, with no regression, on my real tasks and on an evaluation the agent can neither touch nor see. Ratchet changes the harness around the model (its rules, skills, and prompts), never the model's weights. When a new model or tool arrives, adopted changes are checked again, and one that no longer helps is proposed for retirement.

## One turn of the ratchet

1. A real task of mine runs through a versioned multi-agent workflow.
2. Its concrete failures become small tasks with hidden checks, scored by a checker that never loads the submitted code. The small tasks are grouped by cause and split into held-in and held-out sets.
3. Working only from the held-in tasks, an agent in a sandbox proposes a change to one part of the harness and predicts what it will fix.
4. The change and the current harness each run every small task three times. The change qualifies only if it fixes what it predicted, makes no small task worse, and adds at most 10% time and tokens.

Every check is decided by a machine, under a rule I set once; adoption and merges stay with me.

## Where it is going

Ratchet is a first step toward AIOS, a personal AI operating system that keeps improving on its owner's real work. Across all three questions, the unit of account is what one verified improvement costs in money, data, people, and time.

## Where it stands

- Built so far: 80+ reviewed PRs and 338 tests; the core was rebuilt in October 2026 (15 PRs, 163 tests).
- The gates are code, not prompts: a bubblewrap sandbox denied all 33 tested read routes to gold answers and host credentials.
- Not yet shown: a full turn of the loop on my real tasks. With few tasks, the first results will be exploratory; this page will report them.
