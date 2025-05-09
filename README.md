# Ben Needs a Friend: 2025 edition
This directory contains materials from the Ben Needs a Friend tutorial given at ODSC East 2025.

## Contents
[Slides]()
`ben-friend-in-context-learning`: Introduction to using LLMs with llamabot and basic in context learning methods.  Can be run in Codespaces.
`ben-friend-rag`: Example for Retrieval-Augmented Generation.  Can be run in Codespaces.
`ben-friend-sft`: Supervised Fine-Tuning of the Llama3.2 model using Unsloth.  Designed to be run in Google Colab.
`ben-friend-agent`: Building an agent that interacts with tools.  Cannot run on Codespaces due to instance size limitations.

## Setup
The first two notebooks can be run in Github Codespaces.  The SFT notebook is designed for Google Colab.  The agent notebook requires a larger LLM, which would be best to run locally.

### Codespace setup
* Click the "Use as template" button in the top right of the repository page
* Wait a few minutes while the devcontainer starts and installs the necessary libraries
* Open the first notebook (in-context-learning)
* In the top right, ensure the default (Python 3.10) kernel is selected
* You should be able to run the first cell.  If not, refresh your browser.  If that doesn't work, try the "Use as template" portion again.
* Follow the steps below to download the required models to the codespace

### Downloading the required models


in the top right of this repository.  Once you click that, a devcontainer should start up.  You will need to wait a few minutes and potentially refresh your browser to have a working environment.

### Downloading models




There should be a button that says "Use as Template" in the repository.  Once you click tha

I use [pixi](https://pixi.sh/latest/) as the environment manager for the tutorial section.  You will need to follow setup instructions there to install.

For Linux/Mac OS: `curl -fsSL https://pixi.sh/install.sh | sh`

