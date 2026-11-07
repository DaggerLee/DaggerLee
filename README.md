# Yunzhe Li

I build AI agents and the evaluations that check whether a change really made them better: hidden checks, held-out tasks, and gates enforced in code rather than in prompts.

M.S. in Computer Science at USC, graduating December 2026, and open to full-time roles starting 2027. Previously: AI Engineering Intern at Sapientia (2026) and Software Engineering Intern at Shanghai Intelligent Transportation (2024).

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
<img src="https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js">
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI">
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langgraph&logoColor=white" alt="LangGraph">
<img src="https://img.shields.io/badge/MCP-000000?style=flat-square&logo=modelcontextprotocol&logoColor=white" alt="MCP">
<img src="https://img.shields.io/badge/Claude%20Code-D97757?style=flat-square&logo=claude&logoColor=white" alt="Claude Code">
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
<img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux">

## 🛠️ Projects

### [SmartDesk](https://github.com/DaggerLee/smartdesk)

An agentic knowledge assistant (FastAPI, LangGraph, MCP). It routes each question to a direct answer, RAG, or tools, and every file write waits for human approval.

**Result:** the shipped router scored 18/18 on a preregistered holdout written after it was frozen.

### Ratchet · private

A system in which an AI agent improves the workflow it runs in, my multi-model coding setup with cross-model review. A change is adopted only after it proves itself on my real work, and adoption is my call alone.

**Results so far:** in 10 rounds, the system proposed 3 changes that passed verification, and I adopted all three: one cut tokens 34% and time 29% on one small task, one cut tokens 20% on small tasks drawn from two real coding tasks, and one fixed a small task that had been failing. None regressed under the rule. Exploratory: few tasks.

[What Ratchet is for, and where it is going →](https://github.com/DaggerLee/DaggerLee/blob/main/ratchet.md)

## 📫 Contact

[![Email](https://img.shields.io/badge/Email-yunzhe.li306%40outlook.com-0078D4?style=flat-square)](mailto:yunzhe.li306@outlook.com) [![LinkedIn](https://img.shields.io/badge/LinkedIn-Yunzhe%20Li-0A66C2?style=flat-square)](https://linkedin.com/in/yunzhe-li-842488273)
