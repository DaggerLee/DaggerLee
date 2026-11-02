# Ratchet

*A system in which an AI agent improves the workflow it runs in. Its repository is private; this page says what it is for and what it has shown so far. Updated November 2026.*

Everyone is talking about recursive self-improvement. Then what? Ratchet is built to answer three questions about an agent that improves itself:

1. **Did it really get better?** Does the next round repeat the last round's mistake, and does a lesson it learned hold on tasks it has not seen?
2. **Did it learn anything bad?** When one score rises, did anything else break?
3. **How long will it keep working?** When a stronger model or a new tool arrives, is an adopted change still worth keeping?

## The rule

A change is adopted only after it proves itself on my real work. The evaluation is hidden from the agent and runs in isolated environments, a change that regresses anything is rejected, and adoption is my call alone. Ratchet changes the workflow around the model, never the model's weights.

## Results so far

In October 2026 the loop ran 9 rounds on two of my real coding tasks. Two changes the system proposed on its own passed verification, and I adopted both. The first used 34% fewer tokens and 29% less time on the task it targeted, with every check still passing. The second used 20% fewer tokens across both tasks, with no regression under the rule.

Both are savings on the tasks the loop worked on. Whether they carry over to new work is the next test: a third real task is joining the loop.

## Where it is going

Ratchet is a first step toward AIOS, a personal AI operating system that keeps improving on its owner's real work.

## Where it stands

- 375 automated tests.
- The workflow it improves is my own multi-model coding setup, with cross-model review.
