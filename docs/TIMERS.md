# Understanding timers

[← Back to Nyerk](../README.md)

A timer is only as reliable as the information behind it. Nyerk distinguishes schedules, estimates and observations so that an old or missing value is not presented as a confirmed spawn.

## What the labels mean

| Information | What it tells you |
| --- | --- |
| Community schedule | A published event timetable. It can change with region, maintenance or game updates. |
| Manual observation / estimate | A countdown or kill time entered by the player, possibly combined with a known respawn interval. |
| Game observation | A deadline received from supported game traffic. Availability depends on the build and which map data has arrived. |
| Last observed | Previously captured information; it has not just been rechecked against the server. |
| Unknown / awaiting observation | Nyerk does not have enough evidence for a deadline. |
| Time elapsed / check map | The known deadline has passed. It does not confirm the boss is alive. |

## Public RC28

The public build includes scheduled events, server/faction context, boss pinning, manual boss observations and configurable popout reminders. Shugo and Dimensional Invasion were checked against the developer's game; Spacetime Rift was also reported as matching. Those checks are not verification of every server or future schedule.

Field bosses start their respawn timers after a kill. A fixed repeating timetable can drift and should not be treated as a live boss service. The older fixed Kaira, Nahma and Executor schedules are known to disagree with observed Abyss countdowns.

## Boss observations in the next builds

RC30–RC31 work is implemented locally and has not been included in the public RC28 download:

- Read supported boss lists and preserve the game's reported deadlines.
- Save observations locally so they return at startup.
- Match additional maps using boss-position evidence.
- Keep separate Nahma locations, with map filtering and individual pins.
- Replace the conflicting fixed Abyss boss schedules with observed countdowns.
- Preserve multi-day deadlines and show expired times without inventing a new spawn.

The existing recordings verify Verteron's feed. Altgard and additional maps, including Abyss areas, still need live acceptance. Channels are not decoded.

**Launching Nyerk cannot obtain fresh timers for every unseen map.** Saved observations can load immediately; fresh observations depend on what the game sends. A new map may require a living-boss position before its list can be identified. These limits are why the work is still being validated.

## Reporting a mismatch

Use the [timer report form](https://github.com/Zeerey/aion2-nyerk-releases/issues/new?template=timer_correction.yml). Include:

- Boss or activity name and map.
- Region, server, faction and channel if known.
- The actual date, local time and timezone when you compared them.
- Nyerk's countdown/status and the game's countdown.
- Whether the boss had recently been killed, you changed channel, or Nyerk had just started.

For example: “At 8:15 PM EDT on October 19, the game showed 1h 49m and Nyerk showed 49m.” The observation time matters: a screenshot without it cannot establish an absolute deadline.

[Roadmap](../ROADMAP.md) · [Troubleshooting](TROUBLESHOOTING.md)
