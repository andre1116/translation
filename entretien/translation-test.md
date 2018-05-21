### Tendermint BFT Stack

Bitcoin is the intellectual ancestor of all blockchain-based cryptographic systems that we know and love today. The Tendermint protocol shares commonality with Bitcoin inasmuch as the two protocols record everything on a blockchain, yet they each provide their unique solutions to the Byzantine General’s Problem, also referred to as the consensus, or “agreement”, problem. Tendermint’s lineage is closely traced back to the world of distributed computing and Byzantine Fault Tolerance (BFT) literature in academia (e.g., see Ethan Buchman’s [thesis](https://atrium.lib.uoguelph.ca/xmlui/bitstream/handle/10214/9769/Buchman_Ethan_201606_MAsc.pdf)). Whereas in the Bitcoin genesis story, after the many failed attempts of previous electronic cash systems — with the exception of PayPal — Bitcoin rose above the ashes as a censorship-resistant decentralized currency system.

The Bitcoin protocol optimizes for censorship-resistance, critically, due to its primary function as a payment system. Tendermint, on the other hand, optimizes for general Byzantine fault-tolerant distributed applications and data processing amidst a wide area network (WAN), e.g. hundreds of nodes (high node count). This distinction is nuanced and merits deeper investigation.

For context, in the world of academia, there had been very little research done on BFT systems for WAN and only for a small number of nodes — 4 to 7 at maximum — and always for a single administrative domain. As for BFT systems for WAN with a large number of nodes and for multiple administrative domains, no significant body of work has been widely adopted in practice.

Before 2009, when Bitcoin introduced a paradigm-shifting technology — the concept of a blockchain — to the world, the consensus problem in a WAN setting for high node counts was left largely unanswered. Despite solving the Two Generals’ problem, however, Bitcoin was not really an algorithm to solve consensus, in the purely theoretical sense in the research area of distributed systems. Furthering the work in the BFT domain was far from done.

In 2014, Jae Kwon, coming from a computer science and systems engineering background, envisioned a purely BFT-based protocol which would scale to the tune of hundreds of nodes in the permissionless setting with Proof-of-Stake (PoS) as the underlying security mechanism. And so [Tendermint](https://tendermint.com/static/docs/tendermint.pdf) was created. Consequently, this system model designed with PoS as the primary security mechanism over a large number of validating nodes in a WAN turned out to be a significantly complex engineering endeavor, taking almost 4 years to implement in the public blockchain setting. That setting is Cosmos, slated to launch this summer in 2018.

Tendermint BFT 堆栈

比特币是我们今天所知道和喜爱的所有基于区块链的密码系统的智慧祖先。Tendermint协议与比特币具有共同性，因为两种协议都将区块链上的所有内容记录下来，但它们各自为拜占庭问题提供了独特的解决方案，也称为共识或“协议”问题。Tendermint的谱系密切追溯到学术界分布式计算和拜占庭容错（BFT）文献的世界（例如见Ethan Buchman的论文）。而在比特币创世的故事中，除了PayPal以前的电子现金系统失败的尝试之后，比特币超过了灰烬，成为审查抵制分散化的货币系统。

由于其作为支付系统的主要功能，比特币协议优化了审查阻力。另一方面，Tendermint优化了广域网（WAN）中的一般拜占庭容错分布式应用和数据处理，例如，数百个节点（高节点数）。这种区别是微妙的，值得深入研究。

从语境上看，在学术界，对广域网的BFT系统进行的研究很少，只有少量的节点（最多4到7个），并且始终用于单个管理域。至于具有大量节点和多个管理域的广域网的BFT系统，在实践中没有显著的工作体系被广泛采用。

在2009年之前，当比特币向世界推出了一种范式转换技术——区块链概念时，广域网设置中针对高节点数的共识问题在很大程度上得不到解决。然而，尽管解决了两位将军的问题，但在分布式系统研究领域的纯理论意义上，比特币并不是真正的解决共识的算法。进一步完善BFT领域的工作还远远没有完成。

2014年，来自计算机科学和系统工程背景的Jae Kwon设想了一种纯粹的基于BFT的协议，该协议可以在无需许可的情况下扩展到数百个节点，其中基于权益的证明（PoS）作为基础安全 机制。所以Tendermint成立了。因此，这种使用PoS作为广域网中大量验证节点主要安全机制的系统模型是一项非常复杂的工程设计工作，需要近4年时间才能在公共区块链设置中实施。这个设定是Cosmos，预定在2018年夏天推出。
