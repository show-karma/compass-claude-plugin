---
name: connect-compass
description: Connect or reconnect Karma Compass before using board records, or check whether the current account is ready.
---

# Connect Karma Compass

Keep the original board request pending. Connection is complete only after an
authenticated Compass tool succeeds.
Confirm success with the board's readable name and the person's role in their
language (for example, chair becomes board chair in English or presidente do
conselho in Portuguese). Record identifiers, field names and raw role values
belong only in tool calls; the reply uses plain prose, not the returned JSON.

1. If Compass tools are available, call `list_boards` once. On success, continue
   the pending request. With no pending request, ask what the person wants next.
2. If the host offers a connection or reconnection action, use it. Otherwise,
   direct the person to this plugin's Connectors tab to connect Karma Compass.
   The person signs in and approves the displayed access in Compass. Credentials
   stay in that authorization flow, outside chat and packaged files.
   Never ask for a token, password, endpoint or manual MCP configuration.
3. After authorization, call `list_boards` once and resume the original request.
   If authorization fails, explain that the account is not connected and offer
   the same connector entry to retry. Follow a returned organization-setup
   instruction before retrying the board request.

An empty board list means the connection works but no board membership is
available. Explain that a membership is needed. A denied board action is a
permissions outcome; reconnecting does not bypass the member's authority.
