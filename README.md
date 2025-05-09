# Ben Needs a Friend: 2025 edition
This directory contains materials from the Ben Needs a Friend tutorial given at ODSC East 2025.

## Contents
[Slides](https://docs.google.com/presentation/d/1w6gT7euYzIGRJIr60SXdX_3Kl8GCmK4o2gWikes-v0Q/edit?usp=sharing)
`ben-friend-in-context-learning`: Introduction to using LLMs with llamabot and basic in context learning methods.  Can be run in Codespaces.
`ben-friend-rag`: Example for Retrieval-Augmented Generation.  Can be run in Codespaces.
`ben-friend-sft`: Supervised Fine-Tuning of the Llama3.2 model using Unsloth.  **Designed to be run in Google Colab.**
`ben-friend-agent`: Building an agent that interacts with tools.  **Cannot run on Codespaces due to instance size limitations.**

## Setup
The first two notebooks can be run in Github Codespaces.  The SFT notebook is designed for Google Colab.  The agent notebook requires a larger LLM, which would be best to run locally.

### Codespace setup
* Click the "Use as template" button in the top right of the repository page
* Wait a few minutes while the devcontainer starts and installs the necessary libraries
* Open the first notebook (in-context-learning)
* In the top right, ensure the default (Python 3.10) kernel is selected
* You should be able to run the first cell.  If not, refresh your browser.  If that doesn't work, try the "Use as template" portion again.
* Follow the steps below to download the required models to the codespace

_NOTE_: Codespaces is finicky, 

### Local setup
* I recommend you use VSCode with Jupyter notebook support extension
* Install the [pixi](https://pixi.sh/latest/) environment manager
* Install [ollama](https://ollama.com/)
* In this directory run `pixi install`
* Open the first notebook (in-context-learning)
* In the top right, ensure the pixi environment `default` (Python 3.10) kernel is selected
* Follow the steps below to download the required models

### Downloading the required models
Ollama will be used to download the required models.  If you are using Codespaces, you will need to open a new terminal to run these commands.

For notebook 1 (in-context) and 2 (rag) you will just need the following models:

```
ollama pull llama3.2:1b-text-q5_K_S
ollama pull qwen2.5:1.5b
```

For notebook 4 (agent), you will need this model.  Note, this is too big to fit in the basic Codespaces instances, so plan to run this locally instead.

`ollama pull qwen2.5:7b`

