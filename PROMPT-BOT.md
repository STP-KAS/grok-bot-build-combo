# Prompt for the Grok bot

Paste this into the Grok bot on the box. This file does not start the storm, does not lock the plan, and does not spend.

If this file disagrees with [NEXT-STORM-PLAN.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/NEXT-STORM-PLAN.md), stop and ask stp. The plan wins. [BOT-TPS.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/BOT-TPS.md) is rate advice from the desk pre-run. It is not this prompt.

## Goal

One combo with Grok Build, on one UTC clock, after the usage reset stp marked OK on 7 Oct 2026.

Friday 9 Oct 2026, 21:30 UTC, for 8 hours, ending Saturday 10 Oct 2026, 05:30 UTC. If that day is not ready, Monday 13 Oct 2026, 21:30 UTC, for 8 hours, ending Tuesday 14 Oct 2026, 05:30 UTC.

Kaspa Pulse counts Friday 21:25 UTC through Saturday 05:35 UTC. That is his clock. It is not T0. Do not start at 21:00 or at 21:25. The 21:00 UTC in the 8 Oct DM is not this file.

## Before any send

Stop unless all three are true:

1. stp has given the storm GO. That GO is separate from any earlier dry-run GO. This file does not give it.
2. `steps-utc.json` is in hand. Do not invent the timetable. Box and Build use the same UTC times.
3. The clock is at or after the first time in that file.

Read free disk on this box before T0. Go only with at least 35 GB free. From 28 to 35 GB, the steps shrink to 10 minutes and that is written down as a deviation. Below 28 GB, no storm. Keep about 19 GB free for n0 pruning. A guard stop ends the run for the box and for Build.

Confirm n0 is synced. If n0 is unsynced, or more than 300 seconds behind, for the guard in the plan, stop.

The box dry run is still open. If the storm GO does not name it as left open, stop and ask.

The hours from 00:25 UTC to 05:30 UTC have no named phase. If the storm GO does not name them, or does not end the storm at 00:25, stop and ask. Do not invent the names.

## This side only

- TN10 only. Network `testnet-10`.
- The Bot wallet only. Do not spend the Build wallet.
- Send through n0 only. Do not send through the desk's public signers, and do not send to `bore.pub` or `159.223.110.159`.
- Six runners, four connections each, for the paced steps. A seventh runner only on the max step. Never eight.
- Build's share of each paced step is 25%. This side sends the rest. The max step is uncapped for both.
- Depth 2 on a long step. Freeze the fee near the loaded quote. The pair that held on the desk was 200 and 300 sompi/gram, cap 600. Each signer uses its own coins.
- Keys stay on the box. Do not print a key, a seed, or a wallet file. Do not print an address.

## When the first TPS starts

T0 is 21:30 UTC. B0 is the first 10 minutes. The lane runners stay off in B0, in the two settles, and in B1.

The plan keeps the fee probes and the box ordered stream on during B0. Those are not the lane load.

The first TPS step is the 2× load at **21:40 UTC**. Hold each load step for 15 minutes, then drain at 0. Do not change rate, fee, depth, or runner count inside a step.

The miners-off control is the same 2× target with the miners off. The box scheduler switches the box miners. Log the switch. Do not invent a different time.

Per-transaction logs stay on. Times are UTC with milliseconds and `Z`. Match Build's ids on n0. That match is this side's job.

## Minute log, on top of the per-second log

Every UTC minute, one local line per sender:

- minute, `YYYY-MM-DDTHH:MM:00Z`
- sender id
- node: `n0`
- tx_sent: submissions by that sender in that minute
- five tx ids from that minute, spread across it, not the first five

Do not print the id list. The five ids stay in the local log. They do not go in git. His accepted count is his. Do not invent it.
