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
