## Build an autonomous AI Agent that Chats on your behalf

## Setup

### Clone this repository

`git clone https://github.com/kagozi/Chat-bot.git`

### Install Cursor
1. Visit cursor at `https://www.cursor.com/`
2. Sign In then create your account
3. Download, install and open Cursor
4. Click "Open project" and open the folder named "Chat-bot"

### Install `uv` package manager
Follow the instructions in this page:
`https://docs.astral.sh/uv/getting-started/installation/`

### Create a virtual environment and install the packages
Simply run:  
`uv sync`  

### API Keys (Optional)
For the best results, I would recommend a propietary model from Open AI or Gemini. Alternatively, you can use Ollama, a locally run model.

For OPEN AI, set up your OpenAI key at `https://platform.openai.com/api-keys` 
Copy the keys and paste it in the `OPENAI_API_KEY` field

### PUSH NOTIFICATIONS
Visit `https://pushover.net/` and click 'Login or Signup' and create your API keys.


### Deployment to HF
To deploy to HuggingFace:
1. create an account here: `https://huggingface.co`
2. Click on the Avatar, select the Access Tokens and Create New Token. Give it WRITE permissions.
Run: `uv tool install 'huggingface_hub[cli]'` to install the HuggingFace tool, then `hf auth login --token YOUR_TOKEN_HERE`, like `hf auth login --token hf_xxxxxx`,

### Update your .env file:
```
mv .env.example .env
```

Update the variables in the .env with your values:

```
OPENAI_API_KEY=xxxx
GOOGLE_API_KEY=xxxx
ANTHROPIC_API_KEY=xxxx
DEEPSEEK_API_KEY=xxxx
PUSHOVER_USER=xxxx
PUSHOVER_TOKEN=xxxx
HF_TOKEN=xxxx
```

Run `uv run gradio deploy`
Follow the instruction, create a folder and name it chat-bot. Specify app.py, choose cpu-basic as the hardware
