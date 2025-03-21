
### Governance Action Type:
Parameters

### Title:
Increase K (stakePoolTargetNum) from 500 to 1,000

### Abstract:
This parameter governance action seeks to increase the K parameter (stakePoolTargetNum) from 500 to 1,000 to increase decentralization, improve the economic stability of more stake pools by encouraging ada holders to delegate to a wider number of pools.

**NOTE:** The Constitution refers to the K parameter as stakePoolTargetNum, they are synonymous for each other. Since all the research, PCPs and past documentation refers to it as K we will use the term K parameter from here on out, but K is interchangeable with term stakePoolTargetNum parameter.

## Motivation

## Rationale

## Precedent: K was already increased to 500

## Constitutional Alignment

## Technical review

## Expected impact

### Economic impact
Ensure that stake pools are adequately rewarded for maintaining the Cardano Blockchain (Appendix I, Section 2.2: #2) Number and health of stake pools (Appendix I, Section 2.2: Core Metrics)

### Reversion/Recovery Plan
A reversion/recovery plan should not be necessary as the K parameters have been changed in the past and the effects are known. However, in case of a disaster recovery the K parameter can/would be set back to 500 if a reverting change was necessary due to either a Severity 1 or Severity 2 incident or issue. If a Severity 3 incident or issue the K parameter can/would be set back to 750 for further monitoring. If at K at 750 and the Severity increased to the 1 or 2 level, K parameter would be set back to 500. No other actions would need to be taken to restore network. Under Appendix I, Section 1 there are 3 Severity Levels classified; Severity 1 is a critical incident or issue, Severity 2 is a major incident or issue, and Severity 3 is a minor incident or issue.

### References and Supporting Information

K- PCP submitted by Earn Coin Pool 
https://forum.cardano.org/t/pcp-k-parameter-earncoinpool/122701

Position to Resubmit the K-PCP by Earn Coin Pool
https://forum.cardano.org/t/pcp-k-parameter-earncoinpool/122701/98

Cardano Foundation on K
https://medium.com/cardanorss/cardano-foundation-to-adjust-its-delegation-methodology-following-changes-to-the-k-parameter-7636ffb8e82#:~:text=The%20k-parameter%20determines%20the%20stake%20pool%20saturation%20point%2C,to%20delegate%20to%20a%20wider%20number%20of%20pools.

Results of moving K to 500 “Overall, it has proven successful” - IOHK
https://iohk.io/en/blog/posts/2021/03/04/not-long-till-d-0-day/

Last K study - IOHK - by Christina Ovezik & Aggelos Kiayias Posted 19 April, 2022
https://blogs.ed.ac.uk/blockchain/2022/04/19/pool-splitting-behaviour-and-equilibrium-properties-in-cardano-rewards-scheme/

