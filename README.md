# Quartz MCP Plugin

Bundles the Quartz MDM MCP server connection with its usage-guidance Skill,
so installing this plugin sets up both at once — no separate manual Skill
upload required.

## Install

In Claude (Settings → Plugins → Add → "Add from a repository"), point at
this repo's URL (or `owner/repo` shorthand if hosted on GitHub).

## What gets installed

- **MCP connector**: `quartz-mcp`, pointing at
  `https://mcp-test.qtzit.com/mcp-v3` (OAuth via Keycloak, client ID
  `claude-mcp-connector`)
- **Skill**: `quartz-mdm-guidance` — usage instructions for the tools this
  server exposes

## Structure

```
quartz-mcp-plugin/
├── .claude-plugin/
│   └── marketplace.json      # marketplace manifest (lists the plugin below)
├── quartz-mcp/                # the plugin itself
│   ├── .claude-plugin/
│   │   └── plugin.json        # plugin metadata
│   ├── .mcp.json               # MCP server connection config
│   └── skills/
│       └── quartz-mdm-guidance/
│           └── SKILL.md
└── README.md
```
