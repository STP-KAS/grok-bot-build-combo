> **Experimental. We are just trying this.**
>
> [Disclaimer](../DISCLAIMER.md)

Wording, Kaspa Pulse (@gokugalax), 7 Oct 2026: sign-and-send processes are senders; runner is the setup; bot is reserved for the operator.

# Monitor plan

This page lists the monitor demands already written in [grok-bot-build-combo](https://github.com/STP-KAS/grok-bot-build-combo) and [tn10-storm-throughput-questions](https://github.com/STP-KAS/tn10-storm-throughput-questions). It does not add a demand. It does not lock the plan. It does not ping Kaspa Pulse. Comparison comes to us first. Ids, keys, seeds, and addresses stay out of git.

If this page and [NEXT-STORM-PLAN.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/1335faffbfb5407d7eda665d60203f455813a933/plan/NEXT-STORM-PLAN.md) disagree, the plan wins.

## Where each demand already sits

| Demand set | On GitHub | Commit |
|---|---|---|
| His five questions, six method points, four tightenings, cadence, 7 Oct compare, 8 Oct clocks and three fields | [tonight-8-oct/PULSE.md](PULSE.md) | `cb960744524f17dd88b0e7f22f2c6c7bb049690d` |
| Ten-minute rows, sample second log, sample minute log, pass rules | [tonight-8-oct/MONITOR.md](MONITOR.md) | same |
| Thursday phases, rehearsal GO, Friday call | [tonight-8-oct/PLAN.md](PLAN.md) | same |
| Friday measurement rules §1 through §8 | [plan/NEXT-STORM-PLAN.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/1335faffbfb5407d7eda665d60203f455813a933/plan/NEXT-STORM-PLAN.md) | `1335faffbfb5407d7eda665d60203f455813a933` |
| 7 Oct window reading | [plan/PULSE-WINDOW-7-OCT.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/1335faffbfb5407d7eda665d60203f455813a933/plan/PULSE-WINDOW-7-OCT.md) | same |

The desk clone of the questions repo is `2c5235b23d4fdd9a814af4703fafdef01165d3e1`, five commits ahead of that GitHub commit. Those five commits are not pushed by this page. `plan/PULSE-README.md` is in the desk clone and is the same list as [PULSE.md](PULSE.md). It is not on `origin/main` yet.

The public README result sections stay empty until the clean run. Build's pre-test readings go in [RESULTS.md](RESULTS.md) in this private repo.

## Two clocks

| Clock | Written window | What it is |
|---|---|---|
| Thursday checkout | 8 Oct 2026, 18:00–20:00 UTC. Stop at 20:00 UTC. | The soft run. Monitor rows the whole window. Lane senders only inside 18:30–18:45 UTC, and only after the words rehearsal GO. |
| His counter, tonight | Same 18:00–20:00 UTC. | He counts the chain. Two nodes. |
| Friday, our T0 | 9 Oct 2026, 21:30 UTC, for 8 hours, end 10 Oct 2026, 05:30 UTC. Else 13 Oct 2026, 21:30 UTC, for 8 hours. | The one clean run. First lane load at 21:40 UTC. |
| His counter, Friday | 9 Oct 2026, 21:25 UTC through 10 Oct 2026, 05:35 UTC. | Five minutes either side of our window. |
| Paced table | T0+175, which is 00:25 UTC the next day. | 2 h 55 min. The hours after 00:25 stay inside the 8-hour window and have no named phase until the storm GO names them or ends the storm at 00:25. |
| DM aims | 20:00 UTC tonight, 21:00 UTC Friday. | Not these clocks. 20:00 UTC tonight is the stop. |

One clean run first. Go through the numbers. Then weekly. Do not stack a second storm in front of Friday. Ping him after the 9 Oct or 13 Oct run. Tonight does not ping him and does not send him the sheet.

## What he is measuring

Source: [PULSE.md](PULSE.md). The plan section is named beside each line.

| # | Demand | Plan | Thursday checkout | This desk's pre-test |
|---|---|---|---|---|
| 1 | Accepted tx/s against submitted, over the whole storm, and where acceptance flattens. | §3c, §4 | Sample second log, two columns. His accepted figure is his. | Submit is in the sender logs. Chain-accepted on his side is not measured here. |
| 2 | Confirmation time at each load step, median and worst, normal fee against 1.5×. Does paying 1.5× buy inclusion. | §4, §5 | Tonight's sample freezes 200 and 300, half the lanes each, probes off. | pre8 and s7 froze 200 and 300. k3 froze 100 and 150. Confirmation times are not measured. |
| 3 | Indexer freeze: at what sustained tx/s, and for how long. | §6 | api-tn10 health on the monitor row. | One health read at 18:14 UTC. Not the 30-second series. |
| 4 | Mempool depth over time. Backlog, not only throughput. | §6 | Each named pool on the row. n0 from the bot. | Desk-node mempool during k3 was not sampled. |
| 5 | Whether order holds under load. Sent order against accepted order. Headline tx/s is not the metric. | §4a | Ordered stream off for the Thursday sample. | Ordered stream off. Not measured. |

The two headlines are order under load, and whether 1.5× fee buys inclusion while 1× waits.

## How he asked for the run to be built

| # | Demand | Where it is carried |
|---|---|---|
| 1 | Write the plan first. Publish it with the results. Cite the commit SHA. List deviations. | Plan §1. This page cites `1335faf`. Deviations for the pre-test are in [RESULTS.md](RESULTS.md). The lock SHA is still blank. |
| 2 | Baseline first. Ten minutes of normal traffic, same measurements, then the steps. | Plan §2, B0 and B1. Thursday R1 is ten quiet minutes, probes off. |
| 3 | Fixed steps, not one blast. His example was 1×, 2×, 5×, 10×. The plan's table is a 10-minute baseline, then 2×, 5×, 10×, 20×, 30×, then max. The plan wins on that table. | Plan §3. Thursday is one 15-minute step under a 250 tx/s cap. |
| 4 | Log submitted and accepted per second, UTC. Log send order against accept order. | Plan §4 and §4a. Thursday sample second log. |
| 5 | State mining share up front. Storm 2 measured about 50–63% of TN10 blocks. He had put the share near 60% of TN10 hashrate. The result says which figure it uses. It is TN10 with our miners on. | Plan §7. |
| 6 | Raw data next to the summary. | Plan §8. Thursday sheet is [RESULTS.md](RESULTS.md). The storm CSVs stay in the questions repo after the clean run. |

## Four tightenings, before the lock

| # | Demand | Plan rule used on Friday |
|---|---|---|
| 1 | Miners-off is in the main run, at low load, matched to the same load with miners on. The control is imperfect. Other miners still change templates. Say that next to the pair. | §3b. If 2× of baseline B would pass 250 tx/s total, both halves run at 250 tx/s total, and that is recorded. Thursday leaves miners as they are. No miners-off tonight. |
| 2 | Separate the box from the chain. When accepted flattens, log n0 CPU, mempool-cap hits, and reject reasons. Label the plateau box-bound or network-bound, or leave it unclear. | §6a. n0 as read on 5 Oct: kaspad 2.1.0, `--ram-scale=0.1`, mempool cap 100,000 transactions. Thursday records the numbers and leaves a flat accepted rate unlabeled. |
| 3 | Sync the clocks. NTP on the box and on the desk. Log the offset at the start and at the end. Correct confirmation times, or flag them. | §4. Desk: `w32tm /query /status` and `w32tm /stripchart /computer:time.windows.com /samples:5 /dataonly`, at 18:00 and at 20:00 UTC tonight, and at T0 and at the end on Friday. If the desk offset moves by more than 50 ms between the two reads, flag Build's confirmation times. |
| 4 | Saturation defined before T0: accepted under 95% of submitted for 60 seconds. Reorder rates as counts and percentages, with n. About 90 probes per tier is thin. The plan raised that to about 450 per tier per step. | §3c and §5. See the two 95% rules below. |

## Two different 95% rules

Keep them apart. [MONITOR.md](MONITOR.md) and the questions README already do.

| Rule | What it measures | Source |
|---|---|---|
| Build gate | Mean achieved send rate at least 95% of the target, with no zero seconds. | Plan §3a. Thursday targets are 62 tx/s on this desk and 188 tx/s on the bot. |
| Saturation | From 60 seconds after the step start: our accepted count over a 60-second window stays under 95% of our submit-OK for 60 consecutive seconds. That second is the onset. | Plan §3c. Accepted there is our transactions on n0's virtual chain, by accept time. |
| Sender-limited | Submit-OK stays below 95% of target. Report it separately from "the network stopped accepting". | Plan §3a. |

About 450 probes per tier per step is the plan's probe count (§5: one small transaction per tier every 2 seconds, tiers 1×, 1.2×, 1.5×, 2×). Thursday's sample has probes off.

## 8 Oct fields, on top of the second log

Source: the later note in [PULSE.md](PULSE.md). They do not replace the second log. His column is accepted. Ours is sent.

| Field | Rule |
|---|---|
| tx sent | Per minute, per sender, how many transactions that sender submitted. |
| node | The node that sender posted to, by name. Bot senders: n0. Build senders: a named public TN10 node. Mempool is per node. The word "public" is not a node name. |
| five tx ids | Spread across the minute, not the first five. He checks them on chain one by one. Local log only. Git gets the count. |

## Thursday sheet, every 10 minutes

Due at 18:00, 18:10, 18:20, 18:30, 18:40, 18:50, 19:00, 19:10, 19:20, 19:30, 19:40, 19:50, and 20:00 UTC. A missed row is **not measured**, with the UTC it was due. A number that was not read is **not measured**.

| Field | Bot, on the box | Build, on the desk |
|---|---|---|
| UTC | the row time | the row time |
| Session | up or down | up or down |
| Sender count | lane runners | Build senders |
| Disk free | box GB | desk GB, labeled desk |
| Clock | NTP offset, two public servers | `w32tm`, 5 samples |
| Usage | product counter, or not measured | product counter, or not measured |
| n0 | synced, lag seconds, mempool, CPU when a sample is on | not read from the desk |
| Pools | n0 mempool | six public names, each named, plus the desk node |
| Indexer | HTTP, `isSynced`, `acceptedTxBlockTimeDiff`, `blueScoreDiff` | same check if the bot row is missing |
| Rates | submitted tx/s and accepted tx/s | submitted tx/s and accepted tx/s |
| Miners | count, on or off | count, on or off, no switch |

Lane rates are 0 on every row outside 18:30–18:45 UTC. The written sample is off unless rehearsal GO was said inside that window.

## During the Thursday sample only

Every UTC second, per sender:

- sender id, target, submitted, accepted
- the endpoint that sender posts to
- the local pool and each public pool, each named
- submit-call latency

A pool that sticks gets its name in the note.

Every UTC minute, per sender, the three 8 Oct fields above.

On a sample of transactions, and on every reject: submit time and accept time.

NTP at 18:00 and at 20:00 on both sides.

Pass, if the sample runs: mean submitted at least 95% of that side's target, no zero second, the second lines, the minute lines, NTP, the bot's matched/total line, sender count 0 again by 18:55 UTC, the halt file still saying halt at 20:00 UTC, and no key, seed, address, or txid in git.

Pass, if the sample is skipped: the skip reason in the Friday call, every due row filled or marked not measured, a 20:00 stop line on both sessions, sender count stayed 0, halt still halt, public result sections empty, open Friday gates listed.

## Friday clean run, the plan's logger

These stay on for the clean run. Tonight's checkout does not shrink them and does not run them early.

| Piece | What is logged |
|---|---|
| §1 | At T0, the SHA of the last commit that changed `plan/NEXT-STORM-PLAN.md`. Deviations go in a deviations list with the time and the reason. |
| §2 | B0, 10 minutes, senders off, probes and ordered stream on. B1 the same after the final drain. Baseline B is median network-wide unique accepted tx/s, minus our own probe and stream transactions. |
| §3 | Steps 2×, 5×, 10×, 20×, 30×, then max. 15 minutes on, 5 minutes drain. Max uses 7 runners and a 10-minute drain. Nothing changes inside a step. Never 8 runners. |
| §3b | Miners-off control at the 2× load. Publish the imperfect-control note. If the control hits saturation, flag it backlog-bound and do not use its reorder numbers as the control. |
| §3a | Build's paced share default 25%, four fixed sender processes, own coins, own logs, no auto-scale, no fleet relaunch, no mempool pause inside a step. Fee 1× and 1.5×, cap 600, frozen from the step-start quote. |
| §3c | Saturation yes or no, onset UTC, A60/S60 at onset and at the step end, and whether the drain cleared the backlog. Also per sender. |
| §4 | Per second: submit-OK, rejects by reason, offered, accepted split by fee tier. Accepted counted by accept second and by submit second. Network-wide unique accepted from n0's virtual-chain notifications. |
| §4 | Per transaction, lanes in a 1-in-10 sample and all probes: send sequence, submit start, submit-OK, accept time, accept position, fee tier. |
| §4a | Ordered stream, 2 per second per tier at 1× and 1.5×. Reorder rate, out-of-order accepts, stalls, and fee-driven overtakes, each as a count and a percentage, with n and a 95% interval. |
| §5 | About 450 probes per tier per step. Report n, p50, p95, p99, worst, and the share over 30 seconds and over 60 seconds. |
| §6 | api-tn10 health every 30 seconds. One already-accepted probe polled once a minute until it is visible. Freeze: 3 samples (90 seconds) of 503 or timeout, or lag above 120 seconds and rising, or visibility delay above 300 seconds. n0 mempool every 1 second. Fee estimate every 10 seconds. |
| §6a | n0 CPU, RSS, runner CPU, mempool against the 100,000 cap, evictions, reject reasons. Plateau label: box-bound, network-bound, or unclear, by the criteria fixed in that section. |
| §7 | Mining share per second and per step: blocks total, blocks ours, percent. Include the miners-off step. Blocks per second and difficulty next to it. |
| §8 | Raw CSV next to the summary: `steps.jsonl`, `per_second.csv`, `probes.csv`, `ordered_stream.csv`, `order_per_step.csv`, `build_per_second.csv`, `build_tx_sample.csv.gz`. |

Side by side, before any reading: his chain count and our count, on the same window. He sends the comparison first. A submit count and a chain-accepted count stay two numbers until the same ids are on both clocks.

## 7 Oct compare

Closed on 8 Oct. He asked for start, end, target tx/s, sent against accepted, which node, and a handful of tx ids for 18:52–19:23 UTC. Our log does not cover that window. The last submit is 18:38:39 UTC. Neither the 2,750 figure nor the pool near 9.7k is a ceiling. The reading is [PULSE-WINDOW-7-OCT.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/1335faffbfb5407d7eda665d60203f455813a933/plan/PULSE-WINDOW-7-OCT.md). Tonight does not invent that window.

## Who writes, and who does not

Build appends [RESULTS.md](RESULTS.md) and pushes this private repo. The bot prints its block. The desk copies that block into the bot columns. Kaspa Pulse counts the chain from outside the setup. This checkout does not send him the sheet.

Intentions are good; thought process is questionable. STP remains delusional. Si vis pacem, para bellum.
