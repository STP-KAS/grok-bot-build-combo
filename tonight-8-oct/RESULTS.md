> **Experimental. We are just trying this.**
>
> [Disclaimer](../DISCLAIMER.md)

Wording, Kaspa Pulse (@gokugalax), 7 Oct 2026: sign-and-send processes are senders; runner is the setup; bot is reserved for the operator.

# Monitor results

Private record for the Thursday 8 Oct 2026 checkout. Rules: [MONITOR.md](MONITOR.md). Clock: [PLAN.md](PLAN.md).

A figure is a reading from this session, or **not measured**. Ids, keys, seeds, and addresses stay out of this file.

The public storm result sections stay empty. This file is not those sections.

## Morning reading, before the window

Read on the desk at **2026-10-08T08:24:34Z**, node census at **2026-10-08T08:25:25Z**. The evening window opens at 18:00 UTC. The bot was not read. n0 was not read. Usage was not read.

| Check | Reading |
|---|---|
| Desk clock | `w32tm` stratum 2, source time.nist.gov, last sync 2026-10-08T08:23:57Z. Root delay 0.123 s. Root dispersion 7.863 s. |
| Desk NTP vs time.windows.com | Five samples at 08:24:34Z: −0.1025523 s, −0.1027508 s, −0.1027172 s, −0.1026246 s, −0.1025256 s. Mean −0.1026 s. |
| Desk disk free | 647.8 GB. This is the desk, not the bot disk. |
| Desk kaspad | One process. Local Borsh open. testnet-10, kaspad 2.1.0, synced, UTXO index on, mempool 0, normal fee 100, priority fee 100. |
| Desk miners | 18 one-thread miners, suffix `stp grok build`. Count logged. Not switched. |
| Sender count | 0. No measure, scale, lane, p2w, campaign, or observe process. |
| Older fleet halt | Present. First line `halt`. |
| Desk measure arm file | Present. First line `fee2h`. Sender count is still 0. This is not rehearsal GO and not storm GO. |
| Measure STOP file | Absent. Left absent. |
| Faucet keeper | One desk keeper was running. Left running. |

### Public TN10 names, 2026-10-08T08:25:25Z

All six answered testnet-10, kaspad 2.1.0, synced, UTXO index on. Virtual DAA scores during this sequential pass ran from 591144635 to 591144662. Tips moved during the pass, so this pass does not count machines. The 7 Oct census of three machines stands until a check separates them on purpose.

| Name | Mempool | Normal fee | Priority fee |
|---|---:|---:|---:|
| vector-10 | 5776 | 173 | 306 |
| proton-10 | 0 | 100 | 100 |
| electron-10 | 0 | 100 | 100 |
| muon-10 | 50 | 100 | 100 |
| quark-10 | 7 | 100 | 100 |
| neutrino-10 | 0 | 100 | 100 |
| desk node | 0 | 100 | 100 |

Vector's normal quote is above the idle floor and below 200. The sample, if it runs, still asks for a fresh quote at 18:30 UTC before it freezes 200 and 300.

### Indexer, 2026-10-08T08:24:34Z

api-tn10 health: database `isSynced` true, `blueScoreDiff` 10, `acceptedTxBlockTimeDiff` 1 second. Reported server kaspad 2.1.0, UTXO index on, synced.

### Plan SHA

Desk questions repo HEAD `2c5235b23d4fdd9a814af4703fafdef01165d3e1`. `origin/main` is `1335faffbfb5407d7eda665d60203f455813a933`. The last commit that touches `plan/NEXT-STORM-PLAN.md` on this desk is that HEAD. This is not a lock. Friday writes the lock SHA at T0. The public result sections were not filled by this reading.

### Morning rows that are not measured

Bot session, bot disk, n0 sync, n0 lag, bot NTP, bot usage, Build usage, n0 match, box dry run.

## Evening rows

Due every 10 minutes. Status stays **not measured** until that UTC is read. The 18:00 and 18:10 rows were not read at those clocks, so those cells stay **not measured**. Log times and rates are in the pre-test section below, with the UTC of the log.

| UTC | Phase | Bot up | Build up | Senders | Bot disk GB | Desk disk GB | n0 lag s | NTP bot | NTP desk | Usage bot | Usage build | Submit tx/s | Accepted tx/s | Pool note | Indexer | Note |
|---|---|---|---|---:|---|---|---|---|---|---|---|---|---|---|---|---|
| 18:00 | R0 | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | window opens |
| 18:10 | R0 | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | |
| 18:20 | R1 | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | quiet starts |
| 18:30 | R2 | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | sample only with rehearsal GO |
| 18:40 | R2 | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | |
| 18:50 | R3 | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | drain |
| 19:00 | R4 | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | |
| 19:10 | R4 | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | |
| 19:20 | R5 | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | Friday call starts |
| 19:30 | R5 | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | |
| 19:40 | R5 | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | |
| 19:50 | R5 | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | |
| 20:00 | stop | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | both sessions stop |

## Sample block

Status: **not measured**. Rehearsal GO was not said. The 18:30–18:45 UTC sample has not started. The pre-test section is a separate send. It does not fill this block.

| Field | Value |
|---|---|
| rehearsal GO | not measured |
| First submit UTC | not measured |
| Last submit UTC | not measured |
| Build target / mean submitted / mean accepted | not measured |
| Bot target / mean submitted / mean accepted | not measured |
| Zero seconds | not measured |
| Rejects | not measured |
| Saturation (60 s under 95%) | not measured |
| n0 match | not measured |
| Fee pair | 200 and 300, cap 600, if the sample starts under the quote rule |

## Friday call

Status: **not measured**. Due from 19:40 UTC. The lines and the pass rules are in [PLAN.md](PLAN.md).

| Line | Status | Note |
|---|---|---|
| Both sessions alive to 20:00 UTC | not measured | |
| Usage headroom for 8 hours | not measured | Two hours do not prove eight. |
| Bot disk ≥ 35 GB | not measured | Desk 647.8 GB is not this line. |
| n0 synced, lag ≤ 300 s | not measured | |
| Desk node synced | pass at 08:25:25Z | Recheck at 18:00 UTC. |
| Public names rechecked | pass at 08:25:25Z | Machine count not re-proven. Recheck before Friday. |
| Sample | not measured | |
| n0 match | open | |
| Box dry run | open | A 15-minute sample does not close this by itself. |
| Halt still halt | pass at 08:24:34Z | Recheck at 20:00 UTC. |
| `fee2h` unused as a GO | pass at 08:24:34Z | Sender count was 0. |
| Public result sections empty | pass | This file is private. |
| Plan unlocked, no storm GO, no steps-utc.json | pass | Left that way. |
| Friday ready | not measured | stp decides after the 20:00 UTC row. |

## Pre-test Build result

Private Build readings from this desk on 8 Oct 2026. They are not the rehearsal sample, and they are not the storm. The public result sections in tn10-storm-throughput-questions stay empty. This note does not ping Kaspa Pulse. His accepted count is his.

The monitor list is [MONITOR-PLAN.md](MONITOR-PLAN.md). The plan cited for the rules is [NEXT-STORM-PLAN.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/1335faffbfb5407d7eda665d60203f455813a933/plan/NEXT-STORM-PLAN.md) at `1335faffbfb5407d7eda665d60203f455813a933`. The desk copy of that repo is `2c5235b23d4fdd9a814af4703fafdef01165d3e1`, five commits ahead, and this note does not push it. The checkout this note was added to was `cb960744524f17dd88b0e7f22f2c6c7bb049690d`. This is not a lock.

On the finished runs, the figure used for accepted is the summary line's `accept_seen`. Summing the per-second `accept_seen` field undercounts on this harness. That sum is not used for pre8 or s7.

### Desk reading, 2026-10-08T18:14:08Z

| Check | Reading |
|---|---|
| Desk disk free | 646.8 GB. This is the desk, not the bot disk. |
| Desk NTP | `w32tm` stratum 2, source time.nist.gov, last sync 2026-10-08T18:12:22Z. Root delay 0.123 s. Root dispersion 7.869 s. |
| Desk NTP vs time.windows.com | Five samples: −0.1164770 s, −0.1087657 s, −0.1086743 s, −0.1085520 s, −0.1088182 s. Mean −0.1103 s. |
| Desk kaspad | One process. |
| Desk miners | 18. Count logged. Not switched. |
| Older fleet halt | Present. First line `halt`. |
| Desk measure arm file | Present. First line `fee2h`. This is not rehearsal GO and not storm GO. |
| Measure STOP file | Absent. Left absent. |
| Sender count | 6. Step k3, still inside its 1,800 s arm. |
| Indexer | One api-tn10 health read. Database `isSynced` true, `blueScoreDiff` 32, `acceptedTxBlockTimeDiff` 2 seconds. This is not the every-30-seconds series. |
| Bot session, bot disk, bot NTP, n0, usage, n0 match | not measured |

### pre8, finished

Checkout shape. Four senders, targets 16, 16, 15, and 15 tx/s. Depth 2. Fee frozen at 200 and 300 sompi/gram, cap 600. `via` both. Each sender's nodes were the desk node, vector-10.kaspa.green, and proton-10.kaspa.stream.

Armed from 2026-10-08T15:49:32Z. Summary lines from 2026-10-08T16:04:32Z to 2026-10-08T16:04:33Z. Each sender logged 895 seconds.

| Sender | Target | Submit | Summary accept_seen | Zero seconds | Rejects | Percent of target |
|---|---:|---:|---:|---:|---:|---:|
| a | 16 | 14320 | 14320 | 0 | 0 | 100 |
| b | 16 | 14320 | 14319 | 0 | 0 | 100 |
| c | 15 | 13425 | 13424 | 0 | 0 | 100 |
| d | 15 | 13425 | 13425 | 0 | 0 | 100 |

Combined submit 55,490. Combined summary accept_seen 55,488. Two transactions were still short of the summary accept count at the stop. Mean submit was 62 tx/s, 100% of the 62 tx/s target. The local minute file is on the desk. Its ids stay out of this file.

### s7, finished, before 18:00 UTC

Seven senders, targets 16, 16, 15, 15, 16, 16, and 15 tx/s. Sum 109 tx/s. Depth 2. Fee frozen at 200 and 300, cap 600. `via` public. Nodes on each sender: vector-10.kaspa.green, proton-10.kaspa.stream, electron-10.kaspa.blue, muon-10.kaspa.blue.

Armed from 2026-10-08T17:22:11Z. Summary lines from 2026-10-08T17:52:12Z to 2026-10-08T17:52:15Z.

| Sender | Target | Seconds | Submit | Summary accept_seen | Zero seconds | Rejects |
|---|---:|---:|---:|---:|---:|---:|
| k1 | 16 | 1790 | 28640 | 28640 | 0 | 0 |
| k2 | 16 | 1789 | 28624 | 28624 | 0 | 0 |
| k3 | 15 | 1790 | 26850 | 26850 | 0 | 0 |
| k4 | 15 | 1790 | 26850 | 26850 | 0 | 0 |
| k5 | 16 | 1790 | 28640 | 28640 | 0 | 0 |
| k6 | 16 | 1790 | 28637 | 28634 | 0 | 0 |
| k7 | 15 | 1789 | 26835 | 26835 | 0 | 0 |

Combined submit 195,076. Combined summary accept_seen 195,073. Each sender's mean was 100% of its own target. Three submissions on k6 were short of that sender's summary accept count.

### k3, desk node, snapshot at 2026-10-08T18:14:06Z

Six senders, r1 through r6. Target 504 tx/s each, 3,024 tx/s together. `via` own. Node: the desk node. Depth 4. Lanes 1,008. Four connections. Fee frozen at 100 and 150 sompi/gram, cap 600. Per-transaction logging was off, so this run has no submit time, no accept time, and no five ids.

Armed 2026-10-08T18:01:20Z for 1,800 seconds. Expected stop about 18:31:20Z. No summary line yet. The accept figure below is the sum of the per-second `accept_seen` field. On pre8 and s7 that sum undercounted the later summary, so this accept figure can move when the summary lines are written.

Aligned seconds, all six logs present: 732, from 2026-10-08T18:01:24Z through 2026-10-08T18:14:06Z.

| Sender | Seconds | Submit | accept_seen sum | Zero submit seconds | Rejects | Max depth |
|---|---:|---:|---:|---:|---:|---:|
| r1 | 761 | 275625 | 267545 | 0 | 0 | 3874 |
| r2 | 761 | 276038 | 268390 | 0 | 0 | 3820 |
| r3 | 760 | 274875 | 267666 | 0 | 0 | 3866 |
| r4 | 760 | 274996 | 267134 | 0 | 0 | 3849 |
| r5 | 760 | 274980 | 267979 | 0 | 0 | 3920 |
| r6 | 759 | 274501 | 266511 | 0 | 0 | 3817 |

Together, on the 732 aligned seconds: submit 1,588,926, mean 2,170.7 tx/s. That is 71.8% of the 3,024 target. The plan's sender-limited line is submit-OK under 95% of target. This snapshot is under that line.

accept_seen sum 1,547,876, mean 2,114.6 tx/s, which is 97.4% of the submit sum on those seconds. The last 60 aligned seconds were 2,173.2 submit tx/s and 2,186.8 accept_seen tx/s. The longest run of aligned seconds with accept_seen under 95% of submit was 12 seconds.

The plan's saturation rule (§3c) counts our transactions on n0's virtual chain. n0 was not read. That rule is **not measured**.

The arm cap is 1,008 lanes times depth 4, which is 4,032. The logged depth reached 3,817 to 3,920, so the pipe was near that cap.

### Runs left unscored

A four-sender public run and a fifteen-sender public start were stopped so the next coin partition would not spend the same coins. This note does not give them a rate.

### Mining share

**Not measured** on these sends. The plan's §7 counter, one line per block from n0, was not running. Storm 2's published block share was about 50–63% of TN10 blocks. His earlier figure was near 60% of TN10 hashrate. This section does not pick a new share.

### Deviations from the written Thursday sample

1. Rehearsal GO was not said. The 18:30–18:45 UTC sample did not start.
2. pre8 posted to the desk node as well as vector-10.kaspa.green and proton-10.kaspa.stream.
3. s7 used seven senders at 109 tx/s, on four named public nodes, for about 30 minutes, and it ended before 18:00 UTC.
4. k3 uses six senders, a 3,024 tx/s target, the desk node, depth 4, and fee 100 and 150, with per-transaction logging off.
5. The 18:00 and 18:10 monitor rows were not read at those clocks.
6. n0 match, bot NTP, bot disk, and usage were not measured.

k3 was still running at the 18:14 UTC snapshot. The six summary lines were not in yet.

## Stop line

not measured

Intentions are good; thought process is questionable. STP remains delusional. Si vis pacem, para bellum.
