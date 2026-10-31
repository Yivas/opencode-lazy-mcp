# opencode-lazy-mcp

On-demand startup for local MCP servers in OpenCode v2, with a metadata cache so the model
knows a server's tools before it runs.

**Project scaffold only.** There is no implementation, installable package, release, or verified
OpenCode compatibility yet. The next step is a feasibility test against an exact OpenCode version.

## What it is meant to do

OpenCode starts every enabled MCP server when it loads a project. OpenCode's source suggests that
each open project folder gets its own copy (not yet verified), so even small local servers can add
up, and servers that drive large applications or analysis tools cost memory and startup time even
when the session never calls them. The planned plugin keeps selected servers stopped until they are
needed, starts them after user confirmation, describes their tools from a cache while they are
stopped, and shuts them down after a period without use.

The plugin will only start servers the user has already configured and listed for it. It does not
take commands, arguments or environment values from model output, and it does not widen OpenCode's
permissions.

## Participate

This is a collaborative open-source project under the [MIT License](LICENSE).
[Issues](https://github.com/Yivas/opencode-lazy-mcp/issues) and pull requests are welcome for
documentation corrections and scoped proposals. Discuss implementation work first: no runtime design
has been approved. See [Contributing](CONTRIBUTING.md) and the [Code of Conduct](CODE_OF_CONDUCT.md).

Report sensitive findings through the process in [Security](SECURITY.md), not in a public issue.
There are no supported software versions or installation instructions at this stage.
