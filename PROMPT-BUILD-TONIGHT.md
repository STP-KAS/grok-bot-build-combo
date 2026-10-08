# Prompt build

Paste this into Grok Build on the desk for the test run tonight, 8 Oct 2026. This file does not start the storm, does not lock the plan, and does not spend.

The steps you already have are [tonight-8-oct/PROMPT-BUILD.md](tonight-8-oct/PROMPT-BUILD.md). This page is the goal, the miners, and the desk node. It is the same night as [PROMPT-BOT-RESET.md](PROMPT-BOT-RESET.md).

If this file disagrees with [NEXT-STORM-PLAN.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/NEXT-STORM-PLAN.md), stop and ask stp. The plan wins. If it disagrees with the bot reset page on the clock, stop and ask stp.

Wording, Kaspa Pulse (@gokugalax), 7 Oct 2026: sign-and-send processes are senders; runner is the setup; bot is reserved for the operator.

## Goal

The test is the heavy one already written. Full load. Full monitoring. It is not announced. Same goal as [PROMPT-BOT-RESET.md](PROMPT-BOT-RESET.md).

Not announced means do not post it, do not ping anyone, and leave the public result sections empty. The logs stay complete. A quiet test is not a smaller test, and it is not a thinner log.

Full load is the storm already written in the measurement plan and in this repo: paced steps through max, both sides, probes, the ordered stream, and the per-second logs. Friday 21:30 UTC, or Monday 13 Oct 21:30 UTC. Tonight stays the checkout size already written in [tonight-8-oct](tonight-8-oct/PLAN.md). This page does not start either one.

Full monitoring is the set already written: per-second submit and accept, per-transaction times, mempool by node name, disk, NTP, the n0 match, the saturation rule, mining share, probes at about 450 per tier per step, and the ordered stream. Five ids stay in the local log. On tonight's checkout, keep every monitor row that [tonight-8-oct](tonight-8-oct/MONITOR.md) already names. Drop none of them.

The bot brings n0 back and reports free disk, the box dry run, and the n0 match. This side runs the desk from 18:00 UTC to 20:00 UTC and reports the desk lines. 20:00 UTC is the stop.

You know the checkout. Do that at full monitoring. Do not shrink it. Then do the last act named below.

## Miners

18 miners are on this desk, read at 2026-10-08T15:03:27Z. Leave them on. Tonight's test does not turn them off. Log the count at 18:00 UTC. Do not start a miner. Do not stop a miner.

The miners-off control is a Friday step. It is not this test.

## Desk node

One TN10 kaspad is already running on this desk, testnet-10, UTXO index on, same read. Keep that one running. The monitor reads its sync and its mempool.

Do not start a second kaspad. Do not start a mainnet node.

Tonight's senders do not use this node. A sample uses public TN10 nodes only. Never n0. Never `bore.pub`. Never `159.223.110.159`.

## Spend

This file does not arm a spend. Spend only if stp's message in this session contains **rehearsal GO** and the clock is inside 18:30:00Z–18:45:00Z.

Storm GO does not arm tonight. `steps-utc.json` is for Friday. `fee2h` is not a GO. The halt file stays `halt`.

If rehearsal GO is missing, or it arrives after 18:45 UTC, keep the senders off, write the skip, and finish the monitor.

If the sample runs: target 62 tx/s for 15 minutes, then exit. 4 fixed senders. Depth 2. In-flight 48. 4 connections. Own coins. No auto-scale. No mempool pause inside the 15 minutes. Fee frozen at 200 and 300 sompi/gram, cap 600. At 18:30 UTC read the normal quote. If it is already above 200 on a node you will use, do not start. Ask.

## Report

Append the count rows to [tonight-8-oct/RESULTS.md](tonight-8-oct/RESULTS.md) and push that file. No ids in git. No key, no seed, no address.

- 18:00 UTC: session up, sender count, miner count, desk node synced or not, desk disk GB, NTP offset, usage remaining or not measured.
- Every 10 minutes through 20:00 UTC: the count row already named in the checkout paste.
- 19:40 UTC: start the Friday call table already in that file.
- 20:00 UTC: the stop line.

Desk disk GB is this PC. It is not the bot disk, and it is not the 35 GB line. That line is the bot's reading.

A checkout sample does not close the box dry run. The desk run at 734 tx/s does not close the n0 match. Those three stay on the bot's page.

## Clocks

Same clocks as the bot reset page.

Tonight stays 18:00–20:00 UTC. 20:00 UTC is the stop. If the desk is down at 18:00, write not measured and keep the senders off. Do not start a sender at 20:00.

Friday T0 stays 21:30 UTC. First load is 21:40 UTC. The storm ends Saturday 10 Oct 2026, 05:30 UTC. If that day is not ready, Monday 13 Oct 2026, 21:30 UTC, ending Tuesday 14 Oct 2026, 05:30 UTC.

Storm GO, the plan lock, and `steps-utc.json` stay with stp. The hours after 00:25 UTC stay unnamed.

## Last act

After the 20:00 stop line, write the two files named under **After 20:00 UTC** in [tonight-8-oct/PROMPT-BUILD.md](tonight-8-oct/PROMPT-BUILD.md). Then stop.
