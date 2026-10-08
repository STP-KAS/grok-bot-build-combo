> **Experimental. We are just trying this.**
>
> [Disclaimer](../DISCLAIMER.md)

Wording, Kaspa Pulse (@gokugalax), 7 Oct 2026: sign-and-send processes are senders; runner is the setup; bot is reserved for the operator.

# Kaspa Pulse, his input

Kaspa Pulse ([@gokugalax](https://x.com/gokugalax)), X DM, 4–7 Oct 2026. TN10 only. He stays out of the setup. He counts the chain on his side and sends the comparison first. We stay credited.

The public write-up is [plan/PULSE-README.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/PULSE-README.md) and [plan/PULSE-WINDOW-7-OCT.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/PULSE-WINDOW-7-OCT.md). The measurement plan is [plan/NEXT-STORM-PLAN.md](https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/NEXT-STORM-PLAN.md). If this page and the plan disagree, the plan wins.

This page is his input as already given. It is not a new question to him. The wording line above is the 7 Oct 2026, 19:54 UTC correction, and it is not asked again.

## What he is measuring

1. Accepted tx/s against submitted, over the whole storm, and where acceptance flattens.
2. Confirmation time at each load step, median and worst, normal fee against 1.5×. Does paying 1.5× buy inclusion.
3. Indexer freeze: at what sustained tx/s, and for how long.
4. Mempool depth over time. Backlog, not only throughput.
5. Whether order holds under load. Sent order against accepted order. Headline tx/s is not the metric.

The two headlines he is set up for are order under load, and whether 1.5× fee buys inclusion while 1× waits.

## How he asked for the run to be built

1. Write the plan first. Publish it with the results. Cite the commit SHA. List deviations.
2. Baseline first. Ten minutes of normal traffic, same measurements, then the steps.
3. Fixed steps, not one blast. His example was 1×, 2×, 5×, 10×. The plan's table is a 10-minute baseline, then 2×, 5×, 10×, 20×, 30×, then max. The plan wins on that table.
4. Log submitted and accepted per second, UTC. Log send order against accept order.
5. State mining share up front. Storm 2 measured about 50–63% of TN10 blocks. He had put the share near 60% of TN10 hashrate. The result says which figure it uses. It is TN10 with our miners on.
6. Raw data next to the summary.

## Four tightenings, before the lock

1. Miners-off is in the main run, at low load, matched to the same load with miners on. The control is imperfect. Other miners still change templates. Say that next to the pair.
2. Separate the box from the chain. When accepted flattens, log n0 CPU, mempool-cap hits, and reject reasons. Label the plateau box-bound or network-bound, or leave it unclear.
3. Sync the clocks. NTP on the box and on the desk. Log the offset at the start and at the end. Correct confirmation times, or flag them.
4. Saturation defined before T0: accepted under 95% of submitted for 60 seconds. Reorder rates as counts and percentages, with n. About 90 probes per tier is thin. The plan raised that to about 450 per tier per step.

## Cadence, 7 Oct 2026

One clean run first. Go through the numbers. Then weekly. Do not stack runs before that.

The clean run is Friday 9 Oct 2026, 21:30 UTC, for 8 hours, ending Saturday 10 Oct 2026, 05:30 UTC. If that day is not ready, Monday 13 Oct 2026, 21:30 UTC, for 8 hours. Ping him after that run. Tonight is the checkout in front of it, not the clean run, and not a weekly repeat.

## 7 Oct compare, still open

He asked to line up one window before anyone treats a lower chain count, or the 2,750 figure with a pool near 9.7k, as a ceiling. He wanted start, end, target tx/s, sent against accepted, which node, and sample ids.

Our log does not cover 18:52–19:23 UTC. The last submit is 18:38:39 UTC. The included_s sum 2,753 is 15:20:32 UTC. Mempool 9747 is 15:25:33 UTC. Those are not one minute. The pool name on the 9747 line is missing. Tonight does not invent that window, and it does not call either figure a ceiling.

His side counts the chain only. Nothing in this checkout touches his counter.

## What tonight owes that input

Friday's clean run can be read by him only if the logger actually emits the fields. Tonight's sample, when it runs, is the proof of the logger: per-second submitted and accepted, named pools, latency, NTP at both ends, and a match count on n0. The sheet is [MONITOR.md](MONITOR.md).

Tonight also keeps his cadence. The sample is 15 minutes, under a 250 tx/s cap, with miners left as they are. It is not a second storm.

## Later note

Blank, for a note from him if one arrives before Friday. Nothing is written here until then.

Intentions are good; thought process is questionable. STP remains delusional. Si vis pacem, para bellum.
