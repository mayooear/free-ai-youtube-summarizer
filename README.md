## Free AI Youtube Summarizer run on your computer
Free AI Youtube Summarizer built with opensource LLM (mistral-instruct-v0.2), langchain and llama_index.

Max RAM required: 7 GB

### Setup - Download the open source model

If you're using mac or linux, download [ollama](https://ollama.ai/download) and follow these [Readme.md instructions](https://github.com/jmorganca/ollama/blob/main/README.md) to get up and running with your chosen open source large language models locally.

If you're using Windows, download the model via this account [here](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF), then adapt the code to use `llamacpp` instead of `ChatOllama` to reference the models path on your local computer. Follow these instructions [here](https://python.langchain.com/docs/integrations/llms/llamacpp)

### Usage

After you've downloaded your chosen LLM, you can change the default model name:

```
chat_model = ChatOllama(
    model="mistral",
)
```
To adapt the model's instructions, you can change the `system_prompt` variable.

Run the notebook cells to download the youtube transcript and call the model to make a prediction.
