# Lane D closure/comment drafts (main sends only after landing)

Replace PR and landing SHA placeholders with refreshed integration evidence.

## D1 — issue #3719, keep open

The outbound ordering slice landed in <D1 PR> at <landing SHA>. Legacy combined
redacted/signed thinking now has the same order in streaming and JSON responses,
including preceding reasoning deltas. This does not establish multi-turn Anthropic
replay acceptance or cache improvements; those remain open in #3719.

## D2 — release follow-up discussion_r3946496126

The bounded unknown-receipt recovery guard landed in <D2 PR> at <landing SHA>.
While the write outcome is unknown, the dialog blocks new edits/reset and keeps
read-only Retry available. Confirmed writes retain their existing edit behavior.
This is a UI recovery guard, not a global server request-ordering guarantee.

## D3 — issue #3817, close

Landed in <D3 PR> at <landing SHA>. Base-provider pricing now resolves through
exact configured Codex account identities and effective log labels, with matching
Fast/context modifiers and cache invalidation. Literal configured providers stay
isolated; aliases and arbitrary unknown suffixes are not guessed. Credit retained
for @rrmlima. Closing this OpenAI account-label pricing report.

## D4 — issue #3667, close

Landed in <D4 PR> at <landing SHA>. Models now has a manual price editor with a
persistent badge and reset-to-automatic action; `ocx models price` and
`ocx models set-price` expose the same store. Explicit zero user rates are known-zero
estimates, and existing overlays survive sync. Credit retained for @nordz0r.

## D5 — PR #2956, close; issue #3379, keep open

The custom usage-window slice was reimplemented in <D5 PR> and landed at
<landing SHA>, preserving @Manson2438's contribution credit. Inclusive start/end
bounds, existing filters and cost estimates are wired through API, CLI and dashboard.
The original PR is superseded for that slice. Offline reports and hourly chart
buckets were not included. #3379 remains open for its remaining dashboard/reporting
requirements; this comment does not claim the whole issue is resolved.
