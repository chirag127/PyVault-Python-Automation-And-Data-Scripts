# PyAutomate-Workflow-Automation-Python-Toolkit

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit/ci.yml?branch=main&style=flat-square)](https://github.com/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit?style=flat-square)](https://codecov.io/gh/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit)
[![License](https://img.shields.io/github/license/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit?style=flat-square)](https://github.com/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit/blob/main/LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit?style=flat-square)](https://github.com/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit/stargazers)

A curated Python toolkit delivering ready-to-use automation and data‑processing notebooks to accelerate workflows and boost developer productivity.

## Table of Contents
- [Getting Started](#getting-started)
- [AI Agent Directives](#ai-agent-directives)
- [Development Standards](#development-standards)
- [Contribution Guidelines](#contribution-guidelines)

## Getting Started
To begin with PyAutomate, follow these steps:
1. Clone the repository: `git clone https://github.com/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Run the setup script: `python setup.py`

## AI Agent Directives
For AI-related tasks, we use the Cerebras Inference API via the OpenAI SDK.
### Client Configuration
* Base URL: `https://api.cerebras.ai/v1`
* API Key Variable: `CEREBRAS_API_KEY`
* Library: Use the standard `openai` Python library.
python
from openai import OpenAI
import os
client = OpenAI(base_url="https://api.cerebras.ai/v1", api_key=os.environ.get("CEREBRAS_API_KEY"))

### Model Hierarchy (Fallback Cascade)
Always attempt the highest-parameter model first for complex reasoning, cascading down for speed.
* Tier 1 (Frontier Intelligence): `zai-glm-4.6` (357B)
* Tier 2 (Heavy Reasoning): `qwen-3-235b-a22b-instruct-2507` (235B)
* Tier 3 (General Purpose): `gpt-oss-120b` (120B)
* Tier 4 (Balanced Workhorse): `llama-3.3-70b` (70B)
* Tier 5 (Fast Inference): `qwen-3-32b` (32B)
* Tier 6 (Ultra-Fast/Instant): `llama3.1-8b` (8B)

## Development Standards
* Follow SOLID principles
* Keep it DRY (Don't Repeat Yourself)
* YAGNI (You Ain't Gonna Need It)

## Contribution Guidelines
See [CONTRIBUTING.md](https://github.com/chirag127/PyAutomate-Workflow-Automation-Python-Toolkit/blob/main/CONTRIBUTING.md) for details on how to contribute to this project.

Star ⭐ this repository if you find it useful!