> **Experimental. We are just trying this.**
>
> [Disclaimer](../DISCLAIMER.md)

Wording, Kaspa Pulse (@gokugalax), 7 Oct 2026: sign-and-send processes are senders; runner is the setup; bot is reserved for the operator.

# Paste this into Grok Build at 19:50 local

Thursday 8 Oct 2026 checkout. Window **18:00:00Z–20:00:00Z** (20:00–22:00 local, CEST). Stop at 20:00 UTC.

This paste is the checkout. The Friday paste is the other file, `PROMPT-BUILD.md` at the repo root. If the clock is Friday, stop and use that file. The measurement plan wins if this paste disagrees with it: https://github.com/STP-KAS/tn10-storm-throughput-questions/blob/main/plan/NEXT-STORM-PLAN.md

## Wait

Until 18:00:00Z, do not spend, do not launch a sender, and do not edit the public storm repo. Confirm three things in one reply, then wait:

1. You are on the desk, TN10 only, Build wallet only.
2. The older fleet halt file still says halt.
3. Sender count is the count you just read. The desk measure arm file may say `fee2h`. That line is not rehearsal GO and not storm GO. Do not start a sender from it.

## Words that arm a spend

Spend only if stp's message in this session contains **rehearsal GO** and the UTC clock is inside 18:30:00Z–18:45:00Z.

Storm GO does not arm this window. `steps-utc.json` is for Friday. Do not invent it. Do not lock the plan. Do not write the public result sections. Do not clear the halt file. Do not write a measure STOP file.

If rehearsal GO is missing, or it arrives after 18:45 UTC, keep the lane senders off, write the skip, and finish the monitor.

## If the sample runs

- Target **62 tx/s** for 15 minutes, then exit.
- **4** fixed senders. Depth **2**. In-flight **48**. **4** connections. Each sender has its own coins. No auto-scale. No mempool pause inside the 15 minutes.
- Public TN10 nodes only. The desk node stays out of this sample. Never n0. Never `bore.pub`. Never `159.223.110.159`.
- Fee frozen at **200 and 300** sompi/gram, cap **600**. Half the lanes at each tier.
- At 18:30 UTC, read the normal quote. If it is already above 200 on a node you will use, do not start. Ask.
- One sender family. If a Build sender is already running, stop and ask.
- A sender started inside a short-lived shell dies with the shell. Keep the parent until 18:45 UTC.
- Desk miners stay as they are. Log the count at 18:00 UTC. Do not start or stop them.
- Per-transaction logs stay on. Times are UTC with milliseconds and `Z`.

Every UTC second, one line per sender: sender id, target tx/s, submitted tx/s, accepted tx/s, endpoint, named local pool, named public pools, submit-call latency. On a sample and on every reject, log submit time and accept time in the local log.

Print no key, no seed, no address, and no txid.

## Every 10 minutes, 18:00Z through 20:00Z

Append one row to `tonight-8-oct/RESULTS.md` in the private repo https://github.com/STP-KAS/grok-bot-build-combo and push that file. The row is: UTC, phase, session up, sender count, desk disk GB, NTP offset, usage remaining or **not measured**, submit tx/s, accepted tx/s, the six public mempools by name, desk mempool, indexer health, note.

When the bot prints a block, copy that block into the same file in the bot column. Push counts and times. Leave ids, keys, seeds, and addresses out.

At 19:40 UTC start the Friday call table already in that file. At 20:00 UTC write the stop line, push, and stop. Leave the halt file in place. Leave the public result sections empty.

Intentions are good; thought process is questionable. STP remains delusional. Si vis pacem, para bellum.
