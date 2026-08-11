# Learn Agentic AI (LangChain)

Hands-on notebooks for learning **LangChain v1** and building **agentic AI** workflows — models, tools, messages, and structured output — using Groq, Google Gemini, and OpenAI.

## What’s inside

| Notebook | Topic |
|----------|--------|
| `updatedlangchain/1-langchainintro.ipynb` | LangChain intro & first agent with tools |
| `updatedlangchain/2-modelntegration.ipynb` | Model integration (Groq / Gemini) |
| `updatedlangchain/3-tools.ipynb` | Defining and calling tools |
| `updatedlangchain/4-messages.ipynb` | Message types & chat history |
| `updatedlangchain/5-structuredoutput.ipynb` | Structured / typed model outputs |

## Stack

- Python ≥ 3.10
- [LangChain](https://python.langchain.com/) (+ community, OpenAI, Groq, Google GenAI)
- [python-dotenv](https://pypi.org/project/python-dotenv/) for local secrets
- [uv](https://github.com/astral-sh/uv) for dependency management (optional)

## Setup

### 1. Clone

```bash
git clone https://github.com/janithashri/learn-agenticAi.git
cd learn-agenticAi
```

### 2. Install dependencies

With **uv**:

```bash
uv sync
```

Or with **pip**:

```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS / Linux
# source .venv/bin/activate

pip install -r requirements.txt
pip install ipykernel
```

### 3. API keys (do not commit)

Create a `.env` file in the project root (same folder as this README). `.env` is gitignored.

```env
GOOGLE_API_KEY=your_google_api_key
GROK_API_KEY=your_groq_api_key
OPENAI_API_KEY=your_openai_api_key
```

> Notebooks map `GROK_API_KEY` from `.env` to `GROQ_API_KEY` for the Groq client.

Get keys from:

- [Google AI Studio](https://aistudio.google.com/apikey)
- [Groq Console](https://console.groq.com/)
- [OpenAI Platform](https://platform.openai.com/api-keys)

### 4. Run notebooks

Open the `updatedlangchain/` folder in VS Code / Cursor / Jupyter and run cells in order.

```bash
# optional: register kernel
python -m ipykernel install --user --name=learn-agenticAi
```

## Project layout

```
.
├── .gitignore
├── README.md
├── pyproject.toml
├── requirements.txt
├── src/langchainupdated/
└── updatedlangchain/          # learning notebooks
```

## Security

- Never commit `.env` or paste API keys into notebooks.
- Rotate any key that was shared or pushed by mistake.

## License

Personal learning project — use and adapt freely.
