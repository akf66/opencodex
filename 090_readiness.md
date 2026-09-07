# 090 Lane D readiness

Outcome: LANDABLE under the explicit updated per-chain user policy. No merges performed.

Top CI: https://github.com/lidge-jun/opencodex/actions/runs/34120761219
Exact top: fe9460372597061f572beee6c325009fef618c42
Fresh dev: f4a4b468feb04094b90c909d82e04606caf92663
Expected cumulative merge tree = tested tree: ded24302f8f458f7f2ee5604246f032327efcdf2

Required 16 jobs are SUCCESS: Linux4, macOS2, gates, API usage, storage policy,
keyring3, npm-global3, docker. Windows6 and macOS control are explicitly excluded
from per-chain acceptance and reserved for final release-train-head verification.
Their unfinished aggregate is not misrepresented as an overall workflow success.
Remote GUI1787pass/0fail; lint0errors/0warnings, typecheck, privacy and GUI build pass.
Local suites/typecheck/build/install NOT RUN by instruction.

All five PRs ready-for-review. Latest enforce-target/hygiene/label green at each
exact head; native stack endpoint returned [] for each; unresolved non-outdated
review threads absent and no CHANGES_REQUESTED reviews at final snapshot.
Main must refresh these facts immediately before integration.

| Item | PR | Head | Review |
|---|---|---|---|
| #3719 outbound ordering slice | #3877 | c35b5a6e504a4513ad59957f5c81b7db45f8bec6 | independent Astra PASS; verdict in PR |
| #17 name receipt guard | #3902 | c5fb7e3332432c6546bffa9990bce5b971653139 | independent Astra PASS; verdict in PR |
| #3817 account pricing | #3903 | c44c6de87389a95ab798b648659fbc0838af170b | independent Astra PASS; verdict in PR |
| #3667 manual pricing | #3904 | 5669413794ca54388782f6758171a81a2d1b361e | independent Astra PASS; verdict in PR |
| #3379 range slice / #2956 | #3905 | fe9460372597061f572beee6c325009fef618c42 | independent Astra PASS; verdict in PR |

Screenshots derive from this exact top CI artifact. Source/build marker and GUI tree
d37b888016199ab7470993e24dde1c14b3296d5e verified. Synthetic in-memory API data only.
Observed name unknown-receipt lock/read-retry; price save/reopen/reset and badge;
custom range millisecond request, reversed validation and clear; desktop and narrow layout.
Temporary browser tab and localhost preview server terminated after inspection.

#3719 and #3379 remain open. #3817 and #3667 may close after actual landing.
#2956 is superseded by this credited range slice and may close with explicit residuals.
Coauthor ids: rrmlima137737127, nordz0r6949669, Manson2438 183030642; lidge-jun243035832.
A budget admission and D ordering jointly preserved; only positive fallback fixture
budgets changed to280/320KiB, production limits and original70KiB negative assertions intact.
No cross-lane hunk remains to be reapplied.
