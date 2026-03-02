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
* Test plan, test cases, code, Selenium framework, Playwright, and anything in the terminal with the IDE.

  

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


**Installation**
open cmd: npm i -g opencode-ai@latest
opencode --version
scoope install opencode

change model: /model  

ollama api keys: ollama.com/settings  

opencode --version
opencode models

create AGENTS.md: /init

<img width="431" height="225" alt="image" src="https://github.com/user-attachments/assets/04e3676e-d892-4ebf-9c2d-0f26f1588713" />

in chatgpt: I want you to basically give me an enhanced prompt for OpenCode to create a test case generator where the user will submit an idea or a user story and the application will generate a test case from it. And this should be a very minimal application that uses the GroQ API. In this case, the user will enter the GROQ API key and will be able to generate test cases using the free model, which is Llama 3.0.

then paste chatgpt output in opencode

<img width="186" height="251" alt="image" src="https://github.com/user-attachments/assets/290764c9-8c89-429f-9539-1557b60a3f64" />

<img width="1470" height="840" alt="image" src="https://github.com/user-attachments/assets/e0ad613e-95bc-40e3-b3f4-19d09dcb7541" />

you can change model: https://console.groq.com/playground

search model and change:  
<img width="666" height="143" alt="image" src="https://github.com/user-attachments/assets/5aa31027-bcf1-40ee-a25f-39a81d37068d" />

<img width="1342" height="586" alt="image" src="https://github.com/user-attachments/assets/066d3586-6996-488d-a80c-8fbf61c32c37" />

next prompt: Please make sure that test cases are in a proper Jira format and you give them in a tabular form. Please change the UI.
