# Ratchet

*A system in which an AI agent improves the workflow it runs in. Its repository is private; this page says what it is for and what it has shown so far. Updated November 2026.*

Everyone is talking about recursive self-improvement. Then what? Ratchet is built to answer three questions about an agent that improves itself:

1. **Did it really get better?** Does the next round repeat the last round's mistake, and does a lesson it learned hold on tasks it has not seen?
2. **Did it learn anything bad?** When one score rises, did anything else break?
3. **How long will it keep working?** When a stronger model or a new tool arrives, is an adopted change still worth keeping?

## The rule

A change is adopted only after it proves itself on my real work. The evaluation is hidden from the agent and runs in isolated environments, a change that regresses anything is rejected, and adoption is my call alone. Ratchet changes the workflow around the model, never the model's weights.

## Results so far

By early November 2026 the loop had run 10 rounds on three of my real coding tasks, two in TypeScript and one in Python, with 10 small tasks drawn from them. Three changes the system proposed on its own passed verification, and I adopted all three. The first used 34% fewer tokens and 29% less time on the one small task it targeted, with every check still passing. The second used 20% fewer tokens across 7 small tasks from two of the tasks, with no regression under the rule. The third fixed a small task from the third real task that had been failing.

The first two are savings; the third is the first fix of a failure. Small tasks held out from the loop show whether a change broke anything elsewhere: on the second task, the three held out passed under both versions. They cannot show that a lesson carries over to new work, which is still open: on the third task, the one held out failed under both versions, so it shows neither a regression nor a transfer. All of this is exploratory, on few tasks so far.

Not every finding was about the agent. For three rounds my own evaluator failed both versions on every trial of one task, because its scope check counted files the tests leave behind, which the project's .gitignore ignores. I fixed the check.

## Where it is going

Ratchet is a first step toward AIOS, a personal AI operating system that keeps improving on its owner's real work.

## Where it stands

- Each eval trial is a full agent run: 10+ minutes and 1M+ tokens.
- The workflow it improves is my own multi-agent coding setup: Claude Code and Codex agents with cross-model review.
