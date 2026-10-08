# Prompt for the Grok bot

Paste this into the Grok bot. Sending this GitHub to Grok Build or to the bot means go: start the operation. This file does not lock the questions plan and does not spend. The node order is [TWO-NODES.md](TWO-NODES.md).

If this file disagrees with [NEXT-STORM-PLAN.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/NEXT-STORM-PLAN.md), stop and ask stp. The plan wins. [BOT-TPS.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/BOT-TPS.md) is rate advice from the desk pre-run. It is not this prompt.

## Goal

One combo with Grok Build, on one UTC clock, after the usage reset stp marked OK on 7 Oct 2026.

Friday 9 Oct 2026, 21:30 UTC, for 8 hours, ending Saturday 10 Oct 2026, 05:30 UTC. If that day is not ready, Monday 13 Oct 2026, 21:30 UTC, for 8 hours, ending Tuesday 14 Oct 2026, 05:30 UTC.

Kaspa Pulse counts Friday 21:25 UTC through Saturday 05:35 UTC. That is his clock. It is not T0. Do not start at 21:00 or at 21:25. The 21:00 UTC in the 8 Oct DM is not this file.

## Before any send

Stop unless all three are true:

1. This GitHub has been sent to Grok Build or to the bot. That is the storm GO. A dry-run GO is not this.
2. `steps-utc.json` is in hand. Do not invent the timetable. Box and Build use the same UTC times.
3. The clock is at or after the first time in that file.

Read free disk on this box before T0. Go only with at least 35 GB free. From 28 to 35 GB, the steps shrink to 10 minutes and that is written down as a deviation. Below 28 GB, no storm. Keep about 19 GB free for n0 pruning. A guard stop ends the run for the box and for Build.

Confirm desk node B is synced and its tip lag is at or under 300 seconds. If it is not, stop. The runner runs only during the storm. On the desk it uses Borsh `ws://127.0.0.1:17310`. From the box it uses the node B tunnel in the desk handoff, after that handoff lists one.

The box dry run is still open. If the storm GO does not name it as left open, stop and ask.

The hours from 00:25 UTC to 05:30 UTC have no named phase. If the storm GO does not name them, or does not end the storm at 00:25, stop and ask. Do not invent the names.

## This side only

- TN10 only. Network `testnet-10`.
- The Bot wallet only. Do not spend the Build wallet.
- Send through desk node B only, and only during the storm. `bore.pub` and `159.223.110.159` stay closed.
- Six runners, four connections each, for the paced steps. A seventh runner only on the max step. Never eight.
- Build's share of each paced step is 25%. This side sends the rest. The max step is uncapped for both.
- Depth 2 on a long step. Freeze the fee near the loaded quote. The pair that held on the desk was 200 and 300 sompi/gram, cap 600. Each signer uses its own coins.
- Keys stay on the box. Do not print a key, a seed, or a wallet file.

## When the first TPS starts

T0 is 21:30 UTC. B0 is the first 10 minutes. The lane runners stay off in B0, in the two settles, and in B1.

The plan keeps the fee probes and the box ordered stream on during B0. Those are not the lane load.

The first TPS step is the 2× load at **21:40 UTC**. Hold each load step for 15 minutes, then drain at 0. Do not change rate, fee, depth, or runner count inside a step.

The miners-off control is the same 2× target with the miners off. The box scheduler switches the box miners. Log the switch. Do not invent a different time.

Per-transaction logs stay on. Times are UTC with milliseconds and `Z`. Match Build's ids on desk node B. That match is this side's job.

Point the miners at desk node B. On the desk that is gRPC `127.0.0.1:16310`. Coinbase pays the Grok Bot address `kaspatest:qzffl5xy9np46gkttyuftqnv2w04pr8g3wsp7c3vv8se3txtelx6q7c0v0ldx`. Mine only while node B is synced.

The next run's monitor is [plan/NEXT-RUN-MONITOR.md](https://github.com/STP-KAS/tn10-locus/blob/main/plan/NEXT-RUN-MONITOR.md). Print one block every 10 minutes for the desk to copy: UTC, phase, session, sender count, box disk GB, NTP offset, usage or **not measured**, node B synced, node B lag seconds, node B mempool, node B CPU, submit tx/s, accepted tx/s, rejects, miner count. If node B is unsynced or lag is over 300 seconds, sender count is 0 and the block says `waiting`. A missing block stays **not measured** and fails this side's part of the pass. The runner stays off outside the storm.

## Minute log, on top of the per-second log

Every UTC minute, one local line per sender:

- minute, `YYYY-MM-DDTHH:MM:00Z`
- sender id
- node: `desk-nodeB`
- tx_sent: submissions by that sender in that minute
- five tx ids from that minute, spread across it, not the first five

Do not print the id list. The five ids stay in the local log. They do not go in git. His accepted count is his. Do not invent it.
