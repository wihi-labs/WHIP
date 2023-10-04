# WHIP-0006: Voting 

## Author(s)
[Mark Ballandies](https://twitter.com/BallandiesMC)

## Type [governance]

# Abstract

Following the mechanisms outlined in [onocoy's whitepaper](https://static1.squarespace.com/static/6313a587324d1047ec4d9a13/t/64e892a5e6f5d8652a2b925b/1692963500980/20230825_whitepaper_onocoy_final.pdf), WHIP-0006 outlines the principles of WiHi's voting mechanism, where token holders can anonymously delegate tokens to identified delegates who can vote on proposals that can be initiated by all community members. Initially, a supermajority (>66%) is needed for decision-making, with future exploration of alternative voting methods to prevent the "Tyranny of the Majority." This approach aims to attract motivated community members by showcasing their participation in governance. The rationale emphasizes inclusivity, autonomous improvement, and prevention of power concentration. Identifying delegates is essential to prevent fraud and maintain transparency, but minimal criteria will encourage broad participation. Anonymous delegation ensures wide engagement, preserving privacy, and allowing all community members to propose votes. Detailed specifications will follow in future WHIPs.

# Specification 

![WiHi DAO onion](wihi_voting_mechanism.png)

The figure above illustrates the voting mechanism applied in WiHi. 

Community members who possess WiHi tokens can anonymously delegate their tokens to identified (partially doxed) delegates within the system. 

Delegates use their delegated tokens to vote on proposals, with voting power proportional to the square root of the tokens they control and those which were delegated to them (e.g., 1 token unit equals 1 vote, but 4 token units equal 2 votes, 9 tokens – 3, and so on). 
All community members have the opportunity to submit vote proposals. 

Initially, super majority will be employed for decision-making (>66% of the voting power is required to accept a proposal), but alternative voting mechanisms will be explored in the future to better align with community sentiment and prevent the "Tyranny of the Majority."

This and further specifications of the voting mechanism will be illustrated in greater detail in follow-up WHIPs.

# Motivation

In order to grow WiHi's community with intrinsically motivate individuals we need to be able to show them how we want to let them participate in the governance of the system. 

# Rationale [of design decisions within the specification]

The primary objective of WiHi's governance can be summarized as follows:

1. Inclusion of all stakeholders, including users, in decision-making processes.
2. Facilitation of self-improvement without centralized control.
3. Prevention of power concentration within any individual or group of stakeholders.

Identifying/ doxing delegates' is required to  
- prevent Sybil attacks on the square-root voting (fraudulent voting by distributing once own tokens to several anonymous identies)
- ensure transparency in the allocation of voting power. This transparency allows for the identification of power concentration and the implementation of mitigation strategies, such as forks.

Nevertheless, in order to facilitate broad participation and thus the taking of responsibility, the objective is to establish (minimal) criteria such that a large number of community members become delegates, promoting decentralization. 

Anonymous delegation of votin power enables broad participation in governance and ensures private reasoning, [both crucial for the emergence of collective intelligence](https://medium.com/coinmonks/complex-systems-part-2-managing-complexity-with-bottom-up-solutions-9d6fadd88cc4).

Enabling all community members to submit vote proposals support free expression and broad participation, [both crucial for the emergence of collective intelligence](https://medium.com/coinmonks/complex-systems-part-2-managing-complexity-with-bottom-up-solutions-9d6fadd88cc4).
