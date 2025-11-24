# Ollama LLM Council (HTML)

This lightweight page mirrors Andrej Karpathy's [llm-council](https://github.com/karpathy/llm-council) workflow while matching the simple HTML style used in the existing HTML Meetings files. A group of council members (specialists) responds to the user's question over one or more rounds, and a Mayor synthesizes the final answer. All calls are sent to a local Ollama instance via the `POST /api/chat` endpoint.

## Running
1. Start Ollama locally and ensure your model name matches the `MODEL` constant in the HTML (default: `deepseek-r1:8b`).
2. Open `OllamaLLMCouncil.html` in a modern browser.
3. Optionally adjust the global system prompt, Mayor directive, council role list, council size, and number of deliberation rounds.
4. Ask a question and watch the council responses followed by the Mayor's synthesis.
