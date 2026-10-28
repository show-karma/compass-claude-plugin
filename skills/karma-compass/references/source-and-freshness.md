# Source and freshness rules

## Source hierarchy

Use the most authoritative current source available:

1. API-returned meeting, agenda, quorum, roster, vote, and action state.
2. Current immutable versions of governing documents and board records returned through citation search.
3. Current packet and source attachments with document identifiers and versions.
4. Organization preferences and Prospecting Memory, explicitly labeled as learned working context.
5. Inference, explicitly labeled and never used to assert authority.

Do not use general web search for organization-specific governance facts.

## Provenance labels

Keep enough provenance to explain every material agenda choice:

- meeting and agenda identifiers and versions;
- document identifier, immutable version, page or section, and span when returned;
- submission identifier and status;
- action-item identifier and state;
- prior meeting identifier for carried-forward work;
- the time this run observed the source, when the tool provides it.

Do not expose opaque identifiers gratuitously in prose. They remain available for audit and exact tool calls; use human-readable labels in the member summary.

## Freshness gate

Before reporting completion or requesting review, re-read the meeting workspace, agenda workspace, readiness, context, prior records, submissions, and attachments. A no-op requires this second sweep just as a saved draft does. Regenerate or stop when any of these changed materially:

- agenda version;
- meeting time, duration, or lifecycle state;
- source or packet document version;
- required decision or missing-input inventory;
- quorum projection or rule availability;
- trusted access revision.

The durable review proposal does not by itself prove that the reasoning sources stayed current, so the skill must run this separate freshness gate. Repeat every governance citation that shaped either a saved draft or a no-op result. For a no-op, preserve the existing agenda only when the second sweep confirms the same agenda id and version and still yields no material evidence-backed change.
