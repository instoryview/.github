# Instoryview

**Instoryview is an Instagram follower and following tracker with a free story viewer and developer tools.** It detects new followers, lost followers, new following and unfollowed accounts for the public accounts you track, and exposes the same data through an Open API, a CLI, an AI agent Skill and an MCP server. → [instoryview.com](https://instoryview.com)

## Repositories

| Repository | What it is | Install |
|---|---|---|
| [**cli**](https://github.com/instoryview/cli) | Command line for your tracked accounts, snapshots and detected changes | `npm install --global instoryview` |
| [**skill**](https://github.com/instoryview/skill) | Agent Skill for Claude Code, Codex, Cursor and other assistants | `npx skills add instoryview/skill` |
| [**chatgpt-plugin**](https://github.com/instoryview/chatgpt-plugin) | ChatGPT / Codex Plugin preview and remote MCP connection | MCP: `https://instoryview.com/mcp` |
| [**app**](https://github.com/instoryview/app) | Android and iOS app | Android: internal testing |
| [**story-viewer**](https://github.com/instoryview/story-viewer) | Free Instagram story viewer for public accounts | [instoryview.com/stories](https://instoryview.com/stories) |

## For developers and AI assistants

- **Open API:** six endpoints under `https://instoryview.com/open-api/v1` (tracking, account, followers, following, changes, budgeted queries). [Reference](https://instoryview.com/docs/reference)
- **MCP server:** `https://instoryview.com/mcp` (OAuth). [Plugins and MCP](https://instoryview.com/docs/plugins)
- **Docs:** [instoryview.com/docs](https://instoryview.com/docs) · [How tracking works](https://instoryview.com/how-tracking-works)

## Principles

Changes are reported as *detected* between scans, never as the exact moment someone followed or unfollowed, because Instagram publishes no follow timestamps. Reads of existing data do not start a scan. No Instagram password is ever requested. Account owners can remove their account at [instoryview.com/removal](https://instoryview.com/removal).

Support: support@instoryview.com
