# WHIP-13: Initial Voting

## Author(s)
Mark

## Type
Technical

## Acceptance date [only after acceptance]

# Abstract 
WHIP-12 illustrates the initial voting mechanism of the WiHi DAO approximating the initial governance illustrated in [WHIP-12](https://github.com/wihi-labs/WHIP/blob/main/0012-initial-governance.md).

# Specification 
- Implementation
    - In order to implement the initial governance illustrated in WHIP-12, a [Realms](https://realms.today/) multi-sig DAO is created on Solana mainnet with the name "WiHi DAO". Members of this multi-sig are refered to as council members in the realms terminology.
    - Council membership is open to all WiHi association members
    - Council members can have a varying 'vote weight'
    - Vote weight of a council member is the integer rounded amount of vote power steming from the cap table or 1. At initialisation, the vote weights are distributed as follows Uros: 5, Michael: 5, Mark: 3, Vlad: 2, Saleh: 2, Kevin: 1, Yangchen: 1.
    - Threshold for decision taking is 51% of vote weight. Please note, in case some association members are not joining governance their vote weight is not considered in the threshold calculation.
        - Hence, only votes within the WiHi association that are subject to this majority rule can be faciliated by this on-chain voting mechanism. All DAO-wide decision for the time being shall require this simple majority of 51%.      
    - Votes are conducted via the Realms proposal mechanism
    - Vote weights cannot be delegated
    - Voting proposals can be initiated by all council members. 
    - Vote period is 5 days. 
    - Voting needs to be announced at least 14 days before the vote period ends by mail and in a discord channel within the friend layer. The voting on the intial WHIPs (WHIP 1-14) can be announced 5 days before the vote period ends. 
    - Members eligible for voting have to receive an email informing them about the voting and its details
    - For transparency reasons, the vote and its details have to be announced in a discord channel in the friends layer of the DAO onion
    - The voting window is 5 days
    - Changes in vote weight requires a proposal
- The WiHi association shall adopt this initial governance for their decision making. In particular, for all subject matters that require simple majority (51%), voting should be conducted via this initial governance mechanism. This will require a vote within WiHis general assembly.  

# Motivation 
The illustrated implementation follows the principles laid out in WHIP-12 and the WiHi association articles as best as possible, while keeping its implementation time efficient. In particular, a need within the DAO has arisen to finalize the open WHIPs asap. This WHIP is the enabler of this finalization.

# Rationale
- All council members being able to initiate proposals is aligned with the requirement from the WiHi association articles that the governance committee and/ or 5% of the voting power can initiate a mail-in-ballot or general assembly.
- Ideally, a vote weight would be used that equals the square root of weights in the cap table (which could be treated as a fictional token). Nevertheless, this would require a custom implementation as realms is neither facilitating non-transferable tokens that have fractions, nor supports square-root voting. Out of bandwidth considerations, this is left for future work.
- Vote weights cannot be delegated, because realms is using a non-transferable token for its vote weight/ council token implementation that cannot be delegated.
- Solana mainnet is utilized to guarantee the permanence/ immutability of decision taken within the WiHi DAO. In particular, this initial voting is not a test/ experiment.
- This voting mechanism is aligned with the dual-token model illustrated in WHIP-14. In particular, the illustrated initial voting/ vote weight/ council token will eventually be replaced with the WNT token.
- Vote weights are not adjusted on a monthly basis, as significant changes will not happen often: Because vote weight is the rounded integer value of vote power which in turn is calculated by taking the square-root of the weights in the cap table, an additional cap weight in a month has no significant impact. In case a major monetary investment is peformed, a new contributor is joining the cap table, or the cap weights have changed over time significantly, the weights shall be adjusted via a proposal.
