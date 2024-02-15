# WHIP-13: Initial Voting

## Author(s)
Mark

## Type
Technical

## Acceptance date [only after acceptance]

# Abstract 
WHIP-12 illustrates the initial voting mechanism of the WiHi DAO implementing the initial governance illustrated in WHIP-12.

# Specification 
- Vote power 
    - Vote power is implemented with a non-transferable ("soul-bound"), fungible and uncapped Solana-based token called Vote Point. Please refer to [1] and [2] for defintions. 
    - For each weight received in the cap table (see WHIP-12), a member receives a Vote Point. 
    - Vote power is the square root of vote points a member controls
    - New units of vote points are assigned at the end of each month and decided on by this voting according to the previous vote power distribution. 
    - The initial vote point distribution according to the cap table will be conducted by the core team
- Voting mechanism 
    - Votes follow the principles laid out in WiHi's association articles:
    - Voting can be initiated by the governance committee or by 5% of the vote power
    - If not otherwise specified in the association articles, a vote requires simple majority to pass
    - Voting needs to be announced at least 14 days before the vote period ends
    - Members eligible for voting have to receive an email informing them about the voting and its details
    - For transparency reasons, the vote and its details have to be announced in a discord channel in the friends layer of the DAO onion
    - The voting window is 5 days
- Implementation
    - Vote unit is a token which mint authority lies with the DAO
    - open questions:
        - Should the WiHi DAO utilize realms for its voting
        - how to implement non-transferability - token 2022
        - how to implement square root voting 

# Motivation 
on-chain 

# Rationale [of design decisions within the specification]