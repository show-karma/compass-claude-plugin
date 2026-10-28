# Connection entry

Use the host's native connect or reconnect action first, and keep the original
request in the current conversation.

- In Claude, open this installed plugin's Connectors tab and connect Karma
  Compass. Reuse the existing connector matching the packaged server URL.
- In ChatGPT, use the installed Compass plugin's Apps connection action. If
  plugin discovery supplies its verified listing URL, use that returned URL.
  A private test package may supply its verified listing link here.

The person signs in and approves access in Compass, then returns to the same
conversation. Check authenticated access and finish their pending request.
If the host offers neither a connection action nor a verified entry, explain
that setup is incomplete and ask the publisher to supply the entry. A guessed
plugin ID, OAuth URL, pasted token or manual MCP registration is not a recovery.
