> **Experimental. We are just trying this.**
>
> [Disclaimer](DISCLAIMER.md)

Wording, Kaspa Pulse (@gokugalax), 7 Oct 2026: sign-and-send processes are senders; runner is the setup; bot is reserved for the operator.

# Two nodes

8 Oct 2026, later. This page is the forward rule for every later send. The Thursday checkout files stay as they were.

**Goal.** The highest included tx/s the two sides can hold together. Submitted and accepted stay separate. The score is the sum of the two accepted rates. Two nodes share one chain. They do not double the mass cap of about 3,024 included tx/s.

**Start.** Sending this GitHub to Grok Build or to the bot means go: start the operation.

**The bot's runner.** It uses desk node B, the second kaspad on the desk. It runs only during the storm. Outside the storm it stays off. Network `testnet-10`. UTXO index on. On the desk the runner uses Borsh `ws://127.0.0.1:17310`. From the box it uses the node B tunnel in the desk handoff, and only after that handoff lists one. It sends only while node B is synced and its tip lag is at or under 300 seconds. A short box disk stops the bot and does not stop Build.

**Build.** Build keeps locus, the first desk kaspad, on loopback Borsh, while locus is synced and the UTXO index is on.

**Miners.** Point the miners at desk node B. On the desk that is gRPC `127.0.0.1:16310`. Coinbase pays the Grok Bot address `kaspatest:qzffl5xy9np46gkttyuftqnv2w04pr8g3wsp7c3vv8se3txtelx6q7c0v0ldx`. Mine only while node B is synced.

| Who | Node | When it sends |
|---|---|---|
| The bot's runner | desk node B | Only during the storm, and only while node B is synced and tip lag is at or under 300 seconds |
| Grok Build | locus, the first desk kaspad | While that node is synced and the UTXO index is on |

The monitoring tasks are in [STP-KAS/tn10-locus](https://github.com/STP-KAS/tn10-locus) `plan/MONITOR.md`. If this page and `NEXT-STORM-PLAN.md` disagree on a clock, a fee, or a question, the questions plan wins. If they disagree on the node, this page wins.

`bore.pub` and `159.223.110.159` stay closed.

---

Intentions are good; thought process is questionable. STP remains delusional. Si vis pacem, para bellum.
