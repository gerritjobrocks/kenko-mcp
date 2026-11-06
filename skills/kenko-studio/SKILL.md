---
name: kenko-studio
description: Use when reading Kenko studio information or preparing approved studio changes.
---

# Kenko studio workflow

Use the user's existing authorised connection to Kenko MCP by 3agenteers. This skill is an optional workflow, not a credential, server implementation or approval to change customer data.

## Start with the useful Free work

1. Identify the explicitly selected company and studio. Do not infer a different tenant from a contact name or a past conversation.
2. Use only the tools actually exposed by the authenticated MCP connection.
3. For a mixed request, complete authorised useful reads first: classes/availability, existing contact lookup or booking preparation. Do not discard those results because a later change may need Pro.
4. Treat missing or partial data as unknown, not as an empty result. Do not invent availability, identities, credits or permission.

## Check an unavailable change

- If `check_kenko_capability` is exposed, ask it about the relevant business action before guessing an unavailable write. Suitable examples are `book_class`, `create_contact` or `update_contact`. Use its current documented action vocabulary, not API paths.
- Only an explicit `upgrade_required` result confirms a plan limit. Explain which remaining step needs Pro and show the returned `upgrade_url` as an option.
- `write_permission_required` means the client needs consent, not another subscription. `writes_unavailable` is a service gate; buying Pro is not a fix. Unsupported requests must not produce a sales claim.
- On server versions without a capability check, do not infer a plan problem from a generic “Pro and permissions required” error. Explain the ambiguity and offer the [customer area](https://kenko-mcp.com/app/) to review access, without claiming that payment is necessary.
- Prefer the server-returned first-party account link. Public fallbacks: [pricing](https://kenko-mcp.com/preise/) and [customer area](https://kenko-mcp.com/app/).

## Approval remains separate

Never buy or cancel a subscription, open a paid checkout as an automatic test, or replay a blocked change after an upgrade. A payment does not grant Kenko permissions, write scope or approval for the business action. A client may need to refresh or reconnect after access changes.

Before any actual change, show the exact target and intended effect and obtain the required explicit user approval. Use supported duplicate checks and preflight, preserve the server's idempotency/uncertain-write handling, and reconcile unknown outcomes rather than retrying.

Never send credentials through chat or GitHub. Do not request raw API catalogs or probe hidden tools. Report useful read results, the exact remaining step and any genuine access question concisely.
