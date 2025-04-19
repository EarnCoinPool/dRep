
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
The K parameter creates a soft cap on the total stake in a pool that would receive optimal rewards. This number is often referred to as the saturation level. The cap or saturation level changes over time and is defined as a percentage of the maximum supply of ada (45bn) minus any amount that remains in the reserve (as of epoch 547, Reserve: 7,311,783,103) so that would equal 37,688,216,897 ada.

The current saturation level:  
Maximum pool size = (45bn - 7,311,783,103 in reserves) / k = (37,688,216,897 / 500 ) = 75,376,433.794  

For readability we will use approximate amounts, so approximately:  
***Maximum pool size = (45bn - 7bn in reserves) / k = (38bn / 500 ) = 76 million***

"Within the Cardano documentation, a pool that reaches its maximum size is said to be saturated. A saturated pool offers the highest rewards to delegators and is most lucrative for its operators, while an over-saturated pool delivers lower rewards. The system thereby incentivizes delegators to move their stake to a pool containing less ada, in order to maintain their yield and thus encourages the decentralization of the network."[^3]

Adjusting K parameter to 1,000 would set the saturation level to the following approximate level:  
***Maximum pool size = (45bn -  7bn in reserves) / k = (38bn / 1000 ) = 38 million***  

The move to K=1,000 with a saturation level around 38 million ada will, as stated above by IOHK will incentivize delegators to move their stake to a stake pool containing less ada, so they can maintain their rewards, thus encouraging wider decentralization of the Cardano network.[^3]

#### Is it safe to move K to 1,000 and why moving in one big move is recommended by IOG Scientist
IOG has stated:

"It is worth noting that the k-parameter is not amenable to small, gradual increases."[^5] and "Therefore, the best strategy for an upwards adjustment of k is to move in larger, less frequent increments – and to move it as far and as fast as practical network dynamics and economics will allow."[^5]

The last time K was adjusted it went from 150 to 500 and then the recommendation from IOG was to go to 1,000. The current research looked at 750 vs 1,000 and showed 1,000 would be most effective with a projection of almost doubling our Nakamoto coefficient.[^4]

IOG research has said it is safe to increase K to 1,000 on several post indicating that it's safe both for the security and economics. 

From IOG:

"Modeling the long-term viability of stake pools, we found that k values of 1,000 were stable in the long term. As a result, our aim is to move to k=1,000 during March 2021. We recognize the importance of economic factors that also strongly influence pool profitability and will continue to consult widely with the community on the plan; the social dynamics of the network should also not be underestimated."[^5] and "Previously, IOG had suggested that this value could be safely raised to 1,000"[^3]



#### History of Announcements and Steps to get K Parameter Increased to 1,000
The Shelley/Decentralization phase of the roadmap included K being set to 1,000 stake pools.[^7] It was announced that K would be increased in March 2021 to 1,000[^8] However due Alonzo hard fork and the deployment of the full Goguen smart contract this was delayed.[^9] 

After the delay IOG then sent several surveys and had several discussions with the SPOs over the next year or two. In May 2023 a mainnet poll was conducted. At first SPOs were told it was just on K but then as the poll date neared min pool fee was added. The mainnet poll took place in epochs 412-415 in May 2023 with the results supporting the option to Increase K to 1000 and halve minPoolCost to 170 ada. AdaStat show the vote using 5 metrics. K=1,000 and min fee of 170 won the poll using each of the 5 metrics.[^6]

However, the Parameters Committee decided to just adjust min pool fee and then "watch metrics" before adjusting K. The SPO community was then told there was a new process and if we wanted to adjust K a Parameters Committee Proposal needed to be submitted via Cardano forum and official document. October 2023 Earn Coin Pool submitted a K-PCP. The K-PCP was not taken up and the committee was notified that current PCP would need to resubmit to be considered in the next window.

In May 2024 Earn Coin Pool submitted a Position to Resubmit the K-PCP. The Parameters Committee did not take up the PCP and did not issue a regular PCP result but issued a comment on this discussion of the K parameter to support the community endeavor.

Now it's up to the community to submit a parameter governance proposal.

[^6]: [https://forum.cardano.org/t/pcp-k-parameter-earncoinpool/122701](https://forum.cardano.org/t/pcp-k-parameter-earncoinpool/1227010
[^7]: "Come the end of the Shelley era, we expect Cardano to be 50-100 times more decentralized than other large blockchain networks, with the incentives scheme designed to reach equilibrium around 1,000 stake pools." [https://roadmap.cardano.org/en/shelley/](https://roadmap.cardano.org/en/shelley/)
[^8]: "Modeling the long-term viability of stake pools, we found that k values of 1,000 were stable in the long term. As a result, our aim is to move to k=1,000 during March 2021." [https://iohk.io/en/blog/posts/2020/11/05/parameters-and-decentralization-the-way-ahead/](https://iohk.io/en/blog/posts/2020/11/05/parameters-and-decentralization-the-way-ahead/)
[^9]: "K will not change in Q3. Our focus is on a successful Alonzo hard fork and the deployment of the full Goguen smart contract capability. We have also clearly stated elements like multi-pool delegation get put in place as we reopen the consultation on K and other parameters."[https://x.com/timbharrison/status/1399657898364518401](https://x.com/timbharrison/status/1399657898364518401)

## Precedent: K was already increased to 500

## Constitutional Alignment

### Technical Review / Expected Impact
"From IOG’s calculations, there are about 100 public pools that would be affected by a move to k=1,000, representing around 2bn ada that would need to be redelegated (8% of the supply)."[^3] It also important to note that exchanges like Binance have already setup their pools to be below the K=1,000 saturation cap.[^10] indicating they are willing and ready for K=1,000.

The most recent technical review done in April 2022 by Christina Ovezik & Aggelos Kiayias which  took in to account pool splitting and "emulate the current Cardano stakeholder distribution, using a combination of real data points (taken from ADApools and PoolTool) and synthetic points that we draw from a Pareto distribution"[^4] found that: "As expected, the values of the Nakamoto coefficient diverge more from the ideal ones, but the increase in k still helps to achieve a higher degree of decentralisation."[^4] and "Note that the final number of pools was also lower than k in these observations, which can be attributed to the decrease in the system’s active stake."[^4] This research showed adjusting "...k can drive the system towards a more decentralised state, as measured by its Nakamoto coefficient."[^4] It also compared K=750 vs K=1,000 with the current conditions including pool splitting and demonstrated the K=1,000 almost would double our Nakamoto coefficient while K=750 would have minimal impact. This again confirms earlier research that moving K as far and as fast as possible is best method for adjusting K.

[^10]: [https://pool.pm/search/bnp](https://pool.pm/search/bnp)


### Economic impact
Ensure that stake pools are adequately rewarded for maintaining the Cardano Blockchain (Appendix I, Section 2.2: #2) Number and health of stake pools (Appendix I, Section 2.2: Core Metrics)

### Product Committee 2025 Roadmap Supporting Changes

The Product Committee 2025 roadmap includes: 
* Introduce min-margin parameter that can be voted on via governance to modify[^11]
* Modify pledge-benefit curve for a0[^11]

The 2025 roadmap includes two items that many believe with further help a change to K be more effective. Replacing min pool fee with a min margin and a0 adjustments, making pledge move effective. These two changes could further lead to better than the project results of doubling our Nakamoto coefficient.

[^11]: Product Committee: 2025 Proposed Cardano Roadmap [https://productcommittee.docs.intersectmbo.org/committee-outcomes/2025-cardanos-roadmap/2025-proposed-cardano-roadmap](https://productcommittee.docs.intersectmbo.org/committee-outcomes/2025-cardanos-roadmap/2025-proposed-cardano-roadmap)

### Reversion/Recovery Plan
A reversion/recovery plan should not be necessary as the K parameters have been changed in the past and the effects are known. However, in case of a disaster recovery the K parameter can/would be set back to 500 if a reverting change was necessary due to either a Severity 1 or Severity 2 incident or issue. If a Severity 3 incident or issue the K parameter can/would be set back to 750 for further monitoring. If at K at 750 and the Severity increased to the 1 or 2 level, the K parameter would be set back to 500. No other actions would need to be taken to restore the network. Under Appendix I, Section 1 there are 3 Severity Levels classified; Severity 1 is a critical incident or issue, Severity 2 is a major incident or issue, and Severity 3 is a minor incident or issue.

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

