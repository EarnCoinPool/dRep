
### Governance Action Type:
Parameters

### Title:
Increase K (stakePoolTargetNum) from 500 to 1,000

### Abstract:
This parameter governance action seeks to increase the K parameter (stakePoolTargetNum) from 500 to 1,000 to increase decentralization, improve the economic stability of more stake pools by encouraging ada holders to delegate to a wider number of pools.

**NOTE:** The Constitution refers to the K parameter as stakePoolTargetNum, they are synonymous for each other. Since all the research, PCPs and past documentation refers to the parameter as K we will use the term K parameter from here on out, but K is interchangeable with term stakePoolTargetNum parameter.[^1]

[^1]:"stakePoolTargetNum (k parameter)" [https://docs.cardano.org/about-cardano/explore-more/parameter-guide](https://docs.cardano.org/about-cardano/explore-more/parameter-guide)

### Motivation 
The K parameter is ID’d as the parameter central to decentralization and as such is used to tune decentralization. Cardano experts are generally understood to believe that the design premise of K is sound and the research that justifies it is well-understood and correct. "the increase of k does trigger a substantial increase in the Nakamoto coefficient, confirming that a change in k can aid in boosting the decentralisation of the system."[^12]

[^12]: "the increase of k does trigger a substantial increase in the Nakamoto coefficient, confirming that a change in k can aid in boosting the decentralisation of the system." [https://blogs.ed.ac.uk/blockchain/2022/04/19/pool-splitting-behaviour-and-equilibrium-properties-in-cardano-rewards-scheme/](https://blogs.ed.ac.uk/blockchain/2022/04/19/pool-splitting-behaviour-and-equilibrium-properties-in-cardano-rewards-scheme/)

The Cardano Foundation on the K Parameter - “The k-parameter plays an important factor in keeping the Cardano blockchain adequately decentralized and encourages ada holders to delegate to a wider number of pools.”[^2] IOHK on the K Parameter - “The system . . . [through increases in K] incentivizes delegators to move their stake to a pool containing less ada, in order to maintain their yield and thus encourages the decentralization of the network.”[^3]

[^2]: "What is a k-parameter? The k-parameter determines the stake pool saturation point, ‘k’, which governs the rewards stake pools receive according to how much stake is delegated to them. The k-parameter plays an important factor in keeping the Cardano blockchain adequately decentralized and encourages ada holders to delegate to a wider number of pools." [https://medium.com/cardanorss/cardano-foundation-to-adjust-its-delegation-methodology-following-changes-to-the-k-parameter-7636ffb8e82](https://medium.com/cardanorss/cardano-foundation-to-adjust-its-delegation-methodology-following-changes-to-the-k-parameter-7636ffb8e82)
[^3]: "The system thereby incentivizes delegators to move their stake to a pool containing less ada, in order to maintain their yield and thus encourages the decentralization of the network." [https://iohk.io/en/blog/posts/2022/10/27/staking-parameters-and-network-optimization-where-next-for-k-and-min-fee/](https://iohk.io/en/blog/posts/2022/10/27/staking-parameters-and-network-optimization-where-next-for-k-and-min-fee/)

Recent analysis shows minimum attack vector slowly decreasing and large pools minting majority of the blocks while 44% minted 10 or less blocks. The most current research shows it's safe to move to K=1,000 and by moving K to 1,000 it would lead to just about doubling our Nakamoto coefficient.[^4]

[^4]:Nakamoto coefficient for K=500 is 116, expected at K=1,000 is 226 [https://blogs.ed.ac.uk/blockchain/2022/04/19/pool-splitting-behaviour-and-equilibrium-properties-in-cardano-rewards-scheme/](https://blogs.ed.ac.uk/blockchain/2022/04/19/pool-splitting-behaviour-and-equilibrium-properties-in-cardano-rewards-scheme/)



### Rationale
**Note:** The choice to incorporate quotations within the Governance Action and the Rationale section was made deliberately. This approach serves a dual purpose: it highlights points that have already been articulated and reinforces them with established research findings. By referencing what has previously been stated and previous research, the Rationale demonstrates that it is evidence-based. This is done to clearly communicate that the reasoning presented is not speculative but is grounded in academic work. This approach also shifts the responsibility to those who disagree with the research cited. They are now tasked with providing their own research to challenge or counter the established findings, rather than simply expressing disagreement without supporting evidence.

The K parameter was already changed once from 150 to 500 in December of 2020. The same rationale and justification given then is the same for moving K to 1,000. As IOG stated when the decision was made to increase K from 150 to 500:

"Central to the health of Cardano as a vibrant proof-of-stake network is the manner in which delegators and stake operators are rewarded for running it, and how those rewards are shared to maximize decentralization and secure the network."[^5]

"In the longer term, the system can be successful only if it is widely decentralized. Philosophically, the design of the rewards scheme aims to encourage a wide and diverse set of stake pool operators. This secures the platform against attacks, spreads any available rewards evenly across the community, and makes the system more resilient to change."[^5]

"Many economic systems have a tendency towards consolidation and a smaller number of strong players. On the other hand, blockchains can only be successful when control is decentralized. The rewards-sharing scheme ensures that smaller and medium pools can contribute meaningfully to the ecosystem without becoming subsumed into larger operators and consortia, as has happened with other blockchain systems, particularly Bitcoin."[^5]

"One way to discourage a trend towards a few large pools that collectively control the system is to introduce a counter-incentive to a pool's growth. The rewards-sharing scheme we designed is an example of this novel (in the cryptocurrency space) concept. As soon as stake delegation to a single pool increases above a threshold, the rewards automatically diminish, encouraging ada holders delegating to that pool to find a new home to improve their rewards. This mechanism limits the delegation that can be rationally made to any pool and spreads delegated stake more evenly across a larger number of pools."[^5]

"The move to k=500 will give small- to medium-sized pools that are struggling an improved opportunity to attract delegation. It will also have the effect of limiting pool size to 64 million ada, which means more than 100 of the largest pools will become saturated."[^5]

"Modeling the long-term viability of stake pools, we found that k values of 1,000 were stable in the long term. As a result, our aim is to move to k=1,000 during March 2021. We recognize the importance of economic factors that also strongly influence pool profitability and will continue to consult widely with the community on the plan"[^5]

"We recognize that in the short term, the move to k=500 will mean significant change for some. If delegators to larger pools do not react, some pools will become oversaturated and rewards will be unclaimed (note that no rewards are lost; everything goes back to the system’s reserves for the community to draw upon in the future). As a result, pool operators will need to adjust their margin and cost in the short term to stay profitable and incentivize delegators to take action. While this will require some effort from the community, it is an essential step for the Cardano ecosystem to maximize its decentralization."[^5]

"The increase in k will be a significant step forward in delivering Cardano’s mission."[^5]

"Achieving the highest level of decentralization is the ultimate objective of any blockchain system. Decentralization is the solid foundation over which the Cardano ecosystem will thrive."[^5]

[^5]: [https://iohk.io/en/blog/posts/2020/11/05/parameters-and-decentralization-the-way-ahead/](https://iohk.io/en/blog/posts/2020/11/05/parameters-and-decentralization-the-way-ahead/)

#### What is K and how does it work?
The K parameter creates a soft cap on the total stake in a pool that would receive optimal rewards. This number is often referred to as the saturation level. The cap or saturation level changes over time and is defined as a percentage of the maximum supply of ada (45bn) minus any amount that remains in the reserve (as of epoch 590, Reserve: 6,808,177,356) so that would equal 38,191,822,644 ada.

The current saturation level:  
Maximum pool size = (45bn - 6,808,177,356 in reserves) / k = (38,191,822,644 / 500 ) = 76,383,645.288  

For readability we will use approximate amounts, so approximately:  
***Maximum pool size = (45bn - 7bn in reserves) / k = (38bn / 500 ) = 76 million***

"Within the Cardano documentation, a pool that reaches its maximum size is said to be saturated. A saturated pool offers the highest rewards to delegators and is most lucrative for its operators, while an over-saturated pool delivers lower rewards. The system thereby incentivizes delegators to move their stake to a pool containing less ada, in order to maintain their yield and thus encourages the decentralization of the network."[^3]

Adjusting K parameter to 1,000 would set the saturation level to the following approximate level:  
***Maximum pool size = (45bn -  7bn in reserves) / k = (38bn / 1000 ) = 38 million***  

The move to K=1,000 with a saturation level around 38 million ada will, as stated above by IOHK will incentivize delegators to move their stake to a stake pool containing less ada, so they can maintain their rewards, thus encouraging wider decentralization of the Cardano network.[^3]

#### Is it safe to move K to 1,000 and why moving in one big move is recommended by IOG Scientist
IOG has stated:

"It is worth noting that the k-parameter is not amenable to small, gradual increases."[^5] and "Therefore, the best strategy for an upwards adjustment of k is to move in larger, less frequent increments – and to move it as far and as fast as practical network dynamics and economics will allow."[^5]

The last time K was adjusted it went from 150 to 500 and then the recommendation from IOG was to go to 1,000. The current research looked at 750 vs 1,000 and showed 1,000 would be most effective with a projection of almost doubling our Nakamoto coefficient. While K=750 would have minimal impact[^4]

IOG research has said it is safe to increase K to 1,000 on several post indicating that it's safe both for the security and economics. 

From IOG:

"Modeling the long-term viability of stake pools, we found that k values of 1,000 were stable in the long term. As a result, our aim is to move to k=1,000 during March 2021. We recognize the importance of economic factors that also strongly influence pool profitability and will continue to consult widely with the community on the plan; the social dynamics of the network should also not be underestimated."[^5] and "Previously, IOG had suggested that this value could be safely raised to 1,000"[^3]


#### History of Announcements and Steps to get K Parameter Increased to 1,000
The Shelley/Decentralization phase of the roadmap included K being set to 1,000 stake pools.[^7] It was announced that K would be increased in March 2021 to 1,000[^8] However due Alonzo hard fork and the deployment of the full Goguen smart contract this was delayed.[^9] 

After the delay, IOG then sent several surveys and had several discussions with the SPOs over the next year or two. In May 2023 a mainnet poll was conducted. At first SPOs were told it was just on K but then as the poll date neared, min pool fee was added. The mainnet poll took place in epochs 412-415 in May 2023 with the results supporting the option to Increase K to 1,000 and halve minPoolCost to 170 ada. AdaStat.net shows the voting results using 5 metrics. K=1,000 and min fee of 170 won the poll using each of the 5 metrics.[^6]

However, the Parameters Committee decided to just adjust min pool fee and then "watch metrics" before adjusting K. The SPO community was then told there was a new process and if we wanted to adjust K, using newly formed Parameters Committee Proposal (PCP) which would need to be submitted via Cardano forum and an official document. 

October 2023 Earn Coin Pool submitted a K-PCP. The K-PCP was not taken up by the committee and PCP authors were notified that current PCP would need to resubmit to be considered in the next window.

In May 2024 Earn Coin Pool submitted a Position to Resubmit the K-PCP. The Parameters Committee did not take up the PCP and did not issue a regular PCP result but issued a comment on this discussion of the K parameter to support the community endeavor.

Now it's up to the community to submit a parameter governance proposal.

[^6]: [https://forum.cardano.org/t/pcp-k-parameter-earncoinpool/122701](https://forum.cardano.org/t/pcp-k-parameter-earncoinpool/1227010
[^7]: "Come the end of the Shelley era, we expect Cardano to be 50-100 times more decentralized than other large blockchain networks, with the incentives scheme designed to reach equilibrium around 1,000 stake pools." [https://roadmap.cardano.org/en/shelley/](https://roadmap.cardano.org/en/shelley/)
[^8]: "Modeling the long-term viability of stake pools, we found that k values of 1,000 were stable in the long term. As a result, our aim is to move to k=1,000 during March 2021." [https://iohk.io/en/blog/posts/2020/11/05/parameters-and-decentralization-the-way-ahead/](https://iohk.io/en/blog/posts/2020/11/05/parameters-and-decentralization-the-way-ahead/)
[^9]: "K will not change in Q3. Our focus is on a successful Alonzo hard fork and the deployment of the full Goguen smart contract capability. We have also clearly stated elements like multi-pool delegation get put in place as we reopen the consultation on K and other parameters."[https://x.com/timbharrison/status/1399657898364518401](https://x.com/timbharrison/status/1399657898364518401)

## Precedent: K was already increased to 500

### Constitutional Alignment
The Constitution states that: Target Number of Stake Pools (stakePoolTargetNum) is "Primarily a security parameter, ensuring decentralization by stake pool division/replication"[^17] 

The guardrails for Target Number of Stake Pools (stakePoolTargetNum) states that it must not be lower than 250 and must not exceed 2,000 and must not be negative or zero.(Appendix I, Section 2.4)[^18] Setting Target Number of Stake Pools (stakePoolTargetNum) to 1,000 aligns with the Constitution.

The Constitution also states that K or Target Number of Stake Pools (stakePoolTargetNum) has an economic effect as well as a security effect.

According to the Cardano Constitution one of the overall goals of Economic parameters is to: "Ensure that stake pools are adequately rewarded for maintaining the Cardano Blockchain"[^13] (Appendix I, Section 2.2: #2) According to the Constitution one Core Metric for Economic Parameters is the "Number and health of stake pools"[^14] (Appendix I, Section 2.2: Core Metrics)

Increasing K or Target Number of Stake Pools (stakePoolTargetNum) would align and satisfy both, the goal and the Core Metric. Meaning increasing K would lead to more pools being "adequately rewarded for maintaining the Cardano Blockchain".

[^17]: "Primarily a security parameter, ensuring decentralization by stake pool division/replication" [https://github.com/IntersectMBO/cardano-constitution/blob/main/cardano-constitution-1/cardano-constitution-1.txt.md#target-number-of-stake-pools-stakepooltargetnum](https://github.com/IntersectMBO/cardano-constitution/blob/main/cardano-constitution-1/cardano-constitution-1.txt.md#target-number-of-stake-pools-stakepooltargetnum)

[^18]: Appendix I, 2.4. Technical/Security Parameters [https://github.com/IntersectMBO/cardano-constitution/blob/main/cardano-constitution-1/cardano-constitution-1.txt.md#24-technicalsecurity-parameters](https://github.com/IntersectMBO/cardano-constitution/blob/main/cardano-constitution-1/cardano-constitution-1.txt.md#24-technicalsecurity-parameters)

### Technical Review / Expected Impact
"From IOG’s calculations, there are about 100 public pools that would be affected by a move to k=1,000, representing around 2bn ada that would need to be redelegated (8% of the supply)."[^3] It also important to note that exchanges like Binance have already setup their pools to be below the K=1,000 saturation cap.[^10] indicating they are willing and ready for K=1,000.

The most recent technical review done in April 2022 by Christina Ovezik & Aggelos Kiayias which took in to account pool splitting and "emulate(s) the current Cardano stakeholder distribution, using a combination of real data points (taken from ADApools and PoolTool) and synthetic points that we draw from a Pareto distribution"[^4] found that: "As expected, the values of the Nakamoto coefficient diverge more from the ideal ones, but the increase in k still helps to achieve a higher degree of decentralisation."[^4] and "Note that the final number of pools was also lower than k in these observations, which can be attributed to the decrease in the system’s active stake."[^4] This research showed adjusting "...k can drive the system towards a more decentralised state, as measured by its Nakamoto coefficient."[^4] It also compared K=750 vs K=1,000 with the current conditions including pool splitting and demonstrated the K=1,000 almost would double our Nakamoto coefficient while K=750 would have minimal impact. This again confirms earlier research that moving K as far and as fast as possible is best method for adjusting K.

[^10]: [https://pool.pm/search/bnp](https://pool.pm/search/bnp)


### Economic impact
It's important to note SPOs are paid through two variables; Min pool fix fee and margin. The min pool fix fee can be set as low as 170 ADA. The min pool fix fee is paid only once per epoch to a pool that mints a block. Another way to think of min pool fix fee is a tax on the first block of the epoch. Since all pools that would be affected by a decrease in the saturation cap due to an increase in K are minting blocks each epoch and would be after an increase in K, this variable is irrelevant in any economic impact assessment as the would receive the same ADA in fix fee before and after K increase. This leaves only pools above 35 million in delegation and a non-0% margin to consider in analysis.

According to the Cardano Constitution one of the overall goals of Economic parameters is to: "Ensure that stake pools are adequately rewarded for maintaining the Cardano Blockchain"[^13] (Appendix I, Section 2.2: #2) According to the Constitution one Core Metric for Economic Parameters is the "Number and health of stake pools"[^14] (Appendix I, Section 2.2: Core Metrics)

[^13]: "Ensure that stake pools are adequately rewarded for maintaining the Cardano Blockchain" [https://github.com/IntersectMBO/cardano-constitution/blob/main/cardano-constitution-1/cardano-constitution-1.txt.md#22-economic-parameters](https://github.com/IntersectMBO/cardano-constitution/blob/main/cardano-constitution-1/cardano-constitution-1.txt.md#22-economic-parameters)

[^14]: "Number and health of stake pools" [https://github.com/IntersectMBO/cardano-constitution/blob/main/cardano-constitution-1/cardano-constitution-1.txt.md#core-metrics](https://github.com/IntersectMBO/cardano-constitution/blob/main/cardano-constitution-1/cardano-constitution-1.txt.md#core-metrics)

Increasing K would satisfy both of these, the goal and the Core Metric. We would expect to see more healthy pools and more pools adequately rewarded. Analysis shows that of the 100 pools that would be affected by the change of K to 1,000 only about 22 pools have a non - 0% margin. Meaning only 22 pools would receive less income in the form of margin per block. Each of these pools would need to increase margin to maintain current amount of earnings per epoch.

**Network Cost Argument:**
While some have argued there will be a network cost as some pools will split and spin up new pools. It's important to note that those who split pools and spin up more pools are subverting the K parameter which is meant to set a cap on the ADA staked to one entity. So having increased infrastructure cost to those who look to split could be seen a deterrent to subverting the K parameter.

**Cost of ADA:**
The last time we adjusted K to 500 on December 6th 2020 the price of ADA was $0.15[^15] While the current cost as of 10/23/2025 is $0.64

[^15]: Price of ADA 12/06/2020 [https://finance.yahoo.com/quote/ADA-USD/history/?period1=1607212800&period2=1607212800](https://finance.yahoo.com/quote/ADA-USD/history/?period1=1607212800&period2=1607212800)

**Note on Exchanges:**
An analysis of the two biggest exchanges Coinbase and Binance show that Binance have already setup their pools to be below the K=1,000 saturation cap.[^10] indicating they are willing and ready for K=1,000. While Coinbase currently has 29 pools of which only 17 would be above the new 35 million saturation cap at K=1,000. About 13 new pools may result if Coinbase splits it pools. It also important to note that enterprise addresses[^16] were created so that exchanges didn't participate in staking. These exchanges carry cryptocurrencies in which they can't or don't run their own staking pools for.

[^16]: "Exchanges or other organizations that control large amounts of ada – but hold it on behalf of other users – may wish to follow a policy of not exercising stake rights. By using enterprise addresses, exchanges can demonstrate that they follow this policy." [https://docs.cardano.org/about-cardano/learn/cardano-addresses#enterprise-addresses](https://docs.cardano.org/about-cardano/learn/cardano-addresses#enterprise-addresses)

### Product Committee 2025 Roadmap Supporting Changes

The Product Committee 2025 roadmap includes: 
* Introduce min-margin parameter that can be voted on via governance to modify[^11]
* Modify pledge-benefit curve for a0[^11]

The 2025 roadmap includes two items that many believe with further help a change to K be more effective. Replacing min pool fee with a min margin and a0 adjustments, making pledge move effective. These two changes could further lead to better than the project results of doubling our Nakamoto coefficient.

[^11]: Product Committee: 2025 Proposed Cardano Roadmap [https://productcommittee.docs.intersectmbo.org/committee-outcomes/2025-cardanos-roadmap/2025-proposed-cardano-roadmap](https://productcommittee.docs.intersectmbo.org/committee-outcomes/2025-cardanos-roadmap/2025-proposed-cardano-roadmap)

### Reversion/Recovery Plan
A reversion/recovery plan should not be necessary as the K parameters have been changed in the past and the effects are known. However, in case of a disaster recovery the K parameter can/would be set back to 500 if a reverting change was necessary due to either a Severity 1 or Severity 2 incident or issue. If a Severity 3 incident or issue the K parameter can/would be set back to 750 for further monitoring. If at K=750 and the Severity increased to the 1 or 2 level, the K parameter would be set back to 500. No other actions would need to be taken to restore the network. Under Appendix I, Section 1 there are 3 Severity Levels classified; Severity 1 is a critical incident or issue, Severity 2 is a major incident or issue, and Severity 3 is a minor incident or issue.

### References and Supporting Information

* K- PCP submitted by Earn Coin Pool 
https://forum.cardano.org/t/pcp-k-parameter-earncoinpool/122701

* Position to Resubmit the K-PCP by Earn Coin Pool
https://forum.cardano.org/t/pcp-k-parameter-earncoinpool/122701/98

* Shelley Roadmap
https://roadmap.cardano.org/en/shelley/

* Parameters and decentralization: the way ahead - we'll be making adjustments to the k-parameter in Cardano. Here’s why On December 6 - IOHK
https://iohk.io/en/blog/posts/2020/11/05/parameters-and-decentralization-the-way-ahead/

* Cardano Foundation on K
https://medium.com/cardanorss/cardano-foundation-to-adjust-its-delegation-methodology-following-changes-to-the-k-parameter-7636ffb8e82

* Results of moving K to 500 “Overall, it has proven successful” - IOHK
https://iohk.io/en/blog/posts/2021/03/04/not-long-till-d-0-day/

* Last K study - IOHK - by Christina Ovezik & Aggelos Kiayias Posted 19 April, 2022
https://blogs.ed.ac.uk/blockchain/2022/04/19/pool-splitting-behaviour-and-equilibrium-properties-in-cardano-rewards-scheme/

