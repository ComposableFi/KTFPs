
# Treasury loan for kick-starting money market activity on Kusama


* **KFTP Number:** [To be assigned once it's merged into the master]
* **Authors:** 0xbrainjar - 0xbrainjar@composable.finance
* **KSM Proposer:** [KSM Address of the Proposer]
* **KSM Receivers:** [Receiving KSM Address(es)]
* **Total Amount:** 17,243.00 KSM
* **Created:** [2021-12-13]

## Summary

Provide a $ 5 million KSM loan to lending protocols to kick-start the money market activity on the Kusama ecosystem


## Proposal

**Context**

Kusama needs a structured incentive program to attract customers and showcase its unlimited potential in scalability, efficiency, and cross-chain interoperability.
However, incentives should be wisely directed towards activities that, if adequately rewarded, create a positive feedback loop with a resulting exponential increase in liquidity gathered from outside. 
Lending is one of the essential pillars in a well-functioning DeFi ecosystem because it allows customers to capture opportunities without compromising capital efficiency. 

Other chains are skewing funds towards lending too. The Avalanche Rush program has allocated the highest incentive tranche to AAVE ($ 20 million). 
AAVE Total Value Locked (TVL) on the Avalanche chain has gone from $ 622 million to $ 3.46 billion in just two months. 
Benqi, the Avalanche native lending protocol, has obtained $ 10 million from the Avalanche Rush incentive program.
Its TVL has gone from $ 112 million at the Avalanche Rush announcement date to the current $ 1.85 billion.

**Problem Statement**

The lending activity on Kusama is currently anemic and, without lending/money market opportunities, there’s little room for onboarding foreign assets on the ecosystem. 
Projects like Angular Finance, an isolated lending pair pallet built on top of Composable Picasso, could help mitigate such a gap by enabling loans on Kusama.

**Proposal**

 Unlock $ 5 million KSM from the Kusama treasury in the form of a loan to Angular Finance or other lending projects aimed at kick-starting usage of DeFi applications. 

**The rationale behind the loan**

Whilst these incentive programs are common for other networks, we are aware that this is a new step for Kusama and we are therefore using this proposal to pursue a loan rather than direct liquidity incentives. We feel that this aligns incentives with the participating protocols, in order to use the loan as a proof of concept to illustrate the potential effectiveness of such a program going forward

**Treasury request**

The proposed loan size amounts to $ 5 million KSM for a duration of three months. At expiration date, protocols that received funds will pay the $ 5 million loan back to the Kusama treasury plus any earnings collected during the duration of the loan.

**Technical implementation**

The goal is for incentives to be transferred through a trustless mechanism that leverages XCM to send funds to specific projects' vaults. However, that's currently not possible since the XCM implementation is still in progress.

**Incentive allocation criteria**

The metrics used to determine the incentive allocation across lending protocols will take into account:

* Total Value Locked in the protocol not below $ 15 mln
* Number of protocol active users not below a certain threshold (to be defined)

**Success metrics**

The incentive program will be evaluated based on the 3-month increase in:

* Daily active accounts: success will be achieved with an increase of +100 average daily active users
* Transaction volume per daily active accounts: success will be achieved with an increase of + $ 5,000 transaction voluem per daily active account
* Total Value Locked: success will be achieved with an increase of + $ 100 mln in Total Value Locked 

**Profit projections**

Based on an aggregate incentives-eligible Total Value Locked of $ 80 mln, the incentive program will provide a 25% APR achieved through KSM incentives. Projects can provide additional incentives in the form of native tokens.

**Incentives APR**

The table below shows the expected evolution of success metrics and the related APR achievable through both Kusama and native incentives at an aggregate level

|                                                | As-is| Month 1| Month 2| Month 3|
|------------------------------------------------|-----:|-------:|-------:|-------:|
| Avg. daily active accounts                     |   638|     682|     726|     770|
| Avg. daily transaction volume   ($/mln)        |    27|      31|      36|      40|
| Avg. transaction volume per   active account   | 42470|   45955|   49018|   51731|
|                                                |      |        |        |        |
| TVL $ mln (incentive   recipient)              |    80|     126|     172|     218|
| Kusama incentives ($ mln)                      |      |    1.67|    1.67|    1.67|
| Native incentives ($ mln)                      |      |    0.33|    0.33|    0.33|
| Total incentives ($ mln)                       |      |    2.00|    2.00|    2.00|
|                                                |      |        |        |        |  
| APR on starting TVL (Kusama   incentives only) |      |     25%|     25%|     25%|
| APR on actual TVL (Kusama   incentives only)   |      |     16%|     12%|      9%|
|                                                |      |        |        |        | 
| Total APR on starting TVL                      |      |     30%|     30%|     30%|
| Total APR on actual TVL                        |      |     19%|     14%|     11%|

The allocation among project recipients in shown below (data in $ mln)

|                | Eligible TVL | Kusama incentives | Native incentives |
|----------------|-------------:|------------------:|------------------:|
| Basilisk       |         28.4 |               1.8 |               0.4 |
| Parallel Heiko |         21.9 |               1.4 |               0.3 |
| Altair         |         15.5 |               1.0 |               0.2 |
| Angular        |          9.0 |               0.6 |               0.1 |
| Genshiro       |          5.2 |               0.3 |               0.1 |
|                |              |                   |                   |
| Total          |         80.0 |               5.0 |               1.0 |


**Time horizon**

The duration of the program is 3 months. The program could be renewed at expiration in case one or more success metrics have not reached their targets.

**Default event**

In the event of default, protocols that received incentives from Kusama will repay the loan through their native tokens following the process explained in the "Technical implementation" subsection.

**Risks**

The main risks involved are related to protocol risk, oracle risk and code failures that could result in losses of customers' funds. 

**Contact Info**

0xbrainjar: 0xbrainjar@composable.finance

Github: https://github.com/ComposableFi/KTFPs/tree/master/Proposals
