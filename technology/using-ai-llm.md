# Using generative AI in Datahub

## Introduction

Jupyter AI integrates generative AI into Jupyter, allowing users to interact with AI models directly within their notebooks. This guide explains how to use Jupyter AI in your teaching and research.

## Disclaimer

**Note**: The DataHub infrastructure team does not currently support the deployment of Large Language Models (LLMs) for courses using DataHub. Limited compute resources and the lack of TPUs/GPUs make it challenging to deploy language models, and doing so could lead to a significant increase in cloud costs. For these reasons, deploying language models on DataHub is considered on a case-by-case basis.

In one course, a smaller language model known as DistilBERT was deployed by bumping CPU resources. Here is an [example notebook](https://data100.datahub.berkeley.edu/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2FDS-100%2Fsp24-student&urlpath=lab%2Ftree%2Fsp24-student%2F%2Fhw%2Fhw03%2Fhw03.ipynb&branch=main) using distiBERT. If you're considering using language models or any AI model in your teaching workflow, we strongly recommend scheduling a consultation with the DataHub team at the start of the semester or a few weeks prior to the assignment release. This proactive approach helps determine the feasibility and necessary optimizations to ensure smooth operations.

## Key Features

- **Magic Commands**: Use `%%ai` in notebooks to interact with AI models.
- **Chat Interface**: Chat with AI models within JupyterLab.
- **Model Support**: Works with various AI providers like OpenAI, Hugging Face, etc.
- **Local Models**: Supports running local AI models for privacy.

## Getting Started

### Setting Up API Keys

1. **Obtain API Keys**:
   - Get API keys from your chosen AI model provider (e.g., OpenAI, Hugging Face).

2. **Set Up API Keys in Your Notebook**:
   - Add your API key to the environment variables in your Jupyter notebook:
     ```python
     %env PROVIDER_API_KEY=YOUR_API_KEY_HERE
     ```

### Using Magic Commands

1. **Load the AI Magic Command**:
   - In your notebook, run:
     ```python
     %load_ext jupyter_ai
     ```

2. **Use the AI Magic Command**:
   - To generate text or perform other AI tasks, use the following command:
     ```python
     %%ai
     Your prompt to the AI model here.
     ```

### Using the Chat Interface

- **Access the Chat UI**:
  - Open the chat interface in JupyterLab to interact with the AI conversationally.

## Examples

Explore example notebooks provided in the Jupyter AI repository to see how to use the tool effectively in various scenarios.

## Getting Help

For detailed instructions, troubleshooting, and further information, refer to the [official Jupyter AI documentation](https://jupyter-ai.readthedocs.io).

By following this guide, instructors can utilize AI capabilities within Jupyter notebooks to enhance their educational and research activities.