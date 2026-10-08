> **Experimental. We are just trying this.**
>
> [Disclaimer](../DISCLAIMER.md)

Wording, Kaspa Pulse (@gokugalax), 7 Oct 2026: sign-and-send processes are senders; runner is the setup; bot is reserved for the operator.

# Paste this into Grok Build at 19:50 local

Thursday 8 Oct 2026 checkout. Window **18:00:00Z–20:00:00Z** (20:00–22:00 local, CEST). Stop at 20:00 UTC.

This paste is the checkout. The Friday paste is the other file, `PROMPT-BUILD.md` at the repo root. If the clock is Friday, stop and use that file. The measurement plan wins if this paste disagrees with it: https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/NEXT-STORM-PLAN.md

## Clocks that are not this paste

Kaspa Pulse, 8 Oct 2026, read the checkout PDF. He called it solid. He counts **tonight 18:00–20:00 UTC**. That is this window. Do not redesign the PDF. Add the minute table below.

stp's DM the same morning named **20:00 UTC** as the aim for tonight's pre-test, after a desk resync, disk work, and usage limits. That sentence is not a new start. 20:00 UTC is the stop. A resync, a disk job, or a limit does not slide this window. If the desk is down at 18:00, write **not measured** and keep the senders off. Do not start a sender at 20:00 to meet the DM. His counter for tonight ends at 20:00. A send that starts then is outside it.

His line that the 9th works does not arm Friday. Friday stays the other file. A soft run is this checkout, not a second storm. Bot and Build together, at this size, is already the checkout. Do not add a mode.

7 Oct is closed on his word. Last submit 18:38:39 UTC. His window started 18:53. He counted the chain after the run. No conflict. Do not explain it. Do not call a figure a ceiling.

The five hours after 00:25 UTC are a Friday choice. Do not name them in this paste.

## Wait

Until 18:00:00Z, do not spend, do not launch a sender, and do not edit the public storm repo. Confirm three things in one reply, then wait:

1. You are on the desk, TN10 only, Build wallet only.
2. The older fleet halt file still says halt.
3. Sender count is the count you just read. The desk measure arm file may say `fee2h`. That line is not rehearsal GO and not storm GO. Do not start a sender from it.

## Words that arm a spend

Spend only if stp's message in this session contains **rehearsal GO** and the UTC clock is inside 18:30:00Z–18:45:00Z.

Storm GO does not arm this window. `steps-utc.json` is for Friday. Do not invent it. Do not lock the plan. Do not write the public result sections. Do not clear the halt file. Do not write a measure STOP file.

If rehearsal GO is missing, or it arrives after 18:45 UTC, keep the lane senders off, write the skip, and finish the monitor.

If Build usage is exhausted, do not spend. Write the counter, or **not measured**. Do not invent a later start.

## If the sample runs

- Target **62 tx/s** for 15 minutes, then exit.
- **4** fixed senders. Depth **2**. In-flight **48**. **4** connections. Each sender has its own coins. No auto-scale. No mempool pause inside the 15 minutes.
- Public TN10 nodes only. The desk node stays out of this sample, including while it resyncs. Never n0. Never `bore.pub`. Never `159.223.110.159`.
- Fee frozen at **200 and 300** sompi/gram, cap **600**. Half the lanes at each tier.
- At 18:30 UTC, read the normal quote. If it is already above 200 on a node you will use, do not start. Ask.
- One sender family. If a Build sender is already running, stop and ask.
- A sender started inside a short-lived shell dies with the shell. Keep the parent until 18:45 UTC.
- Desk miners stay as they are. Log the count at 18:00 UTC. Do not start or stop them.
- Per-transaction logs stay on. Times are UTC with milliseconds and `Z`.

Every UTC second, one line per sender: sender id, target tx/s, submitted tx/s, accepted tx/s, endpoint, named local pool, named public pools, submit-call latency. On a sample and on every reject, log submit time and accept time in the local log.

Every UTC minute of the sample, one local line per sender, on top of that per-second log. This is the 8 Oct ask, so his accepted count can sit beside our sent count:

- minute, `YYYY-MM-DDTHH:MM:00Z`
- sender id
- node: the public TN10 name that sender posted to. Not the word "public". Not n0. This side does not post to n0. If the endpoint is not one named public node, stop and ask.
- tx_sent: how many transactions that sender submitted in that minute
- five tx ids from that minute, spread across the minute, not the first five. Five is the reading of "a handful".

Accepted per second stays in the per-second log. His accepted figure is his. Do not invent it. Mempool is per node, so the node name is not optional.

Print no key, no seed, and no address. Do not print the id list in chat. One chat line per minute is enough: minute, sender, node, tx_sent, and the words "ids saved". The five ids go in the local log, and in the checkout PDF if this desk already writes that PDF. If it does not, write a local `checkout-minute.csv` with those columns. The ids do not go in git and they do not go in `tonight-8-oct/RESULTS.md`.

## Every 10 minutes, 18:00Z through 20:00Z

Append one row to `tonight-8-oct/RESULTS.md` in the private repo https://github.com/STP-KAS/grok-bot-build-combo and push that file. The row is: UTC, phase, session up, sender count, desk disk GB, NTP offset, usage remaining or **not measured**, submit tx/s, accepted tx/s, the six public mempools by name, desk mempool, indexer health, note.

The row stays a count row. Do not add tx ids to it.

When the bot prints a block, copy that block into the same file in the bot column. Push counts and times. Leave ids, keys, seeds, and addresses out.

At 19:40 UTC start the Friday call table already in that file. At 20:00 UTC write the stop line, push, and stop. Leave the halt file in place. Leave the public result sections empty.

Intentions are good; thought process is questionable. STP remains delusional. Si vis pacem, para bellum.
