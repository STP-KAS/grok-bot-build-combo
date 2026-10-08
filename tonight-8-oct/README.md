> **Experimental. We are just trying this.**
>
> [Disclaimer](../DISCLAIMER.md)

Wording, Kaspa Pulse (@gokugalax), 7 Oct 2026: sign-and-send processes are senders; runner is the setup; bot is reserved for the operator.

# Thursday 8 Oct 2026, 20:00 local

Two hours. 20:00–22:00 local, CEST (UTC+2), which is **18:00–20:00 UTC**.

The storm stays **Friday 9 Oct 2026, 21:30 UTC, for 8 hours**, ending Saturday 10 Oct 2026, 05:30 UTC. If Friday is not ready, Monday 13 Oct 2026, 21:30 UTC, for 8 hours. This folder does not give the storm GO, does not lock the plan, and does not start a sender.

The measurement plan is [NEXT-STORM-PLAN.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/NEXT-STORM-PLAN.md). If this folder and that plan disagree, the plan wins.

## Why these two hours exist

Kaspa Pulse asked for one clean run first, then the numbers, then weekly repeats. Friday is that clean run. These two hours are the checkout that makes Friday able to be that run: both operators stay up after the usage reset, the monitor writes the fields he asked for, and every open gate is either closed or named.

A multi-hour send tonight would be a second run stacked in front of Friday. The chain sample inside this window is 15 minutes, and only after stp says **rehearsal GO**.

## Files

| Read | When |
|---|---|
| [PLAN.md](PLAN.md) | The clock, the phases, and the Friday call. |
| [PROMPT-BUILD.md](PROMPT-BUILD.md) | Paste into Grok Build on the desk at 19:50 local. |
| [PROMPT-BOT.md](PROMPT-BOT.md) | Paste into the Grok bot on the box at 19:50 local. |
| [MONITOR.md](MONITOR.md) | What is watched, who writes it, and what passes. |
| [PULSE.md](PULSE.md) | Kaspa Pulse's input, and the blank line for a later note from him. |
| [RESULTS.md](RESULTS.md) | The monitor. The morning reading from this session is filled in. The evening rows wait for 18:00 UTC. |

The Friday paste-ins stay [PROMPT-BUILD.md](../PROMPT-BUILD.md) and [PROMPT-BOT.md](../PROMPT-BOT.md) at the repo root. Those files wait for a storm GO and for `steps-utc.json`. They are the wrong paste for tonight.

## At 19:50 local

1. Paste [PROMPT-BOT.md](PROMPT-BOT.md) into the bot.
2. Paste [PROMPT-BUILD.md](PROMPT-BUILD.md) into Grok Build.
3. Both wait until 18:00 UTC.
4. Say **rehearsal GO** only if the 15-minute sample should run. Silence means the two hours are checks and monitor rows, with the lane senders off.
5. At 22:00 local, read the Friday call at the bottom of [RESULTS.md](RESULTS.md).

Intentions are good; thought process is questionable. STP remains delusional. Si vis pacem, para bellum.
