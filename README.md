# Overview

This project is to help learn how to run and use local LLMs for applications. This project uses Open WebUI for a chat interface and a local LLM model to run the chat.

# Setup

- Download LLMMan from [GitHub](https://github.com/llmmanorg/llmman)
- Download a model from [HuggingFace](https://huggingface.co/models)
- Run `docker compose up` to start the application
- Open your browser and go to [`http://localhost:3000`](http://localhost:3000) to access the chat interface

# Models

**Qwen3.5-0.8B-GGUF:Q4_0:** This is a quantized version of the Qwen3.5-0.8B model, optimized for running on local hardware.

```bash
llmman pull hf.co/ggml-org/Qwen3.5-0.8B-GGUF:Q4_0
```
