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


```

---

## Subagents

Subagents are specialized AI assistants that can be invoked to handle specific types of tasks. 

When users call a simulated subagent, it will look for the corresponding markdown file, `.github/subagents/{subagent}.md`, and execute its contents as the block of operations.

For example, if the user instructs `Call planner subagent to plan the refactoring`, you have to look for the markdown file, `.github/subagents/planner.md`, and execute its contents as the block of operations.

# AI Agent Reference Guide

**Purpose:** This document serves as the primary entry point for AI agents. It provides a comprehensive overview of the project structure, development guidelines, and links to specialized documentation for different aspects of the system.

