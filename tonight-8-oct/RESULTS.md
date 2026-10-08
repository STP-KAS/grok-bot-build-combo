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

Due every 10 minutes. Status stays **not measured** until that UTC is read.

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

Status: **not measured**. The window has not opened.

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

## Stop line

not measured

Intentions are good; thought process is questionable. STP remains delusional. Si vis pacem, para bellum.
