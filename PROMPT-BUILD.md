# Prompt for Grok Build

Paste this into Grok Build on the desk. Sending this GitHub to Grok Build or to the bot means go: start the operation. This file does not lock the questions plan and does not spend. The node order is [TWO-NODES.md](TWO-NODES.md).

If this file disagrees with [NEXT-STORM-PLAN.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/NEXT-STORM-PLAN.md), stop and ask stp. The plan wins. The longer desk paste-in is [GROK-BUILD-PROMPT.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/GROK-BUILD-PROMPT.md). The run, once the storm GO and `steps-utc.json` exist, is [TESTDAY.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/TESTDAY.md).

## Which file is the Friday paste

This file is the paste until stp says otherwise.

After the 8 Oct checkout, Build writes [plan/GROK-BUILD-PROMPT-AFTER-8-OCT.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/GROK-BUILD-PROMPT-AFTER-8-OCT.md) from the checkout result and from Kaspa Pulse's input. Do not use that file while it still says it is not written yet. Do not use it at all unless stp has said it replaces this file. The checkout note is [plan/AFTER-8-OCT.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/AFTER-8-OCT.md).

## Goal

One combo with the Grok bot, on one UTC clock, after the usage reset stp marked OK on 7 Oct 2026.

Friday 9 Oct 2026, 21:30 UTC, for 8 hours, ending Saturday 10 Oct 2026, 05:30 UTC. If that day is not ready, Monday 13 Oct 2026, 21:30 UTC, for 8 hours, ending Tuesday 14 Oct 2026, 05:30 UTC.

## His counter is not our T0

Kaspa Pulse, 8 Oct 2026, after the checkout PDF. The 9th works on his side. He counts Friday **21:25 UTC** through Saturday 10 Oct 2026 **05:35 UTC**, two nodes, a few minutes either side of our window. Our T0 stays **21:30 UTC**. The first TPS step stays **21:40 UTC**. Our end stays **05:30 UTC**.

The **21:00 UTC** in stp's DM that morning is not T0. Do not start at 21:00. Do not start at 21:25.

7 Oct is closed. Last submit 18:38:39 UTC. His window started 18:53. He counted the chain after the run. No conflict. Do not explain it. Do not call a figure a ceiling.

Comparison comes to us first. Do not send him this run from the paste. Do not ping him.

## Update the checkout PDF you made from this git

If you are the session that made the checkout PDF from https://github.com/STP-KAS/grok-bot-build-combo , update that same PDF from current main before any send. Do not make a second PDF. Do not change the layout. Do not send it to him.

Write only the 8 Oct changes: his counter beside our clock, the minute line with the id cells still empty, 7 Oct closed, and the hours after 00:25 left unnamed until stp chooses. No key, no seed, no address, no txid.

## Before any send

Stop unless all three are true:

1. This GitHub has been sent to Grok Build or to the bot. That is the storm GO. A dry-run GO is not this.
2. `steps-utc.json` is in hand. Do not invent the timetable.
3. The clock is at or after the first time in that file.

The n0 match, the box dry run, and 35 GB free on the bot disk are still open. If the storm GO does not name any of those it is leaving open, stop and ask.

The hours from 00:25 UTC to 05:30 UTC have no named phase. He asked to name them (long hold, max, drain) or to end the storm at 00:25. This file does not choose. If the storm GO does not choose, stop and ask before any send. Do not write names for those hours. Do not end the storm at 00:25 on your own.

## This side only

- TN10 only. Network `testnet-10`.
- The Build wallet only. Do not spend the Bot wallet.
- Every step goes to locus, the first desk kaspad, on loopback Borsh. Four fixed processes. Depth 2. In-flight 48. Four connections. No auto-scale. No mempool pause inside a step.
- Long hold and the uncapped max stay on locus: depth 2, in-flight 64, fee frozen at 200 and 300 sompi/gram, cap 600.
- `bore.pub` and `159.223.110.159` stay closed. Leave the 3 Oct halt on the older fleet in place.
- Keys stay on the desk. Do not print a key, a seed, or a wallet file.

## When the first TPS starts

T0 is 21:30 UTC. B0 is the first 10 minutes. Send nothing in B0, in the two settles, or in B1. No lanes and no ordered stream.

The first TPS step is the 2× load at **21:40 UTC**. Hold each load step for 15 minutes, then drain at 0. Do not change rate, fee, depth, or process count inside a step.

Point the miners at desk node B. On the desk that is gRPC `127.0.0.1:16310`. Coinbase pays the Grok Bot address `kaspatest:qzffl5xy9np46gkttyuftqnv2w04pr8g3wsp7c3vv8se3txtelx6q7c0v0ldx`. Mine only while node B is synced. Log the count at each phase start. The bot's runner uses that same node and runs only during the storm. Build keeps sending on locus.

Per-transaction logs stay on. Times are UTC with milliseconds and `Z`. The 8 Oct high-rate rounds turned that log off. This run does not.

The next run's monitor is [plan/NEXT-RUN-MONITOR.md](https://github.com/STP-KAS/tn10-locus/blob/main/plan/NEXT-RUN-MONITOR.md). Do every Build line on that page. The 10-minute row still goes to `tonight-8-oct/RESULTS.md` until the storm sheet exists, and it includes desk disk, NTP, usage or **not measured**, submit tx/s, accepted tx/s, the six public mempools by name, locus mempool, indexer health, free RAM, and the miner count. Per minute the node cell is `locus`. Five tx ids stay in the local log. A blank required line is **not measured** and fails the pass. His accepted count is his.

## Minute log, on top of the per-second log

Every UTC minute, one local line per sender:

- minute, `YYYY-MM-DDTHH:MM:00Z`
- sender id
- node: the public TN10 name, or the desk node on the long hold and the uncapped max. Not the word "public". Not n0. This side never posts to n0. Mempool is per node.
- tx_sent: how many transactions that sender submitted in that minute
- five tx ids from that minute, spread across it, not the first five. Five is the reading of "a handful". He checks them on chain one by one.

His accepted count is his. Do not invent it. Our accepted figure stays in the per-second log.

Do not print the id list. The five ids stay in the local log and in the checkout PDF if the desk already writes one. If it does not, write a local `checkout-minute.csv` with those columns. They do not go in git.
