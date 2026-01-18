# LLM Sandbox UI - Setup

Follow these steps to install and initialize the LLM Sandbox Web Interface.

## Installation
1. Create a new `conda` env, then:
  ```
  git clone https://github.com/NeuralVFX/llm-sandbox-ui
  cd llm-sandbox-ui
  pip install -e .
  ```
2. Set your `OPENAI_API_KEY`
   
  In Windows, open `PowerShell` and then:
  ```
  setx OPENAI_API_KEY "your_api_key_here"
  ```

  In Linux, open a console and:
  ```
  export OPENAI_API_KEY=""your_api_key_here"
  ```

### Set Custom Options
You can optionally edit a couple details in the `app_config.py`

- `MODEL` - LLM to run (defaults to `gpt-5.2`)
  - For tool use, I dont recommend non-GPT models
- `NOTEBOOK_SYS_PROMPT` - System prompt for default notebook interaction
- `UE_TOOL_SYS_PROMPT` - System prompt for Unreal tool use

## Initialization
1. Start Web Server
  - Start `unreal-llm-sandbox` from command line (outside of Unreal)
  - Open `http://localhost:5001/notebook/notebook.ipynb` (or any `ipynb` name)
  - If the notebook doesn't exist, a blank one is created
2. Follow instructions at [LLM Sandbox Unreal](https://github.com/NeuralVFX/llm-sandbox-unreal) to start Unreal Server
3. Check [USAGE](docs/USAGE.md) for notebook usage directions
