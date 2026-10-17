# Overview

This project is to help learn how to run and use local LLMs for applications. This project uses Open WebUI for a chat interface and a local LLM model to run the chat.

# Setup - Containerized LLM

- Run `docker compose up` to start the application
- Download a model inside the llmman container using the `llmman pull` command. You can exec into the container using:

    ```bash
    docker exec -it llmman bash
    ```

- Once inside the container, you can pull a model using the `llmman pull` command. For example:

    ```bash
    llmman pull hf.co/ggml-org/Qwen3.5-0.8B-GGUF:Q4_0
    ```

# Setup - Local LLM

- Download LLMMan from [GitHub](https://github.com/llmmanorg/llmman)
- Download a model from [HuggingFace](https://huggingface.co/models)
- Ensure the correct env variables are set for the LLMMan server
    - Check `.env.webui` file for the correct variables
- Run `docker compose up -f docker-compose.webui.yaml` to start the application

# Usage

- Access the web interface at [`http://localhost:3000`](http://localhost:3000) to interact with the LLMs you downloaded.

# Models

**Qwen3.5-0.8B-GGUF:Q4_0:** This is a quantized version of the Qwen3.5-0.8B model, optimized for running on local hardware.

```bash
llmman pull hf.co/ggml-org/Qwen3.5-0.8B-GGUF:Q4_0
```
