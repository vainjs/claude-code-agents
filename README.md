# Claude Code Agents

A curated collection of Claude Code agents and plugins for enhanced development workflows.

## Overview

This repository provides reusable agents and slash commands for [Claude Code](https://claude.com/claude-code), designed to enforce code standards, automate common tasks, and improve development productivity.

## Quick Start

### Add this marketplace to Claude Code

```bash
/plugin marketplace add vainjs/claude-code-agents
```

### Browse available plugins

```bash
/plugin
```

### Install the plugins you need

```bash
/plugin install react-code-standards
```

## Project Structure

```
claude-code-agents/
├── .claude/                 # Claude Code configuration
├── .claude-plugin/          # Plugin registry
└── plugins/                 # Plugin collection
    └── react/               # React/TypeScript plugin
        ├── agents/          # Code standards agent
        ├── commands/        # Review, gen, refactor commands
        └── README.md        # Detailed usage guide
```

## Available Plugins

### React Plugin

TypeScript/React code standards enforcement with automated review, generation, and refactoring capabilities.

**📖 [Full Documentation](plugins/react/README.md)**

## Contributing

Contributions are welcome! To add new plugins or improve existing ones:

1. Fork the repository
2. Create a feature branch
3. Add your plugin following the existing structure
4. Submit a pull request

## License

MIT License - see [LICENSE](LICENSE) file for details.
