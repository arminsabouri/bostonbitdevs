+++
title = "Socratic Seminar 15"
date = 2023-04-20
aliases = ["socratic/2023/04/20/socratic-15.html"]
+++

## Housekeeping 🧹

- [What is a Socratic Seminar?](https://bitdevs.org/about#socratic-seminars)
- Questions are encouraged, including basic ones! Suggest topics for the next Socratic Seminar [here](https://github.com/arminsabouri/bostonbitdevs/issues/new).
- No photos, videos, or recordings.
- [Chatham House Rule](https://www.chathamhouse.org/about-us/chatham-house-rule): You are free to share discussions and learnings from Boston BitDevs, but do not reveal the source of the information. Do not share the identity of any of the speakers or participants.

## Bitcoin

Mark “Murch” Erhardt [Proposed BIP for transaction terminology](https://github.com/Xekyo/bips/pull/1)

### [MuSig2 spend to legacy p2pkh](https://twitter.com/Arminsdev/status/1645528304030457856)

MuSig2 is a multi-signature schnorr scheme. That means it can be encoded into a taproot address without revealing it's a multisig. Old school script multisig reveals that coins encumbered by the condition are certainly under multisig.

[It's a BIP now, too!](https://twitter.com/real_or_random/status/1640337134199640065)

### [Mempools around the world are full!](https://twitter.com/murchandamus/status/1639291486788255744)

### [Utreexo-powered Electrum Server](https://twitter.com/Erik17192799/status/1640831466085990400)

## Lightning

### BOLTs [#765](https://github.com/lightning/bolts/pull/765) adds route blinding to the LN specification

> Route blinding, which we first described in Newsletter #85, allows a node to receive a payment or onion message **without revealing its node identifier to the spender or sender**. No other directly identifiable information needs to be revealed. Route blinding works by having the receiver choose the last several hops over which the payment or message will be forwarded. These steps are onion encrypted like regular forwarding information and are provided to the spender or sender who uses them to send a payment to the first of the hops. That hop begins the process of decrypting the next hop, forwarding the payment to it, having that hop decrypt the subsequent hop, etc, until the receiver accepts the payment without their node being disclosed to the spender or sender. – bitcoinops.org

https://github.com/lightning/bolts/blob/3b814f0d031450a9cddd2718be7ed50c5444095b/proposals/route-blinding.md#introduction

### [Hierarchical Channels](https://github.com/DanGould/bostonbitdevs/pull/new/socratic-15)

Hierachical channels aim to do to lightning channel capacity what lightning channels did to bitcoin.

### Lightning Loop increases supply with P2TR Swap mode

[source](https://twitter.com/alexbosworth/status/1648352250161659905)

## Privacy

### [Your use of bitcoin is being spied on by Strangers](https://b10c.me/observations/06-linkinglion/?t)

>  The [so-called "LinkingLion"] entity ... listens to transaction announcements ... to link newly broadcast transactions to node IP addresses ... in some capacity since 2018 
> I suspect this entity is likely tracking transaction propagation to attempt to determine which node broadcasts which transaction to link transactions to IP addresses.

### [Wasabi claims 8,000 btc daily coinjoin volume (~$3 billion per month)](https://stats.wasabiwallet.io/search/43/from2023-03-19/to2023-04-19)

Only ~2% are "fresh" bitcoin.

## Research

### [Group Oblivious Message Retrieval](https://eprint.iacr.org/2023/534)

> Anonymous message delivery, as in private communication and privacy-preserving blockchain applications, ought to protect recipient metadata: a message should not be inadvertently linkable to its destination... For example, the servers' cost is $3.36 per million messages scanned, where each message may address up to 15 recipients.

### [Piano: Single-Server Private Information Retrieval with Sublinear Server Computation](https://twitter.com/BobMcElrath/status/1641106981816606723)

