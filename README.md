# ZCLAIM - A Sapling-to-Sapling Bridge

Confidential Cross-Blockchain Exchanges: Designing a Privacy-Preserving Interoperability Scheme

---

This document describes the design of a private bridge based on Zcash's Sapling protocol. The protocol assumes an implementation of Sapling on some receiving smart-contract capable chain. Shielded Zcash can be sent with (informally) negligible information leak accross the bridge and back.

The work here was submitted as an external Master's thesis to ETH Zürich in collaboration with [Web3 Foundation](https://web3.foundation/). It was realised under the supervision of Martin Vechev and Petar Tsankov at ETH's [SRI Lab](https://www.sri.inf.ethz.ch/), and Fatemeh Shirazi and Alistair Stewart on the Web3 side (titles omitted).


### Abstract

Interoperability solutions for privacy-focused cryptocurrencies are hard to design: they must integrate with the unique privacy features of the underlying blockchain, itself often in active development, such as to trace specific payments in protocols designed to make payments untraceable. The required specialised research and development effort have resulted in a lack of such projects, despite the dependence on centralised exchanges for cross-chain transfers being particularly problematic for privacy-oriented cryptocurrencies.

In this work, we present Zclaim, an adaptation of the Xclaim framework for decentralised cross-chain exchanges to the privacy-protecting cryptocurrency Zcash. This is to the author’s knowledge the first project that succeeds in maintaining privacy in cross-chain transfers.

Zclaim integrates with the Sapling version of the Zcash protocol, implemented on a smart-contract capable issuing chain, in order to attain private cross-chain transfers. We provide an abstract protocol specification, defining new transfer types that fit into the existing Sapling transaction structure along with zk-SNARKs allowing protocol participants to prove statements about Zcash transactions in zero knowledge on the
issuing chain.

---

This work was summarised into a [paper](https://arxiv.org/abs/2204.10611) and published at [IEEE ICBC 2022](https://icbc2022.ieee-icbc.org/).
