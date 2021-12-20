
# Treasury loan for kick-starting money market activity on Kusama


* **KFTP Number:** [To be assigned once it's merged into the master]
* **Authors:** 0xbrainjar - 0xbrainjar@composable.finance
* **KSM Proposer:** [KSM Address of the Proposer]
* **KSM Receivers:** [Receiving KSM Address(es)]
* **Total Amount:** 17,243.00 KSM
* **Created:** [2021-12-13]

## Summary

Provide a $ 5 million KSM loan to lending protocols to kick-start the money market activity on the Kusama ecosystem.


## Proposal

**Context**

Kusama needs a structured incentive program to attract customers and showcase its unlimited scalability, efficiency, and cross-chain interoperability potential.
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

While these incentive programs are standard for other networks, we know that this is a new step for Kusama. Therefore, we use this proposal to pursue a loan rather than direct liquidity incentives. We feel that this aligns incentives with the participating protocols to use the loan as a proof of concept to illustrate the potential effectiveness of such a program in the future.

**Treasury request**

The proposed loan size amounts to $ 5 million KSM for three months. At the expiration date, protocols that receive funds will pay the $ 5 million loan back to the Kusama treasury plus any earnings collected during the loan duration.

**Technical implementation**

The deployment of funds should be explicit, and voted on a per-allocation request, completely executable through extrinsics.

The goal is to transfer incentives through a trustless mechanism that leverages XCM to send funds to specific chains. Each chain requesting an allocation must be reachable over XCMP and offer means for the treasury to manage these funds over XCMP.

It is understood that XCMP has not fully matured yet. Teams wishing to request an allocation will need to spend considerable engineering effort to ensure that the previous requirements can be met.

**Incentive allocation criteria**

The metrics used to determine the incentive allocation across lending protocols will take into account:

* Total Value Locked in the protocol, not below $ 15 mln
* Number of protocol active users not below a certain threshold (to be defined)

**Success metrics**

The incentive program will be evaluated based on the 3-month increase in:

* Daily active accounts: success will be achieved with an increase of +100 average daily active users
* Transaction volume per daily active accounts: success will be achieved with an increase of + $ 5,000 transaction volume per daily active account
* Total Value Locked: success will be achieved with an increase of + $ 100 mln in Total Value Locked 

**Profit projections**

Based on an aggregate incentives-eligible Total Value Locked of $ 80 mln, the incentive program will provide a 25% APR achieved through KSM incentives. Projects can provide additional incentives in the form of native tokens.

**Incentives APR**

The table below shows the expected evolution of success metrics and the related APR achievable through both Kusama and native incentives at an aggregate level:

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

The allocation among project recipients is shown below (data for illustration purpose only, $ mln):

|                | Eligible TVL | Kusama incentives | Native incentives |
|----------------|-------------:|------------------:|------------------:|
| Protocol 1     |           16 |                 1 |               0.2 |
| Protocol 2     |           16 |                 1 |               0.2 |
| Protocol 3     |           16 |                 1 |               0.2 |
| Protocol 4     |           16 |                 1 |               0.2 |
| Protocol 5     |           16 |                 1 |               0.2 |
|                |              |                   |                   |
| Total          |           80 |                 5 |                 1 |


**Time horizon**

The duration of the program is three months. The program could be renewed at expiration if one or more success metrics have not reached their targets.

**Repayment**

In the event of default, protocols that received incentives from Kusama will repay the loan through their native tokens following the process explained in the "Technical implementation" subsection.

**Risks**

The main risks involved are protocol risk, oracle risk, and code failures that could result in losses of customers' funds. 

**Contact Info**

0xbrainjar: 0xbrainjar@composable.finance

Github: https://github.com/ComposableFi/KTFPs/tree/master/Proposals
