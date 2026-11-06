# Kenko MCP by 3agenteers

**Your Kenko studio, connected to your AI assistant.**

Kenko MCP by 3agenteers is an independent hosted Model Context Protocol server for fitness, yoga, Pilates and other class-based studios using Kenko. Connect compatible AI assistants such as Claude and ChatGPT to the studio information you are authorised to use.

**Free for reading. Pro for approved changes. No local MCP server to run.**

[Connect your studio](https://kenko-mcp.com/app/) · [Website](https://kenko-mcp.com/) · [Free & Pro pricing](https://kenko-mcp.com/preise/) · [Deutsch](https://github.com/gerritjobrocks/kenko-mcp/blob/main/README.de.md)

## Try it with Free

- **Class availability:** “Which classes still have places next week?”
- **Contact lookup:** “Check whether this person already exists in Kenko.”
- **Booking preparation:** “Check the class and the member’s existing credits before I book them.”

These are example requests, not customer testimonials. Results depend on your Kenko permissions, available data and the client you use.

## Connect a remote MCP client

1. Open the [Kenko MCP customer area](https://kenko-mcp.com/app/) and sign in with your own Kenko account.
2. Explicitly select your company and studio.
3. Add this remote MCP server to a compatible client:

```text
https://kenko-mcp.com/mcp
```

4. Complete the client’s authorisation flow. Read-only access is enough to try Free.

The service uses **Streamable HTTP** and **OAuth with S256-PKCE**. Some clients have a native remote-connector dialog; others accept a configuration file. Formats and supported features vary by client and plan.

Example configuration for clients accepting this format:

```json
{
  "mcpServers": {
    "kenko-mcp": {
      "type": "http",
      "url": "https://kenko-mcp.com/mcp"
    }
  }
}
```

[Configuration file](https://github.com/gerritjobrocks/kenko-mcp/blob/main/examples/mcp.json) · [Setup guide](https://kenko-mcp.com/docs/install/) · [Claude guide](https://kenko-mcp.com/docs/claude/) · [Other clients](https://kenko-mcp.com/docs/cursor/)

Never put passwords or access tokens in a prompt, GitHub issue or configuration URL. Sign in through the actual login and authorisation screens.

## When you need Pro

Use Free to read and prepare. Use Pro when you explicitly want to change studio records, for example:

- Book a member into a specific class using an eligible existing credit.
- Create a contact after checking for duplicates.
- Make an approved contact-profile change.

**Pro: CHF 19 per Kenko company per month, excluding VAT.** Your Kenko subscription and AI-provider plans are separate. Pro does not extend your Kenko role or give an AI client permission to act without approval.

[Review Pro and pricing](https://kenko-mcp.com/preise/) · [Activate Pro in your customer area](https://kenko-mcp.com/app/) · [Workflow examples and limits](https://kenko-mcp.com/pro/)

## Optional agent workflow

The [Kenko studio skill](https://github.com/gerritjobrocks/kenko-mcp/blob/main/skills/kenko-studio/SKILL.md) helps an agent keep useful Free results, distinguish a genuine Pro limit from missing permissions, and ask before changes. Install it separately if your agent supports skills. Connecting an MCP server does not automatically install a skill or guarantee the same interface in every AI client.

## What this repository contains

Connection examples, setup documentation and an optional agent workflow for the hosted service. **This is not a self-hostable server distribution.** The service’s backend source and infrastructure are not included. Cloning this repository does not create a Kenko connection or activate Pro.

## Privacy, support and licence

- [Data flow and privacy](https://kenko-mcp.com/docs/datenschutz/)
- [Provider and service terms](https://kenko-mcp.com/nutzungsbedingungen/)
- Support: [gerrit@3agenteers.com](mailto:gerrit@3agenteers.com)
- [MIT licence](https://github.com/gerritjobrocks/kenko-mcp/blob/main/LICENSE) covers this repository’s documentation, configuration examples and skill, not the hosted service or its private server source.

**Independent integration by [3agenteers](https://3agenteers.com/) / Chestnut Innovation GmbH. Not an official Kenko product. Product status: Beta.**
