# free_claudeCode

# Claude Code Unlimited (free)

# nvidia nim api key 
https://build.nvidia.com/

# run this in power shell 

```
wsl --install
```

# Run this command install uv

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



