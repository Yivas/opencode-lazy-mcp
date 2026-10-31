# Security

## Supported versions

| Line | Support |
| --- | --- |
| Repository scaffold | Documentation reports only; no executable software |
| Software releases | None published or supported |

This repository does not yet implement a plugin, start processes or install dependencies. The
planned design starts and stops MCP server processes that the user has configured; until it exists
and is tested, no part of it is a security boundary.

## Reporting

Use [GitHub private vulnerability reporting](https://github.com/Yivas/opencode-lazy-mcp/security/advisories/new)
for sensitive findings involving this repository. Do not publish exploit details or private data in
issues or pull requests. If the private form is unavailable, open an issue asking for a private
contact without disclosing the finding.

Include the affected commit or file, environment, a minimal sanitized reproduction, impact and any
workaround. Remove tokens, credentials, personal information, conversations, private endpoints and
MCP server configuration with real values. Do not attach complete session logs.

The maintainer will assess scope, request missing evidence when needed, and coordinate a correction
or disclosure. No response deadline, bounty, CVE assignment or embargo is promised. Findings in
OpenCode, MCP servers or other dependencies belong to their maintainers unless this repository
contributes to the problem.
