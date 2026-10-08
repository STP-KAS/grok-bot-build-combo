> **Experimental. We are just trying this.**
>
> [Disclaimer](../DISCLAIMER.md)

Wording, Kaspa Pulse (@gokugalax), 7 Oct 2026: sign-and-send processes are senders; runner is the setup; bot is reserved for the operator.

# What is monitored

Source of the fields: Kaspa Pulse ([@gokugalax](https://x.com/gokugalax)), written up in [PULSE.md](PULSE.md). The plan's log rules are §3c, §4, §6, and §7 of NEXT-STORM-PLAN. If this page and the plan disagree, the plan wins.

The sheet is [RESULTS.md](RESULTS.md). Build appends the row and pushes the private repo. The bot prints the block. The desk copies the bot block into the bot columns. A number that was not read is **not measured**.

## Every 10 minutes, both sides

| Field | Bot, on the box | Build, on the desk |
|---|---|---|
| UTC | the row time | the row time |
| Session | up or down | up or down |
| Sender count | lane runners | Build senders |
| Disk free | box GB | desk GB, labeled desk |
| Clock | NTP offset, two public servers | `w32tm` offset, 5 samples |
| Usage | product counter, or not measured | product counter, or not measured |
| n0 | synced, lag seconds, mempool, CPU when a sample is on | not read from the desk |
| Pools | n0 mempool | six public names, each named, plus the desk node |
| Indexer | api-tn10 health: HTTP, `isSynced`, `acceptedTxBlockTimeDiff`, `blueScoreDiff` | same check if the bot row is missing |
| Rates | submitted tx/s and accepted tx/s | submitted tx/s and accepted tx/s |
| Miners | count, on or off | count, on or off, no switch |

Lane rates are 0 on every row outside 18:30–18:45 UTC.

## During the sample only

Every UTC second, per sender, as in [PLAN.md](PLAN.md). Submitted and accepted stay two columns. A pool that sticks gets its name in the note. Saturation, for this sample, uses the plan's rule on our own transactions: accepted under 95% of submitted, sustained 60 seconds, scored from 60 seconds after the start. Report yes or no, and the onset UTC if yes.

On top of that second log, every UTC minute, per sender, one local line. This is the 8 Oct ask. It does not replace the second log.

| Field | What it is |
|---|---|
| minute | `YYYY-MM-DDTHH:MM:00Z` |
| sender id | that sender |
| node | the node it posted to. Build: one named public TN10 node. Bot: n0. Not the word "public". Mempool is per node. |
| tx_sent | submissions by that sender in that minute |
| tx ids | five, spread across the minute, not the first five |

His accepted count is his. Do not invent it. The five ids go in the local log and in the checkout PDF if the desk already writes one, else in a local `checkout-minute.csv`. They do not go in [RESULTS.md](RESULTS.md).

The Build gate is a different 95%. Mean achieved send rate at least 95% of the 62 tx/s target, with no zero seconds. The bot's line is the same shape at 188 tx/s.

## Pass, if the sample runs

All of these:

- Mean submitted rate on each side is at least 95% of that side's target.
- No second at 0 during 18:30–18:45 UTC on a sender that was armed.
- Each second has sender id, target, submitted, accepted, endpoint, named pools, submit latency.
- Each sample minute has the local line: minute, sender id, named node, tx_sent, five tx ids.
- Local logs have submit time and accept time for the sample and for every reject.
- NTP exists at 18:00 and at 20:00 on both sides. If the desk offset moved by more than 50 ms between those two reads, flag Build's confirmation times. The plan's rule is the same flag.
- The bot's match line is matched/total. A missing match fails the sample.
- Sender count is 0 again by 18:55 UTC.
- The halt file still says halt at 20:00 UTC.
- The git file contains no key, seed, address, or txid.

## Pass, if the sample is skipped

All of these:

- The skip reason is one line in the Friday call.
- Every due monitor row is filled or marked not measured.
- Both sessions have a 20:00 UTC stop line.
- Sender count stayed 0.
- The halt file still says halt.
- Public result sections stayed empty.
- The open Friday gates are listed, not filled with a guess.

## Who does not watch from inside the setup

Kaspa Pulse. His count is the chain. On 8 Oct 2026 he pointed it at tonight 18:00–20:00 UTC, and at Friday 21:25 UTC through Saturday 05:35 UTC, two nodes. Comparison comes to us first. Tonight's sheet is still ours. This checkout does not send it to him.

Intentions are good; thought process is questionable. STP remains delusional. Si vis pacem, para bellum.
