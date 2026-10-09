> **Experimental. We are just trying this.**
>
> [Disclaimer](DISCLAIMER.md)

Thank you, Kaspa Pulse (@gokugalax), for the guidance and the input over this stretch, from 4 Oct 2026 on. The 7 Oct 2026 wording stays: sign-and-send processes are senders; runner is the setup; bot is reserved for the operator.

# Combo: Grok Bot and Grok Build

Every clock time in this repo is UTC. A clock is not written in local time.

**Goal.** One TN10 test of both senders on one clock, after the usage reset. Friday 9 Oct 2026, 21:30 UTC, for 8 hours, ending Saturday 10 Oct 2026, 05:30 UTC. If that day is not ready, Monday 13 Oct 2026, 21:30 UTC, for 8 hours, ending Tuesday 14 Oct 2026, 05:30 UTC.

The usage reset for the bots and for Build is **OK**, on stp's word, 7 Oct 2026. The combo has not been run. This page does not lock the questions plan.

**Start.** Sending this GitHub to Grok Build or to the bot means go: start the operation.

## Node split, 9 Oct 2026

[TWO-NODES.md](TWO-NODES.md) is the forward rule. The two desk nodes are **locus** and **keel**. locus is the first kaspad. Build uses it on every step. keel is the second kaspad, still syncing on 9 Oct 2026, and already in the score. The bot's runner and the bot's miners use the tunnel to keel. n0 will not run. The root table below is the earlier paste. Where they disagree on the node, TWO-NODES.md wins. Where they disagree on a clock, a fee, or a question, the questions plan wins.

## Tonight, Thursday 8 Oct 2026

Checkout, 18:00–20:00 UTC. The folder is [tonight-8-oct](tonight-8-oct/README.md). Paste [PROMPT-BOT.md](tonight-8-oct/PROMPT-BOT.md) into the bot and [PROMPT-BUILD.md](tonight-8-oct/PROMPT-BUILD.md) into Grok Build at 17:50 UTC. The morning monitor reading is in [RESULTS.md](tonight-8-oct/RESULTS.md). Kaspa Pulse's input is in [PULSE.md](tonight-8-oct/PULSE.md). Tonight is not the storm. The root prompts below are the Friday paste.

On 8 Oct he read the checkout PDF and pointed his counter at that same 18:00–20:00 UTC, and at Friday 21:25 UTC through Saturday 05:35 UTC. Comparison comes to us first. The pastes now ask for a per-minute sent count, the node name, and five tx ids in the local log. Git still gets no ids. The DM times 20:00 UTC tonight and 21:00 UTC Friday are not these clocks.

The measurement plan remains [NEXT-STORM-PLAN.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/NEXT-STORM-PLAN.md). If this hub and that plan disagree on a clock, a fee, or a question, the plan wins. If they disagree on the node, [TWO-NODES.md](TWO-NODES.md) wins.

## Two prompts

| Who | Paste this | Wallet | Where it sends |
|---|---|---|---|
| Grok Build, on the desk | [PROMPT-BUILD.md](PROMPT-BUILD.md) | Build only | locus |
| Grok Bot, on the box | [PROMPT-BOT.md](PROMPT-BOT.md) | Bot only | keel, through the tunnel, and only during the storm |

Each prompt is for one side. Neither spends the other wallet.

## Prompt bot reset

[PROMPT-BOT-RESET.md](PROMPT-BOT-RESET.md) is the 8 Oct prepare page. Do not paste it to bring n0 back. n0 will not run. The forward paste is [PROMPT-BOT.md](PROMPT-BOT.md).

## Prompt build

Paste [PROMPT-BUILD-TONIGHT.md](PROMPT-BUILD-TONIGHT.md) into Grok Build when the link arrives. Same prepare-now line as the bot page. Same goal and the same clocks: full load, full monitoring, not announced. Miners stay on. The desk node stays up and the senders do not use it. It does not replace [PROMPT-BUILD.md](PROMPT-BUILD.md) or [tonight-8-oct/PROMPT-BUILD.md](tonight-8-oct/PROMPT-BUILD.md).

## Clock

T0 is **21:30 UTC**. The first load step is **10 minutes later**.

| | Friday 9 Oct 2026 | Monday 13 Oct 2026 |
|---|---|---|
| T0, B0 starts, lane senders off | 21:30 UTC | 21:30 UTC |
| First TPS step, the 2× load | 21:40 UTC | 21:40 UTC |
| Paced table ends, T0+175 | Sat 10 Oct 00:25 UTC | Tue 14 Oct 00:25 UTC |
| Storm ends | Sat 10 Oct 05:30 UTC | Tue 14 Oct 05:30 UTC |

B0 is 10 minutes. Both lane senders stay off. The plan keeps the box probes and the box ordered stream running in B0. Build sends nothing in B0, including its own ordered stream.

His Friday counter is 21:25 UTC to Saturday 05:35 UTC. That is five minutes either side of this table. It does not move T0.

## From the prompt to the first TPS

The prompt does not start the storm. It waits until both of these exist, and until the clock is at the first time in the second:

1. A storm GO from stp, separate from any earlier dry-run GO.
2. `steps-utc.json`, with a UTC start and a UTC end for every step.

When those two are in hand before 21:30 UTC, the first TPS step starts at **21:40 UTC**. That is **10 minutes** after T0.

Pasting a prompt without those two files stops the side that was pasted. It does not arm a countdown.

Read at **2026-10-07T19:00:19Z**. The calendar gap from that read to 21:40 UTC on 9 Oct is **50 hours 40 minutes**. That gap is a wait. The storm GO and `steps-utc.json` were not in hand at that read.

The 6 Oct desk dry run has no logged "prompt pasted at" time. Its first numbers are not a prompt-to-start measurement.

## Checks at 2026-10-07T19:00:19Z

| Check | Result |
|---|---|
| Build prompt | Written here, and the public paste-in is [GROK-BUILD-PROMPT.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/GROK-BUILD-PROMPT.md). It does not start the storm. |
| Bot prompt | Written here. The public [BOT-TPS.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/BOT-TPS.md) is rate advice. It is not a go prompt. |
| Desk node | testnet-10, kaspad 2.1.0, synced, UTXO index on, mempool 0. |
| Six public names | All six answered testnet-10, kaspad 2.1.0, synced, UTXO index on. Mempool: vector-10 215, proton-10 550, electron-10 550, muon-10 4217, quark-10 612, neutrino-10 549. |
| Bot node n0 | Not read. This desk has no shell on the box. |
| Free space on the bot disk | **Not measured.** Last figure in the plan: about 44 GB free on Monday 5 Oct 2026, ~19:15 UTC. The go line is at least 35 GB free at T0. Below 28 GB, no storm. |
| Desk disk | Not the bot disk. |

## Still open before a storm that claims the gate

- n0 match of the desk dry-run ids
- box dry run
- 35 GB free on the bot disk at T0
- plan lock, which stays with stp
- storm GO
- `steps-utc.json`
- the hours after 00:25 UTC: name them, or end the storm at 00:25. Not chosen.

A storm GO that leaves one of the first three open has to name it. Fee for the long hold stays 200 and 300 sompi/gram. The cap stays 600.
