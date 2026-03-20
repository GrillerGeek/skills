# Claude Code Plugins

A curated collection of plugins for [Claude Code](https://claude.com/claude-code).

## Setup

Add this marketplace to Claude Code (one-time):

```bash
claude plugin marketplace add https://github.com/GrillerGeek/skills.git
```

Then install any plugin by name:

```bash
claude plugin install ux-review
```

## Available Plugins

| Plugin | Description |
|--------|-------------|
| [ux-review](https://github.com/GrillerGeek/ux-review) | Multi-agent UX review with simulated personas and specialist analysis |
| [idd-framework](https://github.com/GrillerGeek/idd-framework) | Intent-Driven Development workflow with role-specific agents for stakeholder interviews, artifact generation, and structured documentation |

## Local Testing

To test a plugin without installing, clone it and use `--plugin-dir`:

```bash
git clone https://github.com/GrillerGeek/ux-review.git
claude --plugin-dir ./ux-review
```

## Contributing

To add a plugin to this marketplace, submit a PR that:
1. Adds your plugin entry to `.claude-plugin/marketplace.json`
2. Adds a row to the table above
