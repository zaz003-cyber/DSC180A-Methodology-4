---
title: D35 Blockchain Project Reflections
---

**Zihan Zhang** · [zaz003@ucsd.edu](mailto:zaz003@ucsd.edu)  
**Section:** D35 Blockchain · **Mentor:** Rajesh Gupta

**What topic in our domain interested me most this quarter?**

I was most interested in how a verifier can tell whether a credential is still valid. A document hash lets a verifier check that a document matches the registered record, but the verifier must also check who issued the credential and whether it has been revoked. The Vera project gave me a concrete way to see how those checks fit together.

**What could I investigate for my Quarter 2 project?**

I would compare a smart contract registry with a signed credential and a conventional status endpoint. With synthetic credentials, I would test valid, revoked, and mismatched documents, then measure how quickly each approach verifies them and how quickly a revocation becomes visible. I would also compare what each approach requires the verifier to trust.

**What would I change in our Quarter 1 approach?**

I would add an end-to-end scenario that issues a degree, links a self-reported credential to it, revokes the degree, and checks what the verifier reports for both records. This would test the behavior across the contracts and make it easier to spot cases where a stored link remains present after a credential is no longer valid.

**What other techniques would I like to try?**

I would try property-based tests for issuer permissions and revocation, and use repeatable testnet runs to measure gas usage and verification latency. I would also explore whether signed off-chain records could reduce the amount of information that has to be publicly linked to a wallet.
