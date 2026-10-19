# What Nyerk does

[← Back to Nyerk](../README.md)

This guide describes the public RC31 feature set. Validation limits and next priorities are listed in the [roadmap](../ROADMAP.md).

## Account overview and characters

See saved character information together: class and level, item level, combat power, Odyle Energy, Ascension and Nightmare. The overview offers cards, a compact roster and a four-card carousel. Character details and available public-profile imagery help distinguish your characters.

Nyerk fills supported fields from observations and public-profile information. It does not invent missing values. A saved character or estimated balance is not necessarily current; pay attention to status and estimate labels.

## Account-wide pet collection

Track collection totals, search known pets and follow progression. Pet collection is shared across characters in this installation's single-account setup; observing a pickup does not require a character to be identified first.

The small pet strip follows the most recently acquired pet and shows its name and progress. If an older save has no acquisition history, it may wait for the next pickup. Missing or unavailable images use a fallback.

## Experimental combat tracking

The Combat page shows counted damage, encounter-average DPS, contributors, targets and skill details. The popout ranks identified contributors by DPS, with damage bars, totals and shares. Supported summons are attributed to verified owners; unresolved sources remain visible without being mislabeled as extra party members.

Completed encounter DPS uses the first-to-last counted outgoing-hit window, including the time between attacks. All contributors use the same encounter duration. A selected target uses its own shared first-to-last hit window, while the popout continues showing the full encounter. Confirmed kills finish a fight once all engaged opponents are defeated; otherwise an inactivity fallback applies. It is not buff-adjusted rDPS, peak DPS, or a sum of per-skill active times.

Nyerk does not yet decode every effect, identity or party relationship. A ranking of identified attackers is not an authoritative party roster. Missing packets, late startup, unsupported effects or a partial encounter can produce disagreement with another meter.

### Saved encounters and fight review

Combat keeps the latest **ten unstarred encounters** automatically, deleting the oldest unstarred fight as room is needed. **Star an encounter** to protect it from rotation. Saved fights survive restarts; interrupted fights can recover from periodic checkpoints with a partial-data label.

Open a saved fight and select a contributor to inspect skills and observed buff, debuff and renewal intervals for the full encounter or a selected time range. Missing effect observations remain unknown; these timelines do not calculate buff-adjusted rDPS. Detailed hit and effect timelines have safety limits, with aggregate damage retained if a timeline is capped. Diagnostic packet recording remains under Network.

## Events, bosses and reminders

View relevant activities using character/server context or a manual selection. Event icons distinguish activity types, countdowns help prioritize upcoming events, and bosses can be pinned. Select which reminders appear in the companion popout.

Shugo, Dimensional Invasion, Spacetime Rift, Abyss activities and reset information have different evidence and timing rules. Supported boss lists supply game-reported deadlines, which are saved locally and restored as last-observed information. Separate Nahma sites and a map filter help distinguish locations. Conflicting fixed Kaira, Nahma and Executor schedules have been removed; those bosses await observations or manual countdowns. A schedule, saved observation or manual estimate is not a continuously refreshed live server feed. [Read the timer guide](TIMERS.md) before relying on a boss countdown.

## A configurable companion popout

Choose Pets, Combat and Timers independently. The pet summary stays compact, event icons provide hover details, and the DPS area expands only as it needs rows. Opacity, locking and visibility controls make it easier to fit around your game interface.

Configured upcoming-event alerts glow in the ten-minute lead-up where a usable deadline is available. An unknown timer cannot provide a reliable countdown alert.

## Network diagnostics

The Network page provides capture status and diagnostic recording tools. Record a focused test, add notes about what happened, and open the recording location afterward. This helps investigate unsupported packets, combat differences and missing data.

Recordings can contain private game/network information. They are not suitable for public GitHub attachments. [Reporting guidance](../SUPPORT.md) explains what to share instead.

## Updates and feedback

Nyerk checks for compatible releases hourly and at startup. You choose when to download and restart. The main window and popout share the update indicator.

**Report a bug** opens a reviewable application summary, then GitHub so you can describe and submit the issue. The donation banner opens [Ko-fi](https://ko-fi.com/zeerey); donations are optional.
