> **Experimental. We are just trying this.**
>
> [Disclaimer](DISCLAIMER.md)

Wording, Kaspa Pulse (@gokugalax), 7 Oct 2026: sign-and-send processes are senders; runner is the setup; bot is reserved for the operator.

# Two nodes

9 Oct 2026. This page is the forward rule for every later send. The Thursday checkout files stay as they were.

**Goal.** The highest included tx/s the two sides can hold together. Submitted and accepted stay separate. The score for a minute is accepted on locus plus accepted on keel. Two nodes share one chain. They do not double the mass cap of about 3,024 included tx/s.

**Start.** Sending this GitHub to Grok Build or to the bot means go: start the operation.

## Names

Both kaspad processes are on this desk. Network `testnet-10`. UTXO index on. Neither name is a public DNS name.

| Name | Which process | Who uses it |
|---|---|---|
| **locus** | The first desk kaspad. Loopback Borsh. | Grok Build, on every step |
| **keel** | The second desk kaspad. The handoff still writes `node=desk-nodeB`. New logs use `keel`. On the desk, Borsh is `ws://127.0.0.1:17310` and gRPC is `127.0.0.1:16310`. | The bot's runner and the bot's miners, through the tunnel |

**n0 will not run.** n0 is the box kaspad. Do not start it, resync it, or keep disk aside for its pruning. The bot does not send through it, and the bot's miners do not mine on it.

**The bot.** The runner and the miners both use the tunnel stp provides to keel. The runner uses the tunnel's Borsh `ws://` address, only during the storm, and only while keel is synced and its tip lag is at or under 300 seconds. The miners use the tunnel's gRPC host and port. Coinbase pays the Grok Bot address `kaspatest:qzffl5xy9np46gkttyuftqnv2w04pr8g3wsp7c3vv8se3txtelx6q7c0v0ldx`. They mine only while keel is synced. Until the handoff lists that tunnel, the runner and the miners wait. Do not invent a host. From the box, do not use `127.0.0.1`. A short box disk stops the bot and does not stop Build.

**keel is in the score while it syncs.** Read at 2026-10-09T07:59:26Z: block download 69%, last block 2026-10-08T17:03:33Z, not synced, tunnels closed. For those minutes keel's accepted rate is 0 and the row says `waiting`. The combined rate is locus alone. Desk miners stay on locus until keel is synced. Do not point them at keel before that.

**Build.** Build keeps locus, on loopback Borsh, while locus is synced and the UTXO index is on.

| Who | Node | When it sends |
|---|---|---|
| The bot's runner | keel, through the tunnel | Only during the storm, and only while keel is synced and tip lag is at or under 300 seconds. Otherwise waiting. |
| The bot's miners | keel, through the tunnel | Only while keel is synced and the handoff lists the tunnel |
| Grok Build | locus | While locus is synced and the UTXO index is on |

**Monitoring.** While keel is not synced, the desk watches the block download and the tunnel stays closed. When keel is synced, the desk opens the tunnel, writes both addresses in the handoff, and says them. That report is not the storm GO. From T0 the sheet is [STP-KAS/tn10-locus](https://github.com/STP-KAS/tn10-locus) `plan/MONITOR.md`, and the checklist is `plan/NEXT-RUN-MONITOR.md`. The desk writes the combined row. The box prints its block. A missing required line is **not measured**. A waiting keel minute adds 0 and is not a failed match. If this page and `NEXT-STORM-PLAN.md` disagree on a clock, a fee, or a question, the questions plan wins. If they disagree on the node, this page wins.

`bore.pub` and `159.223.110.159` stay closed.

---

Intentions are good; thought process is questionable. STP remains delusional. Si vis pacem, para bellum.
