# Advanced NLP: Llama-3-8B-Instruct Implementation

This repository contains a Jupyter notebook for an **Advanced Natural Language Processing** project focused on utilizing large language models (LLMs). The project specifically implements the **Meta-Llama-3-8B-Instruct** model using the Hugging Face `transformers` library.

## Project Overview

The notebook demonstrates the setup and initialization of a state-of-the-art causal language model. It utilizes advanced techniques for efficient model loading and inference, including:
- **4-bit Quantization**: Using `bitsandbytes` to reduce the model's memory footprint, allowing it to run on consumer-grade GPUs (like the T4).
- **Accelerated Inference**: Leveraging the `accelerate` library for optimized performance.
- **Hugging Face Integration**: Utilizing the `pipeline` API for streamlined text generation.

## Repository Structure

| File | Description |
| :--- | :--- |
| `ex2anlp.ipynb` | The main Jupyter notebook containing the implementation and setup for the Llama-3 model. |
| `README.md` | Documentation providing an overview of the project, requirements, and setup instructions. |

## Requirements

To run the notebook, you will need a Python environment with the following libraries installed:
- `transformers`
- `accelerate`
- `bitsandbytes`
- `torch` (PyTorch)

You can install the dependencies using:
```bash
pip install transformers accelerate bitsandbytes torch
```

## Important Setup Note

The **Meta-Llama-3-8B-Instruct** model is a **gated model** on Hugging Face. To use it, you must:
1. Request access to the model on the [official Hugging Face page](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct).
2. Create a Hugging Face **Access Token** in your [account settings](https://huggingface.co/settings/tokens).
3. Authenticate your environment (e.g., using `huggingface-cli login` or setting the `HF_TOKEN` environment variable).

## Authors
- Malak Laham
- Zenab Waked
