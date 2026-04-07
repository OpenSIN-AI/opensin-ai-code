# OpenSIN-AI Code — The Ultimate AI Agent Development Platform

[![Documentation](https://img.shields.io/badge/docs-docs.opensin.ai-blue)](https://docs.opensin.ai)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/python-3.11%2B-blue.svg)](https://www.python.org/downloads/)
[![Tests](https://img.shields.io/badge/tests-2138%20passing-green.svg)](tests/)

OpenSIN-AI Code is a comprehensive AI agent development platform that enables you to build, deploy, and manage autonomous AI agent systems at scale. Built from the ground up for multi-agent collaboration with our A2A (Agent-to-Agent) protocol.

## 🚀 Quick Start

```bash
# Install the platform
pip install opensin-ai-code

# Create your first agent
opensin-ai agent create researcher --model gpt-4

# Test your agent
opensin-ai agent test researcher --prompt "What is AI?"

# Create a team
opensin-ai team create research-team --strategy sequential

# Execute a team task
opensin-ai team exec research-team --task "Research AI trends"
```

## 🔧 Installation

### From PyPI
```bash
pip install opensin-ai-code
```

### From Source
```bash
git clone https://github.com/OpenSIN-AI/opensin-ai-code.git
cd opensin-ai-code
pip install -e .
```

### Development Installation
```bash
git clone https://github.com/OpenSIN-AI/opensin-ai-code.git
cd opensin-ai-code
pip install -e ".[dev]"
```

## 📦 Packages

| Package | Description | Status |
|---------|-------------|--------|
| [`opensin-ai-core`](src/) | Core engine with QueryEngine, Hook System, Tool System, Permission System, Subagent System, MCP Client, Sandbox, Memory System | ✅ Stable |
| [`opensin-ai-cli`](src/main.py) | Command-line interface for managing agents and teams | ✅ Stable |
| [`opensin-ai-sdk`](src/) | Python SDK for programmatic access (integrated) | ✅ Stable |

## 🧠 Core Features

### QueryEngine
Async generator pattern with ReAct loop, token budget tracking, and automatic context compaction.

### Hook System
20+ hook events with 5 execution modes (shell, HTTP, function, agent, prompt) for powerful automation.

### Tool System
Rich tool interface with 8 built-in tools, deferred loading, and permission-aware filtering.

### Permission System
Multi-source permission rules with auto-mode classifier and bypass-immune safety checks.

### Subagent System
Fork pattern with cache-identical prefixes, worktree isolation, and background-to-foreground transitions.

### MCP Client
Multi-transport support (stdio, SSE, HTTP, WS, in-process) with OAuth authentication.

### Sandbox
Secure code execution with filesystem/network rules and git escape prevention.

### Memory System
File-based memory with index and topic files, SIN.md auto-discovery, and session memory extraction.

## 📚 Documentation

Full documentation is available at [docs.opensin.ai](https://docs.opensin.ai), with comprehensive coverage of:

- [Getting Started](https://docs.opensin.ai/guide/getting-started)
- [API Reference](https://docs.opensin.ai/api/overview)
- [Tutorials](https://docs.opensin.ai/tutorials/agent-basics)
- [Integrations](https://docs.opensin.ai/integrations/telegram)
- [Architecture](https://docs.opensin.ai/architecture/overview)
- [Best Practices](https://docs.opensin.ai/best-practices/overview)
- [SIN Features](https://docs.opensin.ai/guide/sin-features)

## 🐳 Local Development

```bash
# Clone the repository
git clone https://github.com/OpenSIN-AI/opensin-ai-code.git
cd opensin-ai-code

# Setup development environment
./scripts/setup.sh

# Run tests
./scripts/test.sh

# Start development server (for API mode)
opensin-ai server start
```

## 🧪 Testing

```bash
# Run all tests
./scripts/test.sh

# Run specific test suites
python -m pytest src/core/ -v
python -m pytest src/cli/ -v
python -m pytest tests/integration/ -v
```

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guide](CONTRIBUTING.md) for details.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📊 Project Stats

- **2,138+** lines of Python code
- **66** Python files
- **26** subsystem packages
- **1** core platform
- **Complete metadata-driven architecture**

## 🌐 Community

- **Documentation:** https://docs.opensin.ai
- **GitHub:** https://github.com/OpenSIN-AI/opensin-ai-code
- **Discord:** https://discord.gg/opensin-ai-code
- **Issues:** https://github.com/OpenSIN-AI/opensin-ai-code/issues

## 📄 License

This project is licensed under the Apache 2.0 License - see the [LICENSE](LICENSE) file for details.

---
Built with ❤️ by the OpenSIN-AI Team