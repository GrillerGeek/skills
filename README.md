# Claude Code Plugins

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](LICENSE)
[![Plugins](https://img.shields.io/badge/plugins-2-green.svg)](#available-plugins)
[![Claude Code](https://img.shields.io/badge/Claude_Code-compatible-blueviolet.svg)](https://claude.com/claude-code)

A curated marketplace of plugins for [Claude Code](https://claude.com/claude-code). Browse, install, and extend your AI coding workflow with specialized review agents and development frameworks.

## Quick Start

**1. Add this marketplace** (one-time):

```bash
claude plugin marketplace add https://github.com/GrillerGeek/skills.git
```

**2. Install a plugin**:

```bash
claude plugin install ux-review
```

That's it — the plugin is ready to use in your next Claude Code session.

## Available Plugins

| Plugin | Category | Description |
|--------|----------|-------------|
| [ux-review](https://github.com/GrillerGeek/ux-review) | Review | Multi-agent UX review with simulated user personas and specialist analysis. Orchestrates intake interviews, persona research, app walkthroughs, and technical/visual specialist reviews into a prioritized backlog. |
| [idd-framework](https://github.com/GrillerGeek/idd-framework) | Development | Intent-Driven Development workflow with role-specific agents for stakeholder interviews, artifact generation, and structured documentation. Decomposes purpose into Product, Intention, Expectation, and Spec artifacts. |

## Local Testing

To test a plugin without installing it globally, clone and reference it directly:

```bash
git clone https://github.com/GrillerGeek/ux-review.git
claude --plugin-dir ./ux-review
```

## Contributing

We welcome new plugins! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to submit yours.

## License

This project is licensed under the [Apache License 2.0](LICENSE).
