# AI Coding Agents -- AI4Devs

A bilingual (ES/EN) presentation on AI Coding Agents, created by **Victor Martin** for [AI4Devs](https://ai4devs.com). The entire deck is a single self-contained `index.html` file with 11 sections covering LLMs, agents, prompting, context management, MCP, multi-agent orchestration, workflows, and more.

**Live:** [victormartingil.github.io/ai4devs](https://victormartingil.github.io/ai4devs/)

---

## Quick Start

1. Open `index.html` in any modern browser — or visit the [live version](https://victormartingil.github.io/ai4devs/).
2. Use the sidebar to navigate between sections.
3. Click the **Present Mode** button to enter a distraction-free fullscreen view suitable for live delivery.

No build step, no dependencies, no server required.

---

## Presentation Sections

| Section | Title | Duration |
|---------|-------|----------|
| s0 | Cover | -- |
| s1 | LLM vs Agent vs Tool | 5 min |
| s2 | Prompting | 8 min |
| s3 | Context Files | 10 min |
| s4 | Agent File Map | 7 min |
| s5 | MCP | 7 min |
| s6 | Multi-Agent and Orchestration | 15 min |
| s7 | Workflow | 8 min |
| s8 | Comparison | 5 min |
| s9 | Anti-patterns | 5 min |
| s10 | Q&A | 15 min |

**Total estimated time: ~85 min**

---

## Examples

The `examples/` directory contains supplementary material referenced throughout the presentation.

### `examples/templates/`

Generic, reusable templates for agentic configuration. These can be adapted to any project regardless of language or framework:

- `CLAUDE.md` / `AGENTS.md` -- agent instructions templates
- `.claude/settings.json` -- researched allowlist for secure vibe coding
- Sub-agents, skills, personas, and prompt templates

### `examples/applied/`

A concrete applied example demonstrating the templates in practice with the following stack:

- Java 21
- Spring Boot 3
- Hexagonal Architecture

---

## References

- [Claude Code Documentation](https://code.claude.com/docs/en/overview)
- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [Gemini CLI Documentation](https://geminicli.com/docs)
- [OpenAI Codex CLI](https://github.com/openai/codex)
- [Model Context Protocol (MCP)](https://modelcontextprotocol.io)
- [Cursor](https://cursor.com)
- [Faros AI](https://faros.ai)
- [DORA (DevOps Research and Assessment)](https://dora.dev)
- [Claude Agent SDK (Python)](https://github.com/anthropics/claude-agent-sdk-python)
- [Claude Agent SDK (TypeScript)](https://github.com/anthropics/claude-agent-sdk-typescript)

---

## License

This material is provided for educational purposes as part of the AI4Devs programme.
