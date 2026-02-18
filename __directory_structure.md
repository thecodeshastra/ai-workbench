# ai-workbench Structure

```text
ai-workbench/
├── .github
│   └── workflows
│       └── deploy-docs.yml
├── docs
│   ├── api-reference
│   │   ├── core-modules.md
│   │   ├── stateless-agent.md
│   │   ├── summarizer-agent.md
│   │   └── virtual-assistant-agent.md
│   ├── user-guide
│   │   ├── getting-started.md
│   │   ├── stateless-agent.md
│   │   ├── summarizer-agent.md
│   │   └── virtual-assistant-agent.md
│   └── index.md
├── resources
│   ├── actions.txt
│   └── Meeting summary.txt
├── src
│   ├── agents
│   │   ├── stateless_agent
│   │   │   ├── __init__.py
│   │   │   ├── base_agent.py
│   │   │   └── prompt.py
│   │   ├── summarizer_agent
│   │   │   ├── __init__.py
│   │   │   ├── async_executor.py
│   │   │   ├── executor.py
│   │   │   ├── planner.py
│   │   │   └── prompt.py
│   │   ├── virtual_assistant_agent
│   │   │   ├── memory
│   │   │   │   ├── persona
│   │   │   │   │   ├── profile.pdf
│   │   │   │   │   └── summary.txt
│   │   │   │   ├── __init__.py
│   │   │   │   ├── experience.json
│   │   │   │   ├── memory_manager.py
│   │   │   │   └── unknowns.json
│   │   │   ├── __init__.py
│   │   │   ├── agent.py
│   │   │   ├── common.py
│   │   │   ├── constants.py
│   │   │   ├── critic.py
│   │   │   ├── executor.py
│   │   │   ├── memory_selector.py
│   │   │   ├── persona_loader.py
│   │   │   ├── planner.py
│   │   │   └── prompt.py
│   │   └── __init__.py
│   ├── apps
│   │   └── virtual_assistant_chatbot.py
│   ├── config
│   │   ├── __init__.py
│   │   └── settings.py
│   ├── core
│   │   ├── prompts
│   │   │   ├── base_persona.py
│   │   │   ├── extract_action.py
│   │   │   └── text_summarizer.py
│   │   ├── providers
│   │   │   ├── __init__.py
│   │   │   ├── anthropic.py
│   │   │   ├── gemini.py
│   │   │   ├── huggingface.py
│   │   │   ├── litellm.py
│   │   │   ├── mock_provider.py
│   │   │   ├── ollama.py
│   │   │   ├── openai.py
│   │   │   └── perplexity.py
│   │   ├── tools
│   │   │   ├── __init__.py
│   │   │   ├── extract_action.py
│   │   │   ├── file_read.py
│   │   │   ├── file_write.py
│   │   │   ├── text_summarizer.py
│   │   │   └── tool_registry.py
│   │   ├── utils
│   │   │   ├── __init__.py
│   │   │   ├── context.py
│   │   │   └── logger.py
│   │   ├── __init__.py
│   │   └── provider_factory.py
│   ├── interfaces
│   │   ├── __init__.py
│   │   ├── base_provider.py
│   │   └── base_tool.py
│   ├── __init__.py
│   ├── run_stateless_agent.py
│   ├── run_summarize_agent.py
│   └── run_virtual_assistant.py
├── tests
│   ├── agents
│   │   ├── stateless_agent
│   │   │   └── test_base_agent.py
│   │   ├── summarizer_agent
│   │   │   ├── test_async_executor.py
│   │   │   ├── test_executor.py
│   │   │   └── test_planner.py
│   │   └── virtual_assistant_agent
│   │       ├── memory
│   │       │   └── test_memory_manager.py
│   │       ├── test_agent.py
│   │       ├── test_common.py
│   │       ├── test_critic.py
│   │       ├── test_executor.py
│   │       ├── test_memory_selector.py
│   │       ├── test_persona_loader.py
│   │       └── test_planner.py
│   ├── core
│   │   ├── providers
│   │   │   └── test_mock_provider.py
│   │   └── test_provider_factory.py
│   └── __init__.py
├── .env
├── .gitignore
├── CHANGELOG.md
├── LICENSE
├── mkdocs.yml
├── pyproject.toml
├── README.md
└── uv.lock
```
