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
    - Vote power is a test token implemented as a transferable, fungible and uncapped SPL token. Please refer to [1] and [2] for defintions. 
    - Vote power is the square root of the weights a member holds in the cap table (see WHIP-12). Its sole purpose is to make the power distribution and voting within WiHi transparent. 
    - New units of vote power are assigned at the end of each month and decided on by the voting mechanism illustrated in this WHIP according to the previous vote power distribution. 
    - The initial vote power distribution according to the cap table will be conducted by the core team
- Voting mechanism 
    - Votes follow the principles laid out in WiHi's association articles:
    - Voting can be initiated by the governance committee or by 5% of the vote power
    - If not otherwise specified in the association articles, a vote requires simple majority to pass
    - Voting needs to be announced at least 14 days before the vote period ends
    - Members eligible for voting have to receive an email informing them about the voting and its details
    - For transparency reasons, the vote and its details have to be announced in a discord channel in the friends layer of the DAO onion
    - The voting window is 5 days
- Implementation
    - In order to implement the token, a realms DAO is created
    - Vote Power is a community token which mint authority lies with the DAO
    - threshold for decision taking is 51%
    - minimum number of community tokens needed to manage the DAO is set to 3
    - Token name is Vote Power
    - Following best practice, a council with the three core team members (Michael, Uros, Mark) is instantiated. As soon as voting functions smoothly, the council will be removed (latest after the 10th vote in a row without an issue).

# Motivation 
 

# Rationale
Ideally, a token would be used that equals the weights in the cap table. Vote power would then be the square root out of these tokens. Nevertheless, this would require a custom implementation. Out of bandwidth considerations, this is left for future work.
Also, ideally the token would be a non-transferable (soul-bound) token using the Token-2022 standard. This standard is at the moment not supported by realms.