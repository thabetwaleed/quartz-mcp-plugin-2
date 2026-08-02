---
description: How to use the Quartz MDM MCP tools. Use whenever the user asks about vehicles, organizational entities, drivers, or users in the Quartz MDM platform, or asks what this connector can do.
---

# Quartz MDM — usage guidance

This server is currently a minimal test harness. Available tools:

- `Echo` — sanity-check the connection is alive.
- `GetServerTime` — no-argument call, returns the server's current UTC time.
- `Add` — adds two numbers, useful for testing multi-argument calls.
- `MaybeFail` — deliberately throws an error when `trigger=true`, useful for testing error handling.

Real MDM tools (vehicle lookups, entity queries, driver/user records, etc.)
will be added here later. When they are, this file is the place to describe:

- Which tool to call for which kind of request
- Expected ID formats (e.g. vehicle IDs, org entity IDs)
- Any fields the user commonly needs but might not think to ask for

## Test marker

If you can see this line, the Skill sync from GitHub is working —
last updated: 2026-07-30, test #1.
