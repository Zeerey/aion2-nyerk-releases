# Development status and roadmap

[← Back to Nyerk](README.md)

Updated October 19, 2026. This is a status guide, not a release-date commitment.

## Available publicly: RC31

[Download RC31](https://github.com/Zeerey/aion2-nyerk-releases/releases/tag/v1.0.0-rc.31)

- Character overview, saved profiles, account-wide pets and configurable layouts.
- Configurable Pets / Combat / Timers popout, pins and hourly update checks.
- Broader experimental combat coverage, verified summon attribution and kill-aware encounter timing.
- Automatic storage of the latest ten unstarred fights, protected starred encounters and per-player skill/effect timelines.
- Game-observed boss deadlines, map filtering, separate Nahma locations and persistent observations.
- In-app reporting, diagnostic recording and optional Ko-fi support.

RC31 includes the previously local RC29 and RC30 changes. It is a release candidate, not final 1.0 acceptance.

## Released features with remaining validation

| Area | Evidence and remaining proof |
| --- | --- |
| **Combat coverage and timing** | Three supplied saved boss fights match all 15 reference contributor totals and standard DPS. Other encounters, unsupported effects and missing identities can still disagree. Outdoor comparison-meter parity is not established. |
| **Saved encounters** | Automated save, rotation, starring, recovery and detail checks passed. Continued live-use testing remains valuable. |
| **Verteron boss deadlines** | A production-path recording replay verifies 31 lists, all 24 bosses, exact captured deadlines and an alive-to-respawn transition. |
| **Altgard and additional maps** | Structural and synthetic tests passed. Live acceptance is still pending, including Abyss map IDs, slot ordering and countdowns. |
| **Persistent timers** | Restart recovery, server isolation, expiry, multi-day deadlines and corrupt-cache protection are tested. Saved observations are not fresh server checks. |

## Next priorities

1. **Combat confidence:** continue checking damage, timing, player identity and summon attribution against well-described encounters.
2. **Boss timer accuracy:** capture Abyss and other map lists and compare decoded deadlines with the game.
3. **Windows distribution:** improve publisher signing and release delivery while preserving update integrity and clear security reporting.
4. **Usability:** refine layouts, readability, popout behavior and the feedback workflow.

Fresh timer data for every map at game launch is not established. Nyerk restores saved observations, but new data depends on what the game sends. Channels are not decoded. An unseen map with no living boss may remain unidentified until sufficient position evidence arrives.

[Suggest a feature](https://github.com/Zeerey/aion2-nyerk-releases/issues/new?template=feature_request.yml) · [Report a bug](https://github.com/Zeerey/aion2-nyerk-releases/issues/new?template=bug_report.yml)
