# Copilot Instructions

## Purpose

This repository contains a Proof of Concept built around an agent-based workflow.  
The goal of any LLM or coding agent working in this codebase is to:

1. Understand the current architecture before making changes.
2. Preserve the separation of responsibilities between orchestration, agents, and configuration.
3. Prefer small, safe, traceable changes.
4. Read and honor project documentation before generating or modifying code.

---

## Project Architecture

The current application structure is:

```text
/
├── .github/workflows/injector.yml  <-- PoC execution engine
├── agents/                         <-- Agent logic
│   ├── researcher.py
│   └── writer.py
├── config/
│   └── settings.json
├── requirements.txt
└── main.py                         <-- Entry point
