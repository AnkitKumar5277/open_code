**Automating QA Workflow Using OpenCode**
* What is OpenCode?
* Installation & Setup
* OpenCode vs Other Tools
* Commands

**What is OpenCode?**
OpenCode is an **open-source AI coding agent** designed for use in the terminal. Unlike proprietary tools, OpenCode supports **75+ AI models** from major providers such as OpenAI, Anthropic Claude, Google Gemini, AWS Bedrock, Groq, Azure OpenAI, OpenRouter, and local models via Ollama and LM Studio.
**Key Features:**
* **Open Source (MIT License)**
  Fully transparent with no vendor lock-in.
* **Terminal-based Interface (TUI)**
  Built using Bubble Tea for a responsive terminal experience.
* **Multi-Provider Support**
  You can use different AI models for different tasks (e.g., Claude for planning, Gemini for generation, local models for private code).
* **Popular Tool**
  Over **95K+ GitHub stars**, making it one of the most popular open-source AI coding tools.

**Why OpenCode for QA Engineers?**
**Model Flexibility**
* Claude → Sonnet 4.6, Opus 4.6, older versions
* GPT → 5.1, 5.2, 5.3
* Open-source models → Kimi-K2.5, Minimax 2.5, Qwen Coder
**Privacy First**
* Local models → GPT-OSS 20B
* Built-in agents

| Feature             | OpenCode                       | Claude Code                      |
| ------------------- | ------------------------------ | -------------------------------- |
| **LLM Providers**   | 75+ models, any provider       | Anthropic Claude only            |
| **License**         | MIT (open source)              | Proprietary                      |
| **Undo/Redo**       | Git-based `/undo` `/redo`      | Double-Escape rewind             |
| **Agent System**    | Build, Plan, Research + custom | Plan mode toggle                 |
| **Project Context** | `AGENTS.md`                    | `CLAUDE.md`                      |
| **Custom Commands** | Markdown files in `commands/`  | `.claude/commands/`              |
| **Permissions**     | Granular per-tool, per-command | `--dangerously-skip-permissions` |
| **Session Sharing** | `/share` generates public URL  | Not built-in                     |
| **IDE Integration** | VS Code, Cursor, any terminal  | Terminal only                    |
| **Cost**            | Free (bring your own API key)  | Claude subscription required     |
