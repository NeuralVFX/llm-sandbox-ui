# LLM Sandbox UI - Setup

Follow these steps to install and initialize the LLM Sandbox Web Interface

## Installation
1. Create a new `conda` env, then:
  ```
  git clone https://github.com/NeuralVFX/llm-sandbo-ui
  cd unreal-llm-sandbox
  pip install -e .
  ```
2. Set your `OPENAI_API_KEY`
  In Windows, open `Powershell` and then:
  ```
  setx OPENAI_API_KEY *Your_API_key*
  ```

  In Linux, open a console and:
  ```
  export OPENAI_API_KEY="Your_API_key"
  ```

# Unreal Server

Follow instructions at **[llm-sandbox-unreal](https://github.com/NeuralVFX/llm-sandbox-unreal)** to install Unreal side

    
### Initialization
1. Start Web Server
  - Start `unreal-llm-sandbox` from command line ( outside of Unreal )
  - Open `http://localhost:5001/notebook/notebook.ipynb` ( or any `ipynb` name )
  - If the notebook doesn't exist, a blank one is created
2. Follow instructions at [LLM Sandbox Unreal](https://github.com/NeuralVFX/llm-sandbox-unreal) to start Unreal Server
3. Check [USAGE](docs/USAGE.md) for notebook usage directions
