> **Experimental. We are just trying this.**
>
> [Disclaimer](DISCLAIMER.md)

Wording, Kaspa Pulse (@gokugalax), 7 Oct 2026: sign-and-send processes are senders; runner is the setup; bot is reserved for the operator.

# Two nodes

8 Oct 2026, later. This page replaces the node column in the root table for every later send. The Thursday checkout files stay as they were.

**Goal.** The highest included tx/s the two sides can hold together. Submitted and accepted stay separate. The score is the sum of the two accepted rates. Two nodes share one chain. They do not double the mass cap of about 3,024 included tx/s.

| Who | Node | When it sends |
|---|---|---|
| TN10 ops | n0 | Only while n0 is synced and tip lag is at or under 300 seconds. Otherwise the senders stay off and the row says waiting. |
| Grok Build | its own node, locus, the desk kaspad | While that node is synced and the UTXO index is on. Loopback Borsh. |

The bot does not send to the desk. Build does not send to n0. A short box disk stops the bot and does not stop Build. The monitoring tasks are in [STP-KAS/tn10-locus](https://github.com/STP-KAS/tn10-locus) `plan/MONITOR.md`. If this page and `NEXT-STORM-PLAN.md` disagree on a clock, a fee, or a question, the questions plan wins. If they disagree on the node, this page wins.

This page does not give the storm GO and does not start a sender.

---

Intentions are good; thought process is questionable. STP remains delusional. Si vis pacem, para bellum.
