# NotebookAI

Chat with a coding agent directly inside Jupyter using a `%ai` magic command.

Inspired by [solveit](https://solve.it.com/) from Jeremy Howard and [Answer.ai](https://www.answer.ai/).

## Usage

```python
%ai fix the bug in the function above
```

The magic reads all cells above it as context, sends them to an LLM, and renders the response as Markdown.

## Setup

Requires: `openai`, `httpx`, `fastcore`

Run the cells in `notebookai.ipynb` to register the magic.

## TODO

Build a simple notebook frontend with the full coding loop:

- **FastHTML** for the web UI (cells, editor, output rendering)
- **jupyter-server-client** for REST API (file management, sessions, kernel lifecycle)
- **jupyter_client** for execution with streaming output (via WebSocket)
- **nbformat** for notebook structure and validation

Goal: minimal, working notebook interface that can create notebooks, execute code cells with real-time output streaming, and save results.
