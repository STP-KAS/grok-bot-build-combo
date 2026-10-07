# Prompt for Grok Build

Paste this into Grok Build on the desk. This file does not start the storm, does not lock the plan, and does not spend.

If this file disagrees with [NEXT-STORM-PLAN.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/NEXT-STORM-PLAN.md), stop and ask stp. The plan wins. The longer desk paste-in is [GROK-BUILD-PROMPT.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/GROK-BUILD-PROMPT.md). The run, once the storm GO and `steps-utc.json` exist, is [TESTDAY.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/TESTDAY.md).

## Goal

One combo with the Grok bot, on one UTC clock, after the usage reset stp marked OK on 7 Oct 2026.

Friday 9 Oct 2026, 21:30 UTC, for 8 hours, ending Saturday 10 Oct 2026, 05:30 UTC. If that day is not ready, Monday 13 Oct 2026, 21:30 UTC, for 8 hours, ending Tuesday 14 Oct 2026, 05:30 UTC.

## Before any send

Stop unless all three are true:

1. stp has given the storm GO. That GO is separate from the dry-run GO. This file does not give it.
2. `steps-utc.json` is in hand. Do not invent the timetable.
3. The clock is at or after the first time in that file.

The n0 match, the box dry run, and 35 GB free on the bot disk are still open. If the storm GO does not name any of those it is leaving open, stop and ask.

## This side only

- TN10 only. Network `testnet-10`.
- The Build wallet only. Do not spend the Bot wallet.
- Paced steps: public TN10 nodes. Four fixed processes. Depth 2. In-flight 48. Four connections. No auto-scale. No mempool pause inside a step.
- Long hold and the uncapped max: two signers on each physical machine, depth 2, in-flight 64, fee frozen at 200 and 300 sompi/gram, cap 600, plus the synced desk node on its own coins.
- Never send to n0, to `bore.pub`, or to `159.223.110.159`.
- Leave the 3 Oct halt on the older fleet in place.
- Keys stay on the desk. Do not print a key, a seed, or a wallet file.

## When the first TPS starts

T0 is 21:30 UTC. B0 is the first 10 minutes. Send nothing in B0, in the two settles, or in B1. No lanes and no ordered stream.

The first TPS step is the 2× load at **21:40 UTC**. Hold each load step for 15 minutes, then drain at 0. Do not change rate, fee, depth, or process count inside a step.

Log the desk miner count at each phase start. Do not switch the miners. stp does that.

Per-transaction logs stay on. Times are UTC with milliseconds and `Z`.
