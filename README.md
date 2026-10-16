# Zenmoney skills

Agent skills and the Claude plugin for [Zenmoney](https://zenmoney.app), a personal finance app with automatic bank sync. The plugin connects Claude to your Zenmoney account and adds the Financial Brief skill. See [skills/zenmoney/README.md](skills/zenmoney/README.md) for what it does, setup, and data and privacy.

## Install in Claude Code

```
/plugin install zenmoney --marketplace zenmoney/skills
```

On Claude Code versions before 2.1.275, add the marketplace first:

```
/plugin marketplace add zenmoney/skills
/plugin install zenmoney@zenmoney
```

Then run `/mcp`, pick `zenmoney`, and sign in to your Zenmoney account.

## Repository layout

- `skills/zenmoney/`: the skills and the plugin's README
- `.claude-plugin/`: the Claude plugin manifest and marketplace

## License

MIT
