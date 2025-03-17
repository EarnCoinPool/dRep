Section 5
Section 5
In order to promote transparency in the process of on-chain governance, prior to being recorded or enacted on-chain, all proposed governance actions are expected to follow a standardized and legible format including a URL and hash of all documented off-chain content to the Cardano Blockchain. Sufficient rationale shall be provided to justify the requested change to the Cardano Blockchain. The rationale shall include, at a minimum, a title, abstract, reason for the proposal, and relevant supporting materials.
The content of every on-chain governance action must be identical to the final off-chain version of the proposed action.
"Hard Fork Initiation" and "Protocol Parameter Change" governance actions shall undergo sufficient technical review and scrutiny as mandated by the Guardrails to ensure that the governance action does not endanger the security, functionality, performance or long-term sustainability of the Cardano Blockchain. On-chain governance actions should address their expected impact on the Cardano Blockchain ecosystem.
All owners of ada shall have the right to ensure that the process for participating in, submitting and voting on on-chain governance actions is open and transparent and is protected from undue influence and manipulation.
 
2.2 Economic Parameters
2.2. Economic Parameters
The overall goals when managing economic parameters are to:
Enable long-term economic sustainability for the Cardano Blockchain;
Ensure that stake pools are adequately rewarded for maintaining the Cardano Blockchain;
Ensure that ada owners are adequately rewarded for using stake in constructive ways, including when delegating ada for block production; and
Balance economic incentives for different Cardano Blockchain ecosystem stakeholders, including but not limited to Stake Pool Operators, ada owners, DeFi users, infrastructure users, developers (e.g. DApps) and financial intermediaries (e.g. exchanges)
 

[2.4. Technical/Security Parameters](https://github.com/IntersectMBO/cardano-constitution/blob/main/cardano-constitution-1/cardano-constitution-1.txt.md#24-technicalsecurity-parameters)

The overall goals when managing the technical/security parameters are:
1. Ensure the security of the Cardano Blockchain network in terms of decentralization and protection against adversarial actions
2. Enable changes to the Plutus language

**Triggers for Change**
1. Changes in the number of active SPOs
2. Changes to the Plutus language
3. Security threats
4. Cardano Community requests

**Counter-indicators**
* Economic concerns, e.g. when changing the number of stake pools

**Core Metrics**
* Number of stake pools
* Level of decentralization

<p> 
 <strong>Changes to Specific Technical/Security Parameters</strong> 
</p>

**Target Number of Stake Pools (stakePoolTargetNum)**<br>
Sets the target number of stake pools  
* The expected number of stake pools when the network is in the equilibrium state
* Primarily a security parameter, ensuring decentralization by stake pool division/replication
* Has an economic effect as well as a security effect - economic advice is also required when changing this parameter
* Large changes in this parameter will trigger mass redelegation events
 
[**2.6. Monitoring and Reversion of Parameter Changes**](https://github.com/IntersectMBO/cardano-constitution/blob/main/cardano-constitution-1/cardano-constitution-1.txt.md#26-monitoring-and-reversion-of-parameter-changes)  
All network parameter changes **must** be monitored carefully for no less than 2 epochs (10 days)  
* Changes must be reverted as soon as possible if block propagation delays exceed 4.5s for more than 5% of blocks over any 6 hour rolling window<br>

All other parameter changes should be monitored  
* The reversion plan **should** be implemented if the overall effect on performance, security, functionality or long-term sustainability is unacceptable.<br>

A specific reversion/recovery plan **must be** produced for each parameter change. This plan must include:  
* Which parameters need to change and in which ways in order to return to the previous state (or a similar state)
* How to recover the network in the event of disastrous failure
This plan should be followed if problems are observed following the parameter change. Note that not all changes can be reverted. Additional care must be taken when making changes to these parameters.
 
[Changes to Specific Technical/Security Parameters](https://github.com/IntersectMBO/cardano-constitution/blob/main/cardano-constitution-1/cardano-constitution-1.txt.md#changes-to-specific-technicalsecurity-parameters)

**Target Number of Stake Pools (stakePoolTargetNum)**

Sets the target number of stake pools
* The expected number of stake pools when the network is in the equilibrium state
* Primarily a security parameter, ensuring decentralization by stake pool division/replication
* Has an economic effect as well as a security effect - economic advice is also required when changing this parameter
* Large changes in this parameter will trigger mass redelegation events

**GUARDRAILS**  
SPTN-01 (y) stakePoolTargetNum must not be lower than 250  
SPTN-02 (y) stakePoolTargetNum must not exceed 2,000  
SPTN-03 (y) stakePoolTargetNum must not be negative  
SPTN-04 (y) stakePoolTargetNum must not be zero  
 
[9. List of Protocol Parameter Groups](https://github.com/IntersectMBO/cardano-constitution/blob/main/cardano-constitution-1/cardano-constitution-1.txt.md#9-list-of-protocol-parameter-groups)

The technical/security parameter group consists of:
* pool pledge influence (poolPledgeInfluence)
* pool retirement maximum epoch (poolRetireMaxEpoch)
* desired number of pools (stakePoolTargetNum)
* Plutus execution cost models (costModels)
* proportion of collateral needed for scripts (collateralPercentage)


