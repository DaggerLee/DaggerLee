# Ratchet

*A system in which an AI agent improves the workflow it runs in. Its repository is private; this page says what it is for and what it has shown so far. Updated October 2026.*

Everyone is talking about recursive self-improvement. Then what? Ratchet is built to answer three questions about an agent that improves itself:

1. **Did it really get better?** Does the next round repeat the last round's mistake, and does a lesson it learned hold on tasks it has not seen?
2. **Did it learn anything bad?** When one score rises, did anything else break?
3. **How long will it keep working?** When a stronger model or a new tool arrives, is an adopted change still worth keeping?

## The rule

A change is adopted only after it proves itself on my real work. The evaluation is hidden from the agent and runs in isolated environments, a change that regresses anything is rejected, and adoption is my call alone. Ratchet changes the workflow around the model, never the model's weights.

## First result

In October 2026 the first change the system proposed on its own passed verification, and I adopted it. With every check still passing, the workflow used 34% fewer tokens and 29% less time.

This is exploratory: it was measured on one task, so it shows a cheaper run on that task, not yet a general gain.

## Where it is going

Ratchet is a first step toward AIOS, a personal AI operating system that keeps improving on its owner's real work.

## Where it stands

- 375 automated tests.
- The workflow it improves is my own multi-model coding setup, with cross-model review.
