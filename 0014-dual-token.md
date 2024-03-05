# WHIP-14: Dual token model

## Authors
[Uroš](https://twitter.com/urosnoetic), [Mark](https://twitter.com/BallandiesMC) 

## Type
Technical 

## Acceptance date [only after acceptance]

# Abstract
WiHi is seeking to build out a global and dense network of weather and climate monitoring. Much of the data currently available to WiHi is free to use. WiHi should avoid paying in equity for the use of free data; otherwise, it would incentivize grifting on its protocol. Here we propose a two-token model comprised of a core token \$WNT, reflecting the value of the WiHi economy, and a utility token \$WIHI, used to reward miners and all other supporters in the supporter layer of the DAO. \$WNT funds the treasury of the \$WIHI with the hope that outflows of \$WIHI will balance the inflows of \$WNT. We propose to allow the market to price the utility token with the expectation that the collective intelligence of the market will decide to adequately reward supporters. We also propose to allow for the provision of a pricing guarantee to certain miners, as not all miners would take the risk of working only for tokens.

# Specification
WiHi shall issue a token called \$WNT which will be used to vote on matters of governance in the WiHi DAO and to reward the core and contributor layers. WiHi shall issue a utility token called \$WIHI which will be used to reward the WiHi supporter layer.

WiHi shall create two treasuries: a core treasury and a supporter treasury. The core treasury shall initially contain the entire, fully diluted supply of \$WNT tokens in addition to any tokens owned by WiHi at the time of instantiation. The supporter treasury shall initially be empty. The core treasury may hold any type of token. The supporter treasury may hold only \$WNT and may receive this \$WNT only from the core treasury.

\$WNT:
- Fixed supply
- Represents voting rights in the WiHi DAO
- Represents ownership of core treasury
- May only be swapped with tokens in the core treasury with agreement of at least 80\% of a DAO vote; upon swap the \$WNT is burned

\$WIHI:
- Flexible supply
- Represents ownership of supporter treasury
- May be swapped with tokens in treasury at any time; upon swap the \$WIHI is burned
- Minted as needed to reward supporters

Core treasury:
- Receives and remits tokens through the normal course of WiHi business

Supporter treasury:
- May receive only \$WNT tokens and only from the core treasury

In certain cases, WiHi shall provide data providers with a guaranteed price for their \$WIHI tokens, wherein this guarantee will be subject to expiry. For this purpose, a custody mechanimsm will be created that will custody this guarantee. When guarantees are swapped for tokens at the agreed-upon price, the swapped guarantees are burned. When gurantees are transferred off the custody mechanism, without being swapped, the agreement is null and void for the tokens now in circulation. The agreement will continue to be honored for the guarantees that remain in custody and have not yet expired. Only the WiHi protocol may transfer tokens into the custody mechanism, meaning that only the WiHi protocol may make such guarantees and guarantees may not be reinstated after being revoked, either due to expiry or due to transfer.

# Motivation
WiHi is seeking to build out a global and dense network of weather and climate monitoring. Weather monitoring is a common good managed and subsidized through a loose cooperation of national, super-national, and private entities. Although the benefits of updating the current cooperative framework with web3 technology are apparent, achieving them requires stakeholder management. Aligning token incentives with project goals is therefore necessary.

The first necessary alignment is that of ensuring that a token captures the value of the WiHi economy. To do this, revenues of the economy must accrue value to token holders. Various designs and industry best-practices exist that ensure such alignment, so this is easy enough to achieve, but what is often missing is a clear definition of who owns the economy and in what proportion. This is the second necessary alignment between token incentives and project goals.

Complicating matters with respect to the second alignment is that WiHi is implementing an open approach to data ingress, wherein any operator may send data and expect to receive a reward. The network of freely-available weather data, which can be accessed through the Internet at little cost, is relatively large and useful. However, the value of rewarding this kind of data is unclear.

Moreover, WiHi seeks to entice membership of those who are intrinsically motivated to solve the challenges in weather and climate. It is further necessary to reward intrinisically-motivated people for their efforts and to separate WiHi-aligned motivation from motivation for financial gain at the expense of WiHi.

# Rationale
The token representing the value of the WiHi economy should be seperated from the token representing the value of the supporter economy. The assumption underlying this proposal is that the main differentiator between the supporter and contributor layers are that it is difficult to separate supporters who are intrinsically motivated to help WiHi succeed and those that are only motivated by financial gain, even at the expense of WiHi's success. Contributors, like the core team, are assumed to help with the day-to-day operations of WiHi and their main motivations and loyalty to project goals tends to be much easier to identify.

It thus makes sense to directly reward contributors and the core team with a stake in the main economy and not directly reward supporters with the same stake. To allow for this degree of seperation, at least two types of tokens are required for rewarding each group.

The main economy token may be called \$WNT, which would stand for "WiHi Network Token," the expectation being that the DePIN community would understand this token to behave similarly to the Helium Network Token. The similarity is in that its fully diluted value represents the full value of the WiHi economy. Tying the value of \$WNT to the value of the economy can be done in various ways. Generally, there are three models:
1) Use incoming revenue to buy \$WNT on the open market (buyback model)
2) Store incoming revenue in treasury and tie ownership of \$WNT to the amount stored (ownership model)
3) Only accept \$WNT as payment for WiHi services, which is burned whenever used for this purpose (burn-and-mint model)

Mathematically, the three models are equivalent from a cash flow perspective because value is generally equal to the difference in discounted cash flows into and out of the economy and this is invariant across any value storage scheme.

Although burn-and-mint is popular in the DePIN space, the most flexible mechanism that serves the long-term interests of WiHi is the middle option. In both remaining models, value is dissipated to token holders without giving the chance to the DAO to decide how it may deploy capital. Since weather and climate are long-term endeavors, it stands to reason that it would be of benefit to the community that WiHi hold on to as much revenue as the community might allow. The DAO may allow for a small amount of burn in order to keep token holders happy, but this should not be overly large; a full burn would be akin to a stock dividend disbursing all revenue for that month.

With a treasury, the DAO is able to direct the flow of funds to different stakeholders. An important segment of stakeholders is comprised of the supporter base. Here, the DAO should direct funds to a treasury that is meant to reward supporters. However, in the initial stages, WiHi is not able to adequately reward supporters due to lack of revenue, nor is it clear how much they should be rewarded, so the proposal envisions that the market should decide the amount.

Therefore, we may introduce a supporter economy token and call it \$WIHI. The name is meant to associate the function of the token with cooperative  and open participation in WiHi. This token, unlike \$WNT, while representing a share of a supporters' treasury, is not associated with governance of WiHi. Its main purpose is to adequately reward the supporter base and the goal would be to reach an equilibrium wherein the \$WNT coming into the supporter treasury is fully balanced by the outgoing \$WIHI at the current market rate. To determine the amount of \$WNT granted to the supporter treasury, we envision a process of negotiation within the DAO, wherein an agreement is reached between supporters and the rest of the DAO. How this should be implemented is outside the scope of this proposal.

Nevertheless, a complication arises in that some miners may not be willing to participate in a scheme without guaranteed rewards. This will become a concern as soon as WiHi is seen as an attractive customer for data providers that are able to charge a significant price for their data. To remedy this, the proposal envisions that these providers be rewarded with options that provide a backstop to the token price via a repurchase guarantee. Such options can be exercised either by being swapped at the guaranteed repurchase price or by being converted to \$WIHI, after which the repurchase guarantee would immediately expire. Moreover, these options should be time-limited in order to allow WiHi to monitor its outstanding liabilities more effectively.

Note that none of the above is meant to imply that the \$WNT token be limited in ownership to the core and contributors. In fact, the opposite should be the case. To achieve truly fair and broad participation, WiHi should strive to distribute \$WNT among as large a group of stakeholders as is feasible. This is why, under the proposed mechanism, the supporter treasury is to be stocked with \$WNT and no other token; the aim here is to create a pipeline of intrinsically-motivated stakeholders, who enter through the supporter door and eventually become contributors themselves, either through ownership of a large amount of \$WNT or through contribution of their time and effort towards the big problems WiHi is solving.
