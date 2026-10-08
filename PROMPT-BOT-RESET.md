# Prompt bot reset

Paste this into the Grok bot on the box when usage resets on 8 Oct 2026. This file does not start the storm, does not lock the plan, and does not spend.

If this file disagrees with [NEXT-STORM-PLAN.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/NEXT-STORM-PLAN.md), stop and ask stp. The plan wins.

Wording, Kaspa Pulse (@gokugalax), 7 Oct 2026: sign-and-send processes are senders; runner is the setup; bot is reserved for the operator.

## Goal

The test is the heavy one already written. Full load. Full monitoring. It is not announced.

Not announced means do not post it, do not ping anyone, and leave the public result sections empty. The logs stay complete. A quiet test is not a smaller test, and it is not a thinner log.

Full load is the storm already written in the measurement plan and in this repo: paced steps through max, both sides, probes, the ordered stream, and the per-second logs. Friday 21:30 UTC, or Monday 13 Oct 21:30 UTC. Tonight stays the checkout size already written in [tonight-8-oct](tonight-8-oct/PLAN.md). This page does not start either one.

Full monitoring is the set already written: per-second submit and accept, per-transaction times, mempool by node name, disk, NTP, the n0 match, the saturation rule, mining share, probes at about 450 per tier per step, and the ordered stream. Five ids stay in the local log. On tonight's checkout, keep every monitor row that [tonight-8-oct](tonight-8-oct/MONITOR.md) already names. Drop none of them.

This page's job is to bring n0 back, synced, and report the three readings that run needs from this box.

1. Free GB on this disk. Read it before the resync. Read it again after n0 is synced.
2. The plan's box dry run, on this box, after n0 is synced.
3. The n0 match of the 6 Oct desk dry-run ids, 20:08–20:29 UTC. Write matched/total, or not measurable.

You know the work. Do that. Report the three. Then stop.

## Report

One line each, with UTC:

- free GB before the resync
- resync start
- n0 synced or not, lag in seconds, free GB after
- box dry run: done, or not done and why
- n0 match: matched/total, or not measurable
- usage left after the reset

The id list stays on the box. If that list is not on the box, the match is not measurable. If n0 no longer has those blocks, the match is not measurable. Ids stay out of git. No key, no seed, no address.

## Clocks

The usage reset is about 16:30 UTC. If it lands earlier or later, use the reset you get. Then resync n0.

Tonight stays 18:00–20:00 UTC. 20:00 UTC is the stop. If n0 is still unsynced at 18:00, write not measured and keep the senders off.

Friday T0 stays 21:30 UTC. First load is 21:40 UTC. The storm ends Saturday 10 Oct 2026, 05:30 UTC. If that day is not ready, Monday 13 Oct 2026, 21:30 UTC, ending Tuesday 14 Oct 2026, 05:30 UTC.

While n0 is unsynced, or more than 300 seconds behind, do not spend.

Keep about 19 GB free. At or under 19 GB, leave the resync off and tell stp. At least 35 GB free after the sync is the Friday go line. From 28 to 35 GB, Friday's steps shrink to 10 minutes. Below 28 GB, no storm.

A checkout sample does not close the box dry run. The desk run at 734 tx/s does not close the n0 match.

Storm GO, the plan lock, and `steps-utc.json` stay with stp. The hours after 00:25 UTC stay unnamed.
