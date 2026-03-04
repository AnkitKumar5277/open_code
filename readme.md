**OpenCode?** opencode.ai/download  
OpenCode is an **open-source AI coding agent** designed for use in the terminal. Unlike proprietary tools, OpenCode supports **75+ AI models** from major providers such as OpenAI, Anthropic Claude, Google Gemini, AWS Bedrock, Groq, Azure OpenAI, OpenRouter, and local models via Ollama and LM Studio.

**Key Features:**
- Open Source
- Terminal-based Interface
- Any Model, Any Provider - use different AI models for different tasks
- MCP Support — Plug in Playwright, Selenium, Appium MCP servers for browser/mobile automation
- Privacy-First — Your code stays on your machine. OpenCode does not store any code or context data
- IDE + Desktop + Web — Available as CLI, VS Code extension, desktop app, and web interface
- FREE  
- Custom Agents  
- Built-inGitHub Actions Agent  

**Test plan, test cases, code, Selenium framework, Playwright, and anything in the terminal with the IDE.**

**Installation**
- open cmd: npm i -g opencode-ai@latest  
- opencode --version  
- scoope install opencode  
- opencode upgrade  
- opencode
- /connect

# COMMANDS
- change model: /model  
- ollama api keys: ollama.com/settings  
- opencode --version
- opencode models
- List all available models from CLI - opencode models
- /theme  

# List all authenticated providers
- opencode auth list
- opencode auth ls          # short version

# What is MCP?
MCP (Model Context Protocol) lets you add external tools to OpenCode. For QA, this means browser automation, code search, accessibility testing, and more — all controllable by the AI agent.

// opencode.json
{
  "$schema": "https://opencode.ai/config.json",
  "mcp": {
    "playwright": {
      "type": "local",
      "command": ["npx", "-y", "@anthropic-ai/mcp-server-playwright"],
      "enabled": true
    }
  }
}

# MCP Management Commands
- opencode mcp add              # Interactive MCP server setup
- opencode mcp list             # List configured MCP servers


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
 
https://github.com/microsoft/playwright-mcp?tab=readme-ov-file

open the app.vwo.com with the playwright mcp and enter the dummy username and password and click on the submit button and verify the error message
