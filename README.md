# Yunzhe Li

I build AI agents and the evaluations that check whether a change really made them better: hidden checks, held-out tasks, and gates enforced in code rather than in prompts.

M.S. in Computer Science at USC, graduating December 2026, and open to full-time roles starting 2027. Previously: AI Engineering Intern at Sapientia (2026) and Software Engineering Intern at Shanghai Intelligent Transportation (2024).

## Projects

### [SmartDesk](https://github.com/DaggerLee/smartdesk)

An agentic knowledge assistant (FastAPI, LangGraph, MCP). It routes each question to a direct answer, RAG, or tools, and every file write waits for human approval.

**Result:** on a 16-item fresh holdout, groundedness rose from 50.0% to 91.7%.

### Ratchet Agent · private

A self-improving agent harness: a change is adopted only after it proves better, with no regression, on my real tasks and on an evaluation the agent can neither touch nor see. Goals, risk, and merges stay human-owned.

**Result:** the gates are code, not prompts. A bubblewrap sandbox denied all 33 tested read routes to gold answers and host credentials.

[What Ratchet is for, and where it is going →](https://github.com/DaggerLee/DaggerLee/blob/main/ratchet.md)

## Contact

[yunzhe.li306@outlook.com](mailto:yunzhe.li306@outlook.com) · [LinkedIn](https://linkedin.com/in/yunzhe-li-842488273)
