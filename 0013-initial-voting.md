# WHIP-13: Initial Voting

## Author(s)
Mark

## Type
Technical

## Acceptance date [only after acceptance]

# Abstract 
WHIP-13 illustrates the initial voting mechanism of the WiHi DAO implementing the initial governance illustrated in [WHIP-12](https://github.com/wihi-labs/WHIP/blob/main/0012-initial-governance.md).

# Specification 
- vWiPo 
    - vWiPo is a temporary token to test the governance mechanisms within WiHi. It is implemented as a transferable, fungible and uncapped SPL token. Please refer to [1](https://link.springer.com/article/10.1007/s10586-021-03256-w) and [2](https://www.researchgate.net/publication/374005682_A_Taxonomy_for_Blockchain-based_Decentralized_Physical_Infrastructure_Networks_DePIN) for defintions. 
    - vWiPo is the square root of the weights a member holds in the cap table (see WHIP-12). Its sole purpose is to make the power distribution and voting within WiHi transparent. 
    - New units of vWiPo are assigned at the end of each month and decided on by the voting mechanism illustrated in this WHIP according to the previous vWiPo distribution. 
    - The initial vWiPo distribution according to the cap table will be conducted by the core team
- Voting mechanism 
    - Votes follow the principles laid out in WiHi's association articles:
    - Voting can be initiated by the governance committee or by 5% of the vWiPo
    - If not otherwise specified in the association articles, a vote requires simple majority to pass
    - Voting needs to be announced at least 14 days before the vote period ends. The voting on the intial WHIPs prior to this WHIP and including this WHIP can be announced at least 5 days before the vote period ends. 
    - Members eligible for voting have to receive an email informing them about the voting and its details
    - For transparency reasons, the vote and its details have to be announced in a discord channel in the friends layer of the DAO onion
    - The voting window is 5 days
- Implementation
    - In order to implement the token, a [Realms](https://realms.today/) DAO is created
    - Token name is vWiPo
    - vWiPo is a community token which mint authority lies with the DAO
    - the votes are conducted via the Realms proposal mechanism
        - Also the creation and assignment of new vWiPo is performed via this proposal mechanism.
    - threshold for decision taking is 51%
    - minimum number of community tokens needed to manage the DAO is set to 1 (roughly 5% of the total vote power)
    - Following best practice, a council with the three core team members (Michael, Uros, Mark) is instantiated. As soon as voting functions smoothly, the council will be removed (latest after the 10th vote in a row without an issue).

# Motivation 


# Rationale
Ideally, a token would be used that equals the weights in the cap table. Vote power would then be the square root out of these tokens. Nevertheless, this would require a custom implementation. Out of bandwidth considerations, this is left for future work.
Also, ideally the token would be a non-transferable (soul-bound) token using the Token-2022 standard. This standard is at the moment not supported by Realms.