> **Experimental. We are just trying this.**
>
> [Disclaimer](../DISCLAIMER.md)

Thank you, Kaspa Pulse (@gokugalax), for the guidance and the input over this stretch, from 4 Oct 2026 on. The 7 Oct 2026 wording stays: sign-and-send processes are senders; runner is the setup; bot is reserved for the operator.

# Plan for Thursday night

**Window.** Thursday 8 Oct 2026, **18:00:00Z to 20:00:00Z.** Both sessions stop at 20:00 UTC even if a line is unfinished.

**Goal.** Leave Friday able to be the one clean run Kaspa Pulse asked for. Friday T0 stays 21:30 UTC. This page is the checkout.

**Usage reset.** stp marked the bot and Build usage reset OK on 7 Oct 2026. The combo has not been run. These two hours are that first combo, at checkout size.

## What the two hours are

The operators stay up for the whole window and write a monitor row every 10 minutes. That is the run.

The lane senders run for one 15-minute sample, and only when both of these are true:

1. stp has said the words **rehearsal GO** during this window.
2. The clock is inside **18:30:00Z–18:45:00Z**.

A storm GO is a different sentence, for Friday, and it needs `steps-utc.json`. Those words do not arm this sample. The desk measure arm file whose first line is `fee2h` does not arm this sample either.

If rehearsal GO arrives after 18:45 UTC, skip the sample. Finish the checks. Write the skip in the Friday call.

A DM on 8 Oct that aims the pre-test at 20:00 UTC does not move this window. 20:00 UTC is the stop. His counter for tonight is 18:00–20:00 UTC. A send that starts at the stop is outside it.

## Phases

| Phase | Local | UTC | Lane senders | Work |
|---|---|---|---|---|
| Paste | 19:50 | 17:50 | off | Both prompts are in. They wait. |
| R0 arm | 20:00–20:20 | 18:00–18:20 | off | Preflight on both sides. First monitor rows. |
| R1 quiet | 20:20–20:30 | 18:20–18:30 | off | Ten quiet minutes. Pools, indexer, clocks, disk, usage. Same shape as a baseline, with probes off. |
| R2 sample | 20:30–20:45 | 18:30–18:45 | on, only with rehearsal GO | One fixed step. Cap 250 tx/s total. |
| R3 drain | 20:45–20:55 | 18:45–18:55 | off | Drain at 0. Measurements stay on. |
| R4 match | 20:55–21:20 | 18:55–19:20 | off | Bot writes matched count over sample count. Ids stay out of git. |
| R5 Friday call | 21:20–22:00 | 19:20–20:00 | off | Fill the call. Stop at 20:00 UTC. |

Monitor rows are due at 18:00, 18:10, 18:20, 18:30, 18:40, 18:50, 19:00, 19:10, 19:20, 19:30, 19:40, 19:50, and 20:00 UTC. A missed row is written as **not measured**, with the UTC it was due.

## The sample, if rehearsal GO is given

One step. Miners stay as they are. No miners-off. No seventh runner. No eighth. Probes off. Ordered stream off. No rate change inside the 15 minutes.

| Side | Target | Processes | Where |
|---|---|---|---|
| Build | 62 tx/s | 4 fixed senders | Public TN10 nodes. Paced shape: depth 2, in-flight 48, 4 connections. |
| Bot, the operator's senders | 188 tx/s | 6 runners, 4 connections each | n0 only. Depth 2. |

62 + 188 = 250. The plan's miners-off control is capped at 250 tx/s total when the low step would pass that line. This sample uses the same ceiling so the checkout stays a low step. It is one step with miners on. It is not the miners-off pair, and it is not Friday's table.

Fee frozen at **200 and 300** sompi/gram, cap **600**. Half the lanes at each tier. Recheck the public quote at 18:30 UTC. If the normal quote on the node a sender will use is already above 200, do not start. Ask stp.

Build spends the Build wallet. The bot spends the Bot wallet. Build does not send to n0, to `bore.pub`, or to `159.223.110.159`. The bot does not send through the desk's public senders.

The older fleet halt stays in place. This sample does not clear it, and it does not write a measure STOP file. The sample process exits at 18:45 UTC because its own end time says so.

## What each side owes the log

Every UTC second of the sample, one line per sender:

- sender id
- target tx/s, submitted tx/s, accepted tx/s
- the endpoint that sender posts to
- the local pool and each public pool, each named
- submit-call latency

Every UTC minute of the sample, one local line per sender, on top of the second log:

- minute, `YYYY-MM-DDTHH:MM:00Z`
- sender id
- node: Build names the public TN10 node. The bot names n0. Not the word "public".
- tx_sent: submissions by that sender in that minute
- five tx ids, spread across the minute, not the first five

On a sample of transactions, and on every reject: submit time and accept time. The ids stay in the local log and in the checkout sheet. The git line is the count.

NTP offset at 18:00 UTC and at 20:00 UTC, on the box and on the desk.

A stuck pool is named. A flat accepted rate is left unlabeled tonight. Friday uses the plan's box-bound / network-bound rule. Tonight only records the numbers.

## Friday call, written at 19:40 UTC

Fill the table in [RESULTS.md](RESULTS.md). This folder does not move Friday.

Friday stays the clean run when every line below is **pass**, or is a line stp will name in the storm GO:

| Line | Pass means |
|---|---|
| Both sessions | A 20:00 UTC stop line from the bot and from Build. |
| Usage | A number at 18:00 and at 20:00 from each side, and headroom stp accepts for 8 hours. **not measured** leaves the line open. Two hours do not prove eight. |
| Bot disk | A GB figure from the box. At least 35 GB free is the go line. 28–35 GB shrinks Friday's steps to 10 minutes and is written as a deviation. Below 28 GB, Friday waits. About 19 GB stays free for n0 pruning. The desk disk is not this figure. |
| n0 | Synced, and lag at or under 300 seconds. |
| Desk node | Synced, testnet-10, kaspad 2.1.0, UTXO index on. |
| Public names | The six names rechecked. Count machines only when the check actually separates them. |
| Sample | Skipped with a reason, or passed the rules in [MONITOR.md](MONITOR.md). |
| n0 match | Bot writes matched/total for the sample. Ids stay out of git. A skip leaves the 6 Oct match open. |
| Box dry run | A 15-minute sample is a box sample. The plan's box dry run stays its own line. |
| Halt | The older fleet halt file still says halt. |
| Arm file | `fee2h` was not used as a GO. |
| Public results | The public result sections are still empty. |
| Plan | Still unlocked. Lock SHA still blank. `steps-utc.json` still absent. Storm GO still absent. |
| Phases after 00:25 | Still unnamed. Storm GO either names them or ends the storm at 00:25. This page does not choose. |

If the bot disk is under 28 GB, or n0 is unsynced, or a session died, the call says Friday is not ready and the written fallback is Monday 13 Oct 2026, 21:30 UTC. stp decides. This file does not.

## Still true after 20:00 UTC

- Fee for the long hold stays 200 and 300 sompi/gram. Cap 600.
- Build's Friday share stays 25% on the paced steps. Four fixed senders. The long hold and the uncapped max also use the synced desk node, two signers per physical machine.
- The bot's Friday runners stay six, plus a seventh only on the max step.
- T0 Friday is 21:30 UTC. B0 is 10 minutes. Lane senders off in B0. First paced load is 21:40 UTC. The 21:00 UTC in the 8 Oct DM is not T0.
- The paced table is 2 h 55 min and ends 00:25 UTC Saturday. The storm window continues to 05:30 UTC. The hours after the table have no named phase. On 8 Oct he asked to name them or end the storm at 00:25. That choice is not made here.
- His counter, same day: tonight 18:00–20:00 UTC, and Friday 21:25 UTC through Saturday 05:35 UTC, two nodes. That is his clock. It does not move T0. Comparison comes to us first.
- Kaspa Pulse counts the chain on his side, sends the comparison first, and stays out of the setup.

Intentions are good; thought process is questionable. STP remains delusional. Si vis pacem, para bellum.
