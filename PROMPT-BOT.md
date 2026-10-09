# Prompt for the Grok bot

Paste this into the Grok bot. Sending this GitHub to Grok Build or to the bot means go: start the operation. This file does not lock the questions plan and does not spend. The node order is [TWO-NODES.md](TWO-NODES.md).

If this file disagrees with [NEXT-STORM-PLAN.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/NEXT-STORM-PLAN.md) on a clock, a fee, or a question, stop and ask stp. The plan wins. If they disagree on the node, [TWO-NODES.md](TWO-NODES.md) wins. [BOT-TPS.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/BOT-TPS.md) is rate advice from the desk pre-run. It is not this prompt.

## Goal

One combo with Grok Build, on one UTC clock, after the usage reset stp marked OK on 7 Oct 2026.

Friday 9 Oct 2026, 21:30 UTC, for 8 hours, ending Saturday 10 Oct 2026, 05:30 UTC. If that day is not ready, Monday 13 Oct 2026, 21:30 UTC, for 8 hours, ending Tuesday 14 Oct 2026, 05:30 UTC.

Kaspa Pulse counts Friday 21:25 UTC through Saturday 05:35 UTC. That is his clock. It is not T0. Do not start at 21:00 or at 21:25. The 21:00 UTC in the 8 Oct DM is not this file.

## Before any send

Stop unless all three are true:

1. This GitHub has been sent to Grok Build or to the bot. That is the storm GO. A dry-run GO is not this.
2. `steps-utc.json` is in hand. Do not invent the timetable. Box and Build use the same UTC times.
3. The clock is at or after the first time in that file.

Read free disk on this box before T0. Go only with at least 35 GB free. From 28 to 35 GB, the steps shrink to 10 minutes and that is written down as a deviation. Below 28 GB, this side does not send. n0 will not run, so do not keep disk aside for n0 pruning. A short box disk stops this side and does not stop Build.

n0 will not run. Do not start it and do not resync it. This side's runner and this side's miners use the tunnel to **keel**, the second desk kaspad. Build uses locus. keel was still in block download at 2026-10-09T07:59:26Z (69%, not synced). It stays in the score. While it is unsynced, or the handoff has no tunnel, or tip lag is over 300 seconds, sender count stays 0 and the row says `waiting`. Check again on the next 10-minute row. Do not invent a tunnel host. From this box, do not use `127.0.0.1`. The desk sockets `ws://127.0.0.1:17310` and `127.0.0.1:16310` are keel's own ports. They are not this box's addresses.

The box dry run is still open. If the storm GO does not name it as left open, stop and ask.

The hours from 00:25 UTC to 05:30 UTC have no named phase. If the storm GO does not name them, or does not end the storm at 00:25, stop and ask. Do not invent the names.

## This side only

- TN10 only. Network `testnet-10`.
- The Bot wallet only. Do not spend the Build wallet.
- Send through keel only, through the tunnel, and only during the storm. `bore.pub` and `159.223.110.159` stay closed. n0 stays off.
- Six runners, four connections each, for the paced steps. A seventh runner only on the max step. Never eight.
- Build's share of each paced step is 25%. This side sends the rest. The max step is uncapped for both.
- Depth 2 on a long step. Freeze the fee near the loaded quote. The pair that held on the desk was 200 and 300 sompi/gram, cap 600. Each signer uses its own coins.
- Keys stay on the box. Do not print a key, a seed, or a wallet file.

## When the first TPS starts

T0 is 21:30 UTC. B0 is the first 10 minutes. The lane runners stay off in B0, in the two settles, and in B1.

The plan keeps the fee probes and the box ordered stream on during B0. Those are not the lane load.

The first TPS step is the 2× load at **21:40 UTC**. Hold each load step for 15 minutes, then drain at 0. Do not change rate, fee, depth, or runner count inside a step.

The miners-off control is the same 2× target with the miners off. The box scheduler switches the box miners. Log the switch. Do not invent a different time.

Per-transaction logs stay on. Times are UTC with milliseconds and `Z`. Match this side's own ids on keel. Build matches its own ids on locus. A waiting minute has no match to owe.

Point this side's miners at keel through the same tunnel, gRPC host and port from the handoff. Coinbase pays the Grok Bot address `kaspatest:qzffl5xy9np46gkttyuftqnv2w04pr8g3wsp7c3vv8se3txtelx6q7c0v0ldx`. Mine only while keel is synced and the handoff lists the tunnel. Until then the miners stay off. Do not point them at n0.

The next run's monitor is [plan/NEXT-RUN-MONITOR.md](https://github.com/STP-KAS/tn10-locus/blob/main/plan/NEXT-RUN-MONITOR.md). Print one block every 10 minutes for the desk to copy: UTC, phase, session, sender count, box disk GB, NTP offset, usage or **not measured**, keel synced, keel lag seconds, keel mempool, keel CPU, submit tx/s, accepted tx/s, rejects, miner count. If keel is unsynced, the tunnel is missing, or lag is over 300 seconds, sender count is 0 and the block says `waiting`. A missing block stays **not measured** and fails this side's part of the pass. The runner stays off outside the storm.

## Minute log, on top of the per-second log

Every UTC minute, one local line per sender:

- minute, `YYYY-MM-DDTHH:MM:00Z`
- sender id
- node: `keel`
- tx_sent: submissions by that sender in that minute
- five tx ids from that minute, spread across it, not the first five

Do not print the id list. The five ids stay in the local log. They do not go in git. His accepted count is his. Do not invent it.
