# Development status and roadmap

[← Back to Nyerk](README.md)

Updated October 19, 2026. This is a status guide, not a release-date commitment.

## Available publicly: RC28

[Download RC28](https://github.com/Zeerey/aion2-nyerk-releases/releases/tag/v1.0.0-rc.28)

- Character overview, saved profiles, collection tracking and configurable layouts.
- Account-wide pet progress and latest-acquired pet display.
- Configurable Pets / Combat / Timers popout and hourly update checks.
- Scheduled activities, manual boss tracking, pins and alerts.
- Experimental combat with improved summon ownership, contributor display and encounter timing.
- In-app reporting, diagnostic recording and optional Ko-fi support.

Combat decoding and several timer assumptions remain work in progress. RC28 is a test release, not final 1.0 acceptance.

## Implemented locally, awaiting public release and further acceptance

These changes are **not included in the public RC28 ZIP**.

| Work | Status / remaining proof |
| --- | --- |
| **RC29: broader skill coverage and encounter-end timing** | Recording comparisons and automated checks passed. Broader live coverage is still being tested. |
| **RC30: saved encounters and deeper review** | Latest ten unstarred fights, protected starred fights, contributor skill details and observed effect intervals are implemented locally. Live acceptance remains part of testing. |
| **RC30–RC31: game-observed boss deadlines** | Verteron recordings verify the decoded deadlines. Other maps still need live acceptance. |
| **RC31: persistent map timers and Abyss expansion** | Local build saves deadlines, restores them at launch, separates Nahma sites and removes conflicting fixed Abyss boss schedules. A fresh Abyss capture is still needed. |

RC31 was installed and validated locally. It has not been published to this downloads repository.

## Next priorities

1. **Combat confidence:** continue checking damage, timing, player identity and summon attribution against well-described encounters.
2. **Boss timer accuracy:** verify additional maps and compare decoded deadlines with the game. Distinguish stale observations from current data.
3. **Windows distribution:** improve publisher signing and release delivery while preserving update integrity and clear security reporting.
4. **Usability:** refine layouts, readability, popout behavior and the feedback workflow.

Fresh timer data for every map at game launch is not established. Nyerk can restore saved observations, but new data depends on what the game sends. No release date or universal boss coverage is promised.

[Suggest a feature](https://github.com/Zeerey/aion2-nyerk-releases/issues/new?template=feature_request.yml) · [Report a bug](https://github.com/Zeerey/aion2-nyerk-releases/issues/new?template=bug_report.yml)
