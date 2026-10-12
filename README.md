# mc-player-session-audit

A minimal event schema for auditing proxy session lifecycle without turning routine observability into player surveillance. Use UUIDs only where operationally necessary, restrict access, and define retention before collection.

## Events
`session.connected`, `session.transferred`, `session.disconnected`, and `session.rejected`. Include UTC timestamp, proxy node, backend identifier, correlation ID, and reason code. Do not log chat, credentials, or raw IP addresses by default.

Apply access controls and retention limits to downstream storage. MIT licensed.
