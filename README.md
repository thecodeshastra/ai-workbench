# AI-workbench [Tomb-stoned]

A reusable library of AI agents for various automation tasks. This workbench includes stateless and stateful agents that can be used for code generation, text summarization, and multi-step task execution.

##

### [For Documentation Click Here](https://thecodeshastra.github.io/AI-workbench/)

## Features

- **Stateless Agent**: Lightweight, one-shot request/response agent for quick queries and code generation
- **Summarizer Agent**: Advanced planning and execution agent with async support for complex tasks
- **Virtual Assistant Agent**: Persona-based chatbot that learns over time and maintains memory via a critic-led cycle
- **Multi-Provider Support**: Works with Gemini, OpenAI, Anthropic, LiteLLM, Ollama, Perplexity, HuggingFace, and more
- **Extensible Architecture**: Easy to add new agents and tools

## Installation

1. **Clone the repository:**

   ```bash
   git clone <repository-url>
   cd AI-workbench
   ```

2. **Create and activate a virtual environment:**

   ```bash
   uv venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

3. **Install dependencies:**

   ```bash
   uv sync
   # To install optional test dependencies:
   uv sync --all-extras
   ```

4. **Configure environment variables:**
   Create a `.env` file with your API keys:

   ```env
   GOOGLE_API_KEY=your_api_key_here
   ```

## Usage

### Stateless Agent

### Stateless Agent

Run the stateless agent for quick, one-off requests:

```bash
uv run stateless-agent
```

### Summarizer Agent

Run the summarizer agent for planning and multi-step tasks:

```bash
uv run summarizer-agent
```

### Virtual Assistant Agent

Run the virtual assistant agent for persona-based interactions:

```bash
uv run virtual-assistant
# or to launch the chatbot interface:
uv run virtual-assistant-chatbot
```

## Documentation

This project uses **MkDocs** with the Dracula theme for documentation.

### View Documentation Locally

```bash
mkdocs serve
```

Then open <http://127.0.0.1:8000> in your browser.

### Build Documentation

```bash
mkdocs build
```

### Deploy to GitHub Pages

```bash
mkdocs gh-deploy
```

### Quick MkDocs Notes

- Configuration: `mkdocs.yml`
- Documentation source: `docs/` folder
- User guides: `docs/user-guide/`
- API reference: `docs/api-reference/`
- Current theme: Dracula (dark mode)

## Project Structure

```text
AI-workbench/
├── src/
│   ├── agents/          # Agent implementations
│   ├── apps/            # Application interfaces runner
│   ├── core/            # Core modules (providers, tools, utils)
│   ├── config/          # Configuration settings
│   ├── interfaces/      # Base interfaces
│   └── run_*.py         # Agents Runner scripts
├── docs/                # MkDocs documentation
├── tests/               # Unit tests
└── requirements.txt     # Python dependencies
```

## License

See [LICENSE](LICENSE) file for details.
