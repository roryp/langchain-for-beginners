# LangChain for Beginners (Python)

Welcome to **LangChain for Beginners**, a Python-first reboot of the original LangChain.js curriculum. This course helps you build practical AI applications using the latest **LangChain v1** and **LangGraph** capabilities, following the official guidance from the LangChain documentation.

## 🎯 Course Goals

- Understand how LangChain structures models, messages, tools, and memory in Python.
- Build reliable chat experiences with streaming, tool calling, and structured outputs.
- Orchestrate multi-step agents with LangGraph, including short-term memory management.
- Assemble Retrieval-Augmented Generation (RAG) and agentic workflows that mirror real-world production patterns.

## 📂 Course Structure

Each chapter contains a `README.md` with learning material, an `assignment.md` to reinforce the concepts, plus starter code in `code/` and reference implementations in `solution/`.

| Chapter | Focus | Highlights |
| --- | --- | --- |
| 00-course-setup | Environment & configuration | Python env, provider setup, verification script |
| 01-introduction | Core concepts | `init_chat_model`, message basics, tracing |
| 02-chat-models | Working with chat models | parameters, streaming tokens, batching |
| 03-prompts-messages-outputs | Prompt & schema design | prompt templates, few-shot, Pydantic outputs |
| 04-function-calling-tools | Tooling fundamentals | `@tool`, tool execution loops, validation |
| 05-agents-langgraph | Building agents with LangGraph | `create_agent`, middleware, memory |
| 06-documents-embeddings-semantic-search | Retrieval workflows | text splitting, embeddings, vector stores |
| 07-agentic-rag-systems | End-to-end agentic RAG | LangGraph agent + retrieval + streaming |

> 💡 **Tip**: Chapters build on one another, but each script is runnable on its own. Feel free to jump to the sections most relevant to your project.

## ✅ Prerequisites

- Python **3.10+**
- A virtual environment (e.g., `venv`, `conda`, or `uv`)
- API access to an LLM provider (GitHub Models or Azure AI Foundry are emphasized in setup)
- Basic familiarity with the command line and Git

## 📦 Install Dependencies

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

Add an `.env` file (copy `.env.example`) with credentials for your chosen provider before running any scripts.

## 🧪 Quick Start

```bash
python scripts/verify_setup.py
```

Expected output confirms your provider, model, and that LangChain is wired correctly.

## 🔄 Relationship to the JS Course

- Structure mirrors the JavaScript curriculum so you can cross-reference topics easily.
- Content is rewritten for Python idioms (`init_chat_model`, `@tool`, LangGraph middleware, `with_structured_output`).
- Examples use LangChain's recommended v1 interfaces and highlight differences from the JavaScript SDK.

## 🛟 Getting Help

- Open an issue in this repository if you spot a problem with the course content.
- Join the [LangChain Discord](https://discord.gg/langchain) for community support.
- Review the latest docs at [docs.langchain.com](https://docs.langchain.com) for API specifics.

Happy building!
