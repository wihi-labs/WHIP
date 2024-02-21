# WHIP-12: WiHi initial governance

## Author(s)
[Mark](https://twitter.com/BallandiesMC) 
[Uros](https://twitter.com/urosnoetic)

## Type
Governance

## Acceptance date [only after acceptance]

# Abstract 
WiHi's envisioned voting mechanism is outlined in [WHIP-0007](https://github.com/wihi-labs/WHIP/blob/main/0007-voting/main.md), WiHi's decentralized organization is described in [WHIP-0002](https://github.com/wihi-labs/WHIP/blob/main/0002-wihi-dao/main.md), and  WiHi's instantiated legal structure for this organization is illustrated in [WHIP-0008](https://github.com/wihi-labs/WHIP/blob/main/0008-legal-structure/main.md). 
This WHIP illustrates the initial mechanism with which WiHi will reach decisions on WHIPs and voting items within the legal entity (e.g. such as electing the governance committee).

# Specification 
- The core team of the DAO (inner layer of DAO onion) consists of those being voted into the governance committee and the commission of the association (legal entity). 
- Members of the association can vote on WHIPs and vote items within the association. 
- Until the WiHi token is deployed, members of the association can become those that are part of the cap table that registers the percentage of tokens from the founders pool a founder receives
- Receving shares within the cap table requires membership of the contributor or core team layer
    - Share calculation:
        - A 100% time engagement in a month with WiHi equals a weight of 1 for that month
        - The share of the founders pool is calculated as the division between the sum of ones own shares divided by the sum of all shares
    - core team members and contributors can contribute fiat into the organization. 10000 (ten thousand) US Dollar adds the weight of 1 to ones own weight calculation. 
- Following the principle of square root voting that mitigates the risk of power concentrations as outlined in [WHIP-0007](https://github.com/wihi-labs/WHIP/blob/main/0007-voting/main.md), the vote power of members within a month equals the square root of their weight on the 1st of that month. 
- Voting is conducted on-chain
- Members who participate in voting have to be listed on the WiHi website with their name and blockchain address they use for voting. 
 
# Motivation 
Until now, without a token deployed, the WiHi organization was not in a position to reach decisions on vote items such as the WHIPs. Following our values of transparency and decentralization, it is important to lay out the mechanism with which decisions are taken, before decisions are taken. Hence the need for this WHIP arose.

# Rationale 
WiHi follows the principle of progressive decentralization, WiHi strives to decentralize all aspects of its system over time. Until the setup of the association, decision making was restricted to the core team. With the setup of the association, the set of people involved in decision making is extended to those who were in WiHi from the beginning, in total counting 7 individuals.

Only members of the association can vote on items, because a) this mitigates liability risks (e.g. otherwise voters could be personal liable), and b) it results in a merger of the off-chain legal world with the on-chain governance world. 