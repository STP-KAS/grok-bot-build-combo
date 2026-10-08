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
| 18:20 | R1 | not measured | up | 6 | not measured | 646.7 | not measured | not measured | −0.1087 s | not measured | not measured | 2161 | 2472 | not read | synced, lag 1 s, blueScoreDiff 15 | k3 pre-test still on |
| 18:30 | R2 | not measured | up | 10 | not measured | 646.3 | not measured | not measured | −0.1097 s | not measured | not measured | 1628 | 1570 | not read | synced, lag 2 s, blueScoreDiff 1 | round 4 still on; written sample not started |
| 18:40 | R2 | not measured | up | 10 | not measured | 632.6 | not measured | not measured | −0.1102 s | not measured | not measured | 3013 | 1697 | see the 18:40 read | synced, lag 2 s, blueScoreDiff 9 | late read 18:47:39Z |
| 18:50 | R3 | not measured | up | 10 | not measured | 631.9 | not measured | not measured | −0.1109 s | not measured | not measured | 2245 | 2137 | see the 18:50 read | synced, lag 3 s, blueScoreDiff 14 | round 5, depth at cap, 0 rejects |
| 19:00 | R4 | not measured | node down | 10 | not measured | 646.1 | not measured | not measured | −0.1102 s | not measured | not measured | 1653 | 1602 | see the 19:00 read | synced, lag 3 s, blueScoreDiff 14 | desk node gone at 19:00:06Z |
| 19:10 | R4 | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | |
| 19:20 | R5 | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | Friday call starts |
| 19:30 | R5 | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | |
| 19:40 | R5 | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | |
| 19:50 | R5 | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | |
| 20:00 | stop | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | not measured | both sessions stop |

### Row 18:20, read 2026-10-08T18:20:20Z

R1 is the quiet phase. Rehearsal GO was not said. The six k3 senders were still inside their 1,800 s arm. That is the pre-test, not the rehearsal sample.

Desk NTP vs time.windows.com, five samples from 18:20:22Z: −0.1087247 s, −0.1089591 s, −0.1088037 s, −0.1085677 s, −0.1086893 s. Mean −0.1087 s. `w32tm /query /status` was not run on this row.

Rates are five aligned seconds, 18:20:15Z through 18:20:19Z, all six logs present: submit 2200, 2265, 2114, 2234, 1991 (mean 2160.8). Local accept_seen 3330, 2135, 2970, 1955, 1970 (mean 2472). That accept figure is the sender's per-second field. It is not n0, and it is not Kaspa Pulse's chain count. The six public pools and the desk-node mempool were not read on this row. One kaspad. Miners 18, not switched. Halt file first line `halt`. Arm file first line `fee2h`. Measure STOP absent. Indexer: database `isSynced` true, `acceptedTxBlockTimeDiff` 1 second, `blueScoreDiff` 15.

### Row 18:30, read 2026-10-08T18:30:16Z

R2 is the written sample phase. Rehearsal GO was not said. The real test is postponed while n0 is still syncing, so the 62 tx/s sample did not start. Round 4's ten senders were still inside the one-hour arm.

Desk NTP vs time.windows.com, five samples from 18:30:18Z: −0.1098801 s, −0.1096296 s, −0.1094852 s, −0.1097370 s, −0.1096650 s. Mean −0.1097 s.

Rates are eleven aligned seconds, 18:29:55Z through 18:30:05Z, all ten logs present, 0 rejects. Submit 2063, 1565, 1820, 1972, 1460, 2238, 576, 1393, 1315, 1422, 2080. Mean 1,627.6 tx/s. Local accept_seen 1974, 1497, 1738, 1933, 1440, 2144, 586, 1311, 1283, 1258, 2103. Mean 1,569.7 tx/s. That accept figure is the sender log, not n0. Depth was 4,032 on every one of those seconds, which is the arm cap. The six public pools and the desk-node mempool were not read. One kaspad. Miners 18, not switched. Halt file first line `halt`. Measure STOP absent. Indexer: database `isSynced` true, `acceptedTxBlockTimeDiff` 2 seconds, `blueScoreDiff` 1.

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

On the finished runs that wrote a summary line, the figure used for accepted is that line's `accept_seen`. Summing the per-second `accept_seen` field undercounts on this harness. That sum is not used for pre8 or s7. Round 3 was stopped before it wrote a summary, so its accept figure is the per-second sum.

The real test is postponed. n0 was still syncing when round 4 started. These rounds are desk tests until that sync is done. They are not rehearsal GO, and they are not storm GO.

## Rounds

| Round | Date | Start UTC | End UTC | Senders | Node | Target | What the log showed |
|---|---|---|---|---:|---|---:|---|
| 1 pre8 | 2026-10-08 | 15:49:32 | 16:04:33 | 4 | desk node, vector-10.kaspa.green, proton-10.kaspa.stream | 62 tx/s | Summary submit 55,490. Summary accept_seen 55,488. 100% of target. 0 rejects. |
| 2 s7 | 2026-10-08 | 17:22:11 | 17:52:15 | 7 | vector-10.kaspa.green, proton-10.kaspa.stream, electron-10.kaspa.blue, muon-10.kaspa.blue | 109 tx/s | Summary submit 195,076. Summary accept_seen 195,073. 100% of each sender's target. 0 rejects. |
| 3 k3 | 2026-10-08 | 18:01:20 | 18:22:36 | 6 | desk node | 3,024 tx/s | Stopped so round 4 could use the coins. 1,215 aligned seconds. Submit mean 2,191.2 tx/s. Local accept_seen mean 2,142.9 tx/s. 0 rejects. No summary line. |
| 4 h10 | 2026-10-08 | 18:24:48 | 18:37:37 | 10 | desk node | 5,040 tx/s | Stopped so a larger set could be tried. 714 aligned seconds. Submit mean 1,854.8 tx/s. Local accept_seen mean 1,750.7 tx/s. 0 rejects. |
| 5 q10 | 2026-10-08 | 18:48:19 | 19:00:06 | 10 | desk node | 5,040 tx/s | Desk node process gone at 19:00:06Z. No shutdown line. Senders then submitted 0. |
| 6 u10 | 2026-10-08 | 19:02:53 | 19:48:19 planned | 10 | desk node | 5,040 tx/s | Node restarted and synced. Miners restored to 18. Opening seconds submitted 5,040 with 0 rejects. |

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

### Round 3 closed, 2026-10-08T18:22:36Z

The six senders were stopped at the last second above so round 4 would not spend the same coins. The arm had been 1,800 seconds, with a planned end near 18:31:20Z. This close is short of that end. No summary line was written. Accept here is the sum of the per-second `accept_seen` field.

Aligned seconds, all six logs present: 1,215, from 2026-10-08T18:01:24Z through 2026-10-08T18:22:36Z. Submit 2,662,313, mean 2,191.2 tx/s, 72.5% of the 3,024 target. accept_seen sum 2,603,621, mean 2,142.9 tx/s, 97.8% of that submit sum. Longest run of aligned seconds with accept_seen under 95% of submit: 12 seconds. Zero submit seconds: 0. Rejects: 0. The plan's n0 saturation rule is **not measured**.

| Sender | Seconds | Submit | accept_seen sum | Max depth | Last second UTC |
|---|---:|---:|---:|---:|---|
| r1 | 1268 | 463706 | 452339 | 3874 | 18:22:36.601 |
| r2 | 1268 | 463966 | 454158 | 3820 | 18:22:36.586 |
| r3 | 1268 | 463148 | 452914 | 3866 | 18:22:37.143 |
| r4 | 1267 | 462763 | 452177 | 3849 | 18:22:36.614 |
| r5 | 1267 | 463177 | 453864 | 3920 | 18:22:36.904 |
| r6 | 1266 | 462276 | 450919 | 3817 | 18:22:36.467 |

### Round 4, ten senders, one hour, started 2026-10-08T18:24:48Z

Ten senders, h01 through h10, parts 0/10 through 9/10. Target 504 tx/s each, 5,040 tx/s together. `via` own. Node: the desk node. Depth 4. Lanes 1,008. Four connections. Fee frozen at 100 and 150 sompi/gram, cap 600. Per-transaction logging is off. Armed for 3,600 seconds. Planned end 2026-10-08T19:24:48Z.

Desk check before the arm, 2026-10-08T18:22:47Z: mempool 0, normal fee 100, 1.5× fee 150, server 2.1.0. Lane coins on the unsplit part were 13,678. Each sender armed at 1,008 lanes.

All ten were alive after the arm. First aligned seconds, all ten logs present, 0 rejects:

| UTC | Submit | Local accept_seen | Max depth |
|---|---:|---:|---:|
| 18:24:58 | 5015 | 1539 | 3541 |
| 18:24:59 | 3798 | 2251 | 3582 |
| 18:25:00 | 3145 | 1973 | 3728 |
| 18:25:01 | 2872 | 1412 | 3880 |
| 18:25:02 | 2973 | 1750 | 3976 |

The first second was on the 5,040 target. Four seconds later the pipe was near the 4,032 depth cap and submit was 2,973. Local accept_seen was still behind submit. This is the opening, not the hour.

### Round 4 closed, 2026-10-08T18:37:37Z

Stopped so a larger set could take the coins. The planned end was 19:24:48Z. No summary line. Accept is the per-second `accept_seen` sum.

Aligned seconds, all ten logs present: 714, from 2026-10-08T18:24:50Z through 2026-10-08T18:37:37Z. Submit 1,324,305, mean 1,854.8 tx/s. accept_seen sum 1,249,972, mean 1,750.7 tx/s. Rejects 0.

A twelve-sender arm at 18:38:51Z left 0.4 GB free. Two processes were cut. The node then rejected transactions as orphans. A second twelve-sender arm left 0.6 GB free, with about 4,258 submit/s, 1,053 local accept_seen/s, and about 4,761 rejects/s. Both were stopped. Twelve is above what this desk can hold. Ten is the count that left 2.7 GB free and submitted with 0 rejects.

### Round 5, ten senders, started 2026-10-08T18:48:19Z

Ten senders, q01 through q10, parts 0/10 through 9/10. Target 504 tx/s each, 5,040 together. `via` own. The desk node. Depth 4. Four connections. Fee frozen at 100 and 150 sompi/gram, cap 600. Per-transaction logging is off. Armed for 3,600 seconds. Planned end 2026-10-08T19:48:19Z.

Lane counts at the arm: 1008, 956, 1008, 940, 762, 862, 1008, 895, 1008, 482. Four of the ten are under 1,008 lanes.

Free RAM with all ten up: 2.7 GB. First aligned seconds, all ten logs present, 0 rejects:

| UTC | Submit | Local accept_seen |
|---|---:|---:|
| 18:48:29 | 3856 | 2124 |
| 18:48:30 | 2944 | 1325 |
| 18:48:31 | 2625 | 1359 |
| 18:48:32 | 2627 | 1980 |

Mean of those four seconds: 3,013 submit/s, 1,697 local accept_seen/s.

### Row 18:40, read 2026-10-08T18:47:39Z

Late for the 18:40 mark. This is the PDF row: UTC, phase, session, sender count, desk disk, NTP, usage, submit, accepted, the six public mempools by name, desk mempool, indexer, note. The count row has no ids.

| Field | Reading |
|---|---|
| Phase | R2 |
| Session | up |
| Desk disk free | 632.6 GB |
| NTP vs time.windows.com | Five samples ending 18:47:39Z: −0.1103042 s, −0.1101433 s, −0.1104016 s, −0.1101091 s, −0.1100897 s. Mean −0.1102 s. |
| Usage | not measured |
| vector-10.kaspa.green | mempool 270, normal fee 100 |
| proton-10.kaspa.stream | mempool 17, normal fee 100 |
| electron-10.kaspa.blue | mempool 17, normal fee 100 |
| muon-10.kaspa.blue | mempool 421, normal fee 140 |
| quark-10.kaspa.red | mempool 10, normal fee 100 |
| neutrino-10.kaspa.stream | mempool 17, normal fee 100 |
| Desk node | mempool 0, normal fee 100, at the same census. Sender count was 0. |
| Indexer | 18:48:32Z. `isSynced` true, `acceptedTxBlockTimeDiff` 2 seconds, `blueScoreDiff` 9. |
| Rates | After round 5 armed, the four seconds above. |
| Miners | 18. Not switched. Halt file first line `halt`. |

### Row 18:50, read 2026-10-08T18:50:12Z

Round 5's ten senders were up. Free RAM 5.6 GB. Halt file first line `halt`. Miners 18, not switched.

Desk NTP vs time.windows.com, five samples from 18:50:13Z: −0.1105574 s, −0.1101328 s, −0.1103329 s, −0.1132569 s, −0.1102839 s. Mean −0.1109 s. Usage was not measured.

Rates are ten aligned seconds from 18:49:55Z through 18:50:05Z. The 18:50:02Z second was not in every log, so it is left out. Submit 2880, 2108, 1991, 2757, 2553, 2401, 2205, 1549, 1752, 2252. Mean 2,244.8 tx/s. Local accept_seen 2727, 1968, 1937, 2577, 2470, 2361, 2093, 1469, 1679, 2089. Mean 2,137 tx/s. Rejects 0. Depth was 4,032 on every one of those seconds, the arm cap.

Mempools and the normal-fee quote, read in the same minute:

| Node | Mempool | Normal fee |
|---|---:|---:|
| vector-10.kaspa.green | 24829 | 180 |
| proton-10.kaspa.stream | 24405 | 179 |
| electron-10.kaspa.blue | 24405 | 179 |
| muon-10.kaspa.blue | 32713 | 179 |
| quark-10.kaspa.red | 24405 | 179 |
| neutrino-10.kaspa.stream | 24405 | 179 |
| desk node | 34911 | 183 |

The running senders are still on the fee frozen at the arm, 100 and 150. The live quote is higher and still under 200. Indexer: `isSynced` true, `acceptedTxBlockTimeDiff` 3 seconds, `blueScoreDiff` 14.

### Row 19:00, read 2026-10-08T19:00:22Z

The desk kaspad process was already gone. Its log's last line is 19:00:06Z and it is an ordinary accepted-block line. There is no shutdown line. Miners were 0. The ten round-5 sender processes were still alive. Free RAM was 12.6 GB. Halt file first line `halt`. Desk disk free 646.1 GB.

Desk NTP vs time.windows.com, five samples from 19:00:23Z: −0.1102388 s, −0.1099277 s, −0.1103799 s, −0.1100279 s, −0.1101982 s. Mean −0.1102 s. Usage was not measured.

The last live aligned seconds, 18:59:55Z through 19:00:05Z, ten logs, 0 rejects, depth 4,032: submit 1376, 2056, 1724, 2285, 1287, 920, 1810, 1871, 1501, 1698. Mean 1,652.8 tx/s. Local accept_seen 1344, 1936, 1697, 2128, 1316, 851, 1814, 1829, 1444, 1661. Mean 1,602 tx/s. The 18:59:59Z second was not in every log, so it is left out. By 19:00:50Z those senders were at submit 0 and depth 4,032, because the node was gone.

| Node | Mempool | Normal fee |
|---|---:|---:|
| vector-10.kaspa.green | 263 | 100 |
| proton-10.kaspa.stream | 36 | 100 |
| electron-10.kaspa.blue | 36 | 100 |
| muon-10.kaspa.blue | 466 | 148 |
| quark-10.kaspa.red | 36 | 100 |
| neutrino-10.kaspa.stream | 36 | 100 |
| desk node | not read | the socket was closed |

Indexer at the same read: `isSynced` true, `acceptedTxBlockTimeDiff` 3 seconds, `blueScoreDiff` 14.

The node was started again at 19:01:33Z with the same flags, including the UTXO index, and without a RAM scale. It reached synced with the UTXO index on and mempool 0. The 18 miners were started again, one thread each, suffix `stp grok build`, priority BelowNormal. The ten round-5 senders were stopped so they would not submit the old pipe into the new process.

### Round 6, ten senders, started 2026-10-08T19:02:53Z

Same shape as round 5. Ten senders, u01 through u10, parts 0/10 through 9/10. Target 504 tx/s each. Desk node. Depth 4. Four connections. Fee frozen at 100 and 150. Per-transaction logging off. Armed for 2,728 seconds so the planned end stays 19:48:19Z.

Lane counts: 1008, 876, 1008, 797, 864, 868, 1008, 836, 1008, 830.

Opening aligned seconds, all ten logs, 0 rejects:

| UTC | Submit | Local accept_seen |
|---|---:|---:|
| 19:02:58 | 5040 | 2139 |
| 19:02:59 | 5040 | 1958 |

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
7. Round 3 was stopped at 18:22:36Z, short of its 18:31:20Z arm end, so round 4 could start.
8. Round 4 was stopped at 18:37:37Z, short of its 19:24:48Z arm end.
9. Twelve senders were tried twice. Free RAM fell to 0.6 GB and the node rejected orphans. Round 5 is ten senders, the count that stayed up with 2.7 GB free.

## Stop line

not measured

Intentions are good; thought process is questionable. STP remains delusional. Si vis pacem, para bellum.
