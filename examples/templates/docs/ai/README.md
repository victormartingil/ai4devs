# Agentic Architecture Documentation

This directory contains the AI agent configuration for the project.

## Structure
- `instructions/` — Atomic rules for specific contexts (backend, frontend, testing)
- `personas/` — Agent persona definitions for specialized tasks
- `prompts/` — Reusable prompt templates for common operations

## Design Principles
- **Tool-agnostic**: All configurations work across Claude Code, Copilot, Gemini CLI
- **Composable**: Each file is atomic and can be combined with others
- **Portable**: AGENTS.md at root provides the universal base context
