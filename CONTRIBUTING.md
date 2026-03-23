# Contributing

Thanks for your interest in contributing to the Claude Code Plugins marketplace!

## Adding a Plugin

To submit a new plugin, open a pull request that includes:

### 1. Add your plugin to the marketplace registry

Add an entry to `.claude-plugin/marketplace.json` in the `plugins` array:

```json
{
  "name": "your-plugin-name",
  "description": "A clear, concise description of what your plugin does.",
  "category": "development",
  "source": {
    "source": "url",
    "url": "https://github.com/your-username/your-plugin.git"
  },
  "homepage": "https://github.com/your-username/your-plugin"
}
```

**Source types:**

- `url` — the entire repo is the plugin
- `git-subdir` — the plugin lives in a subdirectory (add a `"path"` field)

### 2. Add a row to the README

Add your plugin to the **Available Plugins** table in `README.md`:

```markdown
| [your-plugin](https://github.com/your-username/your-plugin) | Category | Brief description of your plugin. |
```

### 3. Plugin requirements

Before submitting, ensure your plugin:

- Has a clear `README.md` in its own repository
- Includes a valid `.claude-plugin/` manifest
- Works with the current version of Claude Code
- Does not include credentials, API keys, or secrets
- Has a license (we recommend Apache 2.0 or MIT)

## Reporting Issues

Found a problem with the marketplace or an existing plugin listing? [Open an issue](https://github.com/GrillerGeek/skills/issues/new) with:

- Which plugin is affected (or if it's a marketplace-level issue)
- Steps to reproduce
- Expected vs. actual behavior

## Code of Conduct

Be respectful and constructive. We're all here to build better tools.
