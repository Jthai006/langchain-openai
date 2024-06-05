# LangChain Repository

This repository contains code and resources related to the LangChain project, showcasing various NLP tasks using LangChain and OpenAI.

## Repository Structure

- **langchain-notebook**: Jupyter notebook demonstrating how to use LangChain with OpenAI for various NLP tasks. Check out `intro-to-langchain-openai.ipynb` for a step-by-step guide.

- **langserve-example**:
  - `client.py`: Python script demonstrating how to interact with a LangChain server using the langserve library. This script invokes a LangChain chain remotely by sending an HTTP request to a LangChain server.
  - `serve.py`: Python script implementing a LangChain server using FastAPI. The server hosts a LangChain agent that can process input requests and generate responses based on a predefined chain.

## Usage

### Jupyter Notebook

To explore LangChain functionality using a Jupyter notebook, navigate to the `langchain-notebook` directory and open `intro-to-langchain-openai.ipynb`.

### LangServe Example

1. Ensure you have the required dependencies installed by running:

   `pip install -r requirements.txt`

2. Start the LangChain server by running the `serve.py` script:

   `python langserve-example/serve.py`

3. Once the server is running, you can interact with it using the `client.py` script:

   `python langserve-example/client.py`

This script sends an input request to the LangChain server and prints the response.

## Dependencies

- langchain
- langchain-openai
- beautifulsoup4
- langchain_community
- faiss-cpu
- langchainhub
- uvicorn
- fastapi
- langserve
- python-dotenv
- sse_starlette

## Environment Configuration

Ensure you have the following environment variables set in your `.env` file:

`LANGCHAIN_TRACING_V2=true`

`LANGCHAIN_API_KEY={}`

`OPENAI_API_KEY={}`

`TAVILY_API_KEY={}`

Replace `{}` with your actual API keys.

## Note

- This repository assumes familiarity with LangChain and OpenAI. Make sure you have the necessary API keys and permissions to access LangChain and OpenAI services.
