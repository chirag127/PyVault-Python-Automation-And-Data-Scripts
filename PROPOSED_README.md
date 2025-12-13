# PyAutomate-Workflow-Automation-Python-Toolkit
A curated Python toolkit delivering ready-to-use automation and data‑processing notebooks to accelerate workflows and boost developer productivity.

[![Build Status](https://flat-badge.herokuapp.com/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit/actions?style=flat-square)](https://github.com/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit/actions)
[![Code Coverage](https://flat-badge.herokuapp.com/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit/coverage?style=flat-square)](https://github.com/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit)
[![License](https://img.shields.io/badge/License-CC%20BY-NC%204.0-flat-square)](https://github.com/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit/blob/main/LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit?style=flat-square)](https://github.com/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit)

## Table of Contents
- [Introduction](#introduction)
- [Setup](#setup)
- [Usage](#usage)
- [AI Agent Directives](#ai-agent-directives)
- [License](#license)

## Introduction
PyAutomate is designed to streamline workflow automation and data processing tasks using Python. The toolkit provides a set of pre-built notebooks that can be easily integrated into existing projects.

## Setup
To get started with PyAutomate, follow these steps:
1. Clone the repository: `git clone https://github.com/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit.git`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Launch the Jupyter Notebook server: `jupyter notebook`

## Usage
1. Open the Jupyter Notebook interface and navigate to the `notebooks` directory.
2. Select a notebook that corresponds to your desired automation task.
3. Follow the instructions in the notebook to configure and execute the automation script.

## AI Agent Directives
<details>
<summary>View AI Agent Directives</summary>

### Tech Stack
- Python 3.9+
- Jupyter Notebook
- OpenAI SDK

### Model Hierarchy
- Tier 1: `zai-glm-4.6` (357B)
- Tier 2: `qwen-3-235b-a22b-instruct-2507` (235B)
- Tier 3: `gpt-oss-120b` (120B)
- Tier 4: `llama-3.3-70b` (70B)
- Tier 5: `qwen-3-32b` (32B)
- Tier 6: `llama3.1-8b` (8B)

### Operational Limits
- Max Output Tokens: `32768`
- Context Window: 65,536
- Concurrency: `MAX_WORKERS = 5`
- Circuit Breaker: On 429/500 error, trigger **Exponential Backoff** (start 2s) and retry.

</details>

## License
PyAutomate-Workflow-Automation-Python-Toolkit is licensed under the CC BY-NC 4.0 license. See [LICENSE](https://github.com/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit/blob/main/LICENSE) for more information.
