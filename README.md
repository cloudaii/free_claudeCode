# free_claudeCode

# Claude Code Unlimited (free)

Tired of hitting usage caps on the official Claude Code CLI or watching your local machine crawl while trying to run heavy models? You don't need a $5,000 rig or a pricey monthly subscription to get elite-level AI coding assistance.
By leveraging NVIDIA NIM and a simple proxy server, you can bypass local hardware limitations and expensive API costs. Here is your step-by-step guide to setting up a "Free Unlimited" Claude Code environment.

**Prerequisites & Environment Setup**

Before we start, we need UV, the ultra-fast Python package installer, to manage our proxy server.




# nvidia nim api key 
https://build.nvidia.com/

# openRouter API key
https://openrouter.ai/workspaces/default/keys?hl=en-US

# deepSeek API key
https://platform.deepseek.com/sign_in


# run this in power shell 

```
wsl --install
```

# Run this command install uv
**official website**
https://docs.astral.sh/uv/getting-started/installation/
```
curl -LsSf https://astral.sh/uv/install.sh | sh
```

# install python 

```
uv python install 3.14
```
# create folder 

```
mkdir local
```
# navigate 

```
cd local
```


# clone git repo

```
git clone https://github.com/Alishahryar1/free-claude-code.git nvidia-nim
```

# navigate 
```
cd nvidia-nim
```
# run this 

```
cp .env.example .env
```

# run nvidia nim
```
uv run uvicorn server:app --host 0.0.0.0 --port 8082
```

# install claude code
```
curl -fsSL https://claude.ai/install.sh | bash
```
# run claude code 
```
ANTHROPIC_AUTH_TOKEN="freecc" ANTHROPIC_BASE_URL="http://localhost:8082" claude
```

# Why This Method Beats Local LLMs

• **Zero Hardware Strain**: Unlike Ollama or LM Studio, which devour your RAM and CPU, this method uses cloud-hosted models. You get lightning-fast responses even on a budget laptop.

• **Better Intelligence**: Local models often struggle with complex logic. By using NVIDIA NIM, you access high-tier models that maintain the "smartness" required for production-grade coding.

• **No More Limits**: Skip the $20/month fee and the frustrating "rate limit reached" messages.

