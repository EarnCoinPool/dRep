
### Governance Action Type:
Parameters

### Title:
Increase K (stakePoolTargetNum) from 500 to 1,000

### Abstract:
This parameter governance action seeks to increase the K parameter (stakePoolTargetNum) from 500 to 1,000 to increase decentralization, improve the economic stability of more stake pools by encouraging ada holders to delegate to a wider number of pools.

**NOTE:** The Constitution refers to the K parameter as stakePoolTargetNum, they are synonymous for each other. Since all the research, PCPs and past documentation refers to it as K we will use the term K parameter from here on out, but K is interchangeable with term stakePoolTargetNum parameter.

### Motivation 
The Shelley/Decentralization phase of the roadmap included K being set to 1,000 stake pools.[^1] It was announced that K would be increased in March 2021 to 1,000[^2] However due Alonzo hard fork and the deployment of the full Goguen smart contract this was delayed.[^3] 

[^1]: "Come the end of the Shelley era, we expect Cardano to be 50-100 times more decentralized than other large blockchain networks, with the incentives scheme designed to reach equilibrium around 1,000 stake pools." [https://roadmap.cardano.org/en/shelley/](https://roadmap.cardano.org/en/shelley/)
[^2]: "Modeling the long-term viability of stake pools, we found that k values of 1,000 were stable in the long term. As a result, our aim is to move to k=1,000 during March 2021." [https://iohk.io/en/blog/posts/2020/11/05/parameters-and-decentralization-the-way-ahead/](https://iohk.io/en/blog/posts/2020/11/05/parameters-and-decentralization-the-way-ahead/)
[^3]: "K will not change in Q3. Our focus is on a successful Alonzo hard fork and the deployment of the full Goguen smart contract capability. We have also clearly stated elements like multi-pool delegation get put in place as we reopen the consultation on K and other parameters."[https://x.com/timbharrison/status/1399657898364518401](https://x.com/timbharrison/status/1399657898364518401)

## Rationale

## Precedent: K was already increased to 500

## Constitutional Alignment

## Technical review

## Expected impact

### Economic impact
Ensure that stake pools are adequately rewarded for maintaining the Cardano Blockchain (Appendix I, Section 2.2: #2) Number and health of stake pools (Appendix I, Section 2.2: Core Metrics)

### Reversion/Recovery Plan
A reversion/recovery plan should not be necessary as the K parameters have been changed in the past and the effects are known. However, in case of a disaster recovery the K parameter can/would be set back to 500 if a reverting change was necessary due to either a Severity 1 or Severity 2 incident or issue. If a Severity 3 incident or issue the K parameter can/would be set back to 750 for further monitoring. If at K at 750 and the Severity increased to the 1 or 2 level, the K parameter would be set back to 500. No other actions would need to be taken to restore the network. Under Appendix I, Section 1 there are 3 Severity Levels classified; Severity 1 is a critical incident or issue, Severity 2 is a major incident or issue, and Severity 3 is a minor incident or issue.

### References and Supporting Information

* K- PCP submitted by Earn Coin Pool 
https://forum.cardano.org/t/pcp-k-parameter-earncoinpool/122701

* Position to Resubmit the K-PCP by Earn Coin Pool
https://forum.cardano.org/t/pcp-k-parameter-earncoinpool/122701/98

* Shelley Roadmap
https://roadmap.cardano.org/en/shelley/

* Cardano Foundation on K
https://medium.com/cardanorss/cardano-foundation-to-adjust-its-delegation-methodology-following-changes-to-the-k-parameter-7636ffb8e82#:~:text=The%20k-parameter%20determines%20the%20stake%20pool%20saturation%20point%2C,to%20delegate%20to%20a%20wider%20number%20of%20pools.

* Results of moving K to 500 “Overall, it has proven successful” - IOHK
https://iohk.io/en/blog/posts/2021/03/04/not-long-till-d-0-day/

* Last K study - IOHK - by Christina Ovezik & Aggelos Kiayias Posted 19 April, 2022
https://blogs.ed.ac.uk/blockchain/2022/04/19/pool-splitting-behaviour-and-equilibrium-properties-in-cardano-rewards-scheme/

