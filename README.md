# FlyDocs for Cursor

Spec-driven development workflow: your agent works issues, sessions and the status lifecycle.

[![Add flydocs to Cursor](https://cursor.com/deeplink/mcp-install-dark.svg)](cursor://anysphere.cursor-deeplink/mcp/install?name=flydocs&config=eyJjb21tYW5kIjoibnB4IiwiYXJncyI6WyIteSIsIkBmbHlkb2NzL2NsaSIsIm1jcCJdfQ==)

## What it does

FlyDocs turns your issue tracker into the spec surface for AI coding agents. This plugin registers the FlyDocs MCP server, which gives your agent the tools a working session runs on: reading the spec (`issue_get`, `issue_list`), capturing and starting work (`issue_create`, `issue_activate`), moving an issue with the audit trail the move needs (`issue_transition`, `issue_comment`, `issue_acceptance_update`), running the session itself (`session_start`, `session_wrap`, `project_update`), and asking what shipped around an issue (`change_context`). Every tool is annotated read-only or mutating, so Cursor can tell a question from a write before it runs one.

## Setup

1. Click **Add to Cursor** above, or install the CLI directly: `npm install -g @flydocs/cli && flydocs init`
2. Enable the **flydocs** server under Settings → Cursor Settings → MCP.
3. Learn more at [flydocs.ai](https://www.flydocs.ai).

## License

MIT, for this wrapper repository only. The FlyDocs CLI (`@flydocs/cli`) is distributed under its own terms via npm.
