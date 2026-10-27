# Prepare a meeting through the connector

Use the shared [source and freshness rules](source-and-freshness.md) from the
platform's meeting-preparation skill. Its internal tool names and durable job
lifecycle are not part of this host. Discover the equivalent authorized
operations through MCP; do not start or settle an internal agent job.

For "help me prepare our next board meeting", start with a preparation brief:
read the available sources below and report the meeting/date, current agenda,
prior decisions needing follow-up, open actions with recorded owners and dates,
and missing information. Link each material finding to its returned source.
This request alone does not authorize saving an agenda, generating a packet or
contacting anyone. Continue to the draft/save steps only when the person asks
to draft, create or change the agenda; publication still needs its human step.

1. Find upcoming meetings. Select the meeting the person named; if no meeting
   matches, explain what is missing and offer scheduling. When scheduling is
   requested, use the returned contract and name who will be invited. An empty
   invitee list means nobody is invited, even when the board has members.
2. Read the meeting workspace, current agenda and version, readiness, meeting
   objectives, prior agendas and minutes, open actions, submissions and paper
   attachments. For prior minutes, list them with `board.minutes.review.list`,
   then read each one's text with `board.minutes.review.get` (see
   [records](records.md)). Search the governing documents for any rule that
   changes the proposal. Use the API's quorum projection rather than
   calculating a rule from an old agenda or inventing a ratio.
3. Separate recorded facts, recommendations and missing inputs. For a requested
   agenda draft, preserve sound
   work in the existing agenda. Use supported business and unresolved prior
   decisions; group open actions as follow-up work. Give each agenda item its
   purpose and a duration that fits the meeting. Name a presenter, owner or
   paper only when a source names one. Missing records are a reason to explain
   the gap, not to add generic business to fill the time.
4. When agenda drafting or editing was requested, compare the proposal with the current agenda. If no material change is
   needed, keep it and report what you checked. Otherwise save one complete,
   reversible draft through the discovered agenda operation, using the current
   version as its base where required. Resolve a version conflict by reading
   again and rebuilding the proposal, not by overwriting another person's work.
5. Recheck material sources under the shared freshness rules and read back the
   saved agenda. If a source is inaccessible or changed, state which conclusion
   is uncertain. A successful save proves a saved draft, not publication.
6. When the person requests publication, inspect readiness and packet status.
   Sending the agenda is one step a person takes in Compass: point them to the
   meeting and say who may send it (the chair, executive director, secretary,
   board assistant or an organization administrator). If packet generation is
   pending or failed, explain that status and use a discovered retry only when
   its contract permits it.

Report the meeting and date, whether you prepared a brief, saved a draft or
kept the current agenda, the few sources that shaped it, and any missing inputs.
For an agenda proposal, include planned time against the meeting length.
Give one next step. Only the PDF files, the packet and the minutes PDF, open in
Compass; the minutes text is readable through `board.minutes.review.get`. Use a
link returned by the API or tell the member where to open it, without inventing
a download URL.
