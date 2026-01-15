## Build an autonomous AI Agent that Chats on your behalf

## Setup

### Clone this repository

`
git clone https://github.com/kagozi/Chat-bot.git
`

### Install Cursor
1. Visit cursor at https://www.cursor.com/
2. Sign In then create your account
3. Download, install and open Cursor
4. Click "Open project" and open the folder named "Chat-bot"

### Install `uv` package manager
Follow the instructions in this page:
`
https://docs.astral.sh/uv/getting-started/installation/
`

### Create a virtual environment and install the packages
Simply run:  
`uv sync`  

### API Keys (Optional)
For the best results, I would recommend a propietary model from Open AI or Gemini. Alternatively, you can use Ollama, a locally run model.

For OPEN AI, set up your OpenAI key at https://platform.openai.com/api-keys 
Copy the keys and paste it in the `OPENAI_API_KEY` field

```
OPENAI_API_KEY=
GOOGLE_API_KEY=xxxx
ANTHROPIC_API_KEY=xxxx
DEEPSEEK_API_KEY=xxxx
```
