# WHIP-1: WiHi Improvement proposals

## Author(s):

[Mark Ballandies](https://twitter.com/BallandiesMC)

## Type

Governance

# Abstract 

A WiHi Improvement Proposal (WHIP) is a (technical) design document providing information to the WiHi community, or describing a new feature for WiHi or its processes or environment. The WHIP should provide a concise (technical) specification of the feature and a motivation for the feature.

WHIPs are the primary mechanism of the WiHi DAO for achieving community-wide consensus/ decisions. It is a mechanism to propose new features, to gather community input on a topic, and to document the design decisions that have gone into WiHi - once accepted a WHIP becomes binding for the WiHi DAO. The WHIP champion is responsible for building consensus within the community and documenting dissenting opinions.

WHIP-1 is sketching a preliminary mechanism for WHIPs to empower the core team to reach design decisions of WiHi more efficiently. It is envisioned that this WHIP will be replaced once the process will be opened for larger parts of the community or shortcomings are identified.

# Specification 

The WHIP process begins with a new idea for WiHi. Each potential WHIP must have a champion -- someone who writes the initial WHIP using the style and format described below, shepherds the discussions in the appropriate forums, and attempts to build community consensus around the idea. The champion is also automatically an author of the WHIP.

Each WHIP has to have the following structure

- Meta-info
    - Author(s)
    - Type [technical, governance, etc.]
    - acceptance date [when decision became final on-chain]
- Abstract [max 200 words]
- Specification [of the concrete improvement]
- Motivation [(of the authors) for proposing the improvement]
- Rationale [of design decisions within the specification]

Further (sub)-sections can be added.

The champion is the one editing the proposed WHIP, but can allow others to join editing in which case these have to be added to the list of authors.

A champion can be any community member.

The process for getting an WHIP accepted is as follows

1. The champion creates a WHIP by creating a markdown document that coheres to the above mentioned structure and by creating a pull request for this document to the WHIP repository on github
2. A moderator accepts the pull request and creates a corresponding "issue" if the formal requirements are met and there is no inappropriate behavior (There is zero-tolerance for advertisements, harassment, trolling, racism, sexism, homophobia, NSFW content and hate speech).
2. The moderator shares with others the document via the “WHIP” channel in discord as a thread. 
3. Official comments from community members on the WHIP, which must be addressed by the author(s) *in writing* within the WHIP document, will be done via the corresponding "issue" on Github - clarifications/sharing of ideas can be done via Discord or other venues.
4. Champions are responsible for getting support for the WHIP (e.g. through calls in the community, discussions on Discord in the whip's thread, etc.).
5. A WHIP is decided on as follows
    1. The champion informs the WiHi community that the WHIP is ready to be decided on by stating this clearly in the WHIP’s thread in the WHIP channel on discord and tagging the moderator who opened the WHIPs thread in this message. 
    2. A moderator creates a voting proposal within the "WiHi Gov Committee" realm and informs the core team in a message in the WHIPs thread on Discord by tagging them and sharing the link to the vote proposal.
    2. The status of WHIPs is changed to "Voting open" by a moderator and the link to the on-chain proposal is added to the WHIP, after which no more changes can be made to the document. 
    2. The voting period is 7 days. 
    2. Each core team member can cast their vote (accept/ reject/ abstain) on-chain on the WHIP via realms. Non-voting is counted as abstaining. For the time being, core team members have one vote each and simple majority decides.  
6. After a decision has been reached, the WHIPs status on github is changed accordingly by a moderator.
7. The process is closed by the moderator sharing the final status in the WHIPs discord thread.

An update of this process has to follow the specified process.

# Motivation

As agreed in the team call at September 26th, 2023, we want to have WHIPs as the main tool to structure our thoughts and find agreement on system design features and system development. In particular, WHIPs have the purpose to inform (new) community members about the taken decisions that resulted in the current system layout.

An improvement proposal system has been chosen to facilitate this as it has been demonstrated by other web3 systems to be effective to govern decentralized communities. In particular, it is a tool that enables bottom-up initiatives to foster a top-level decision of the WiHi DAO which has to be followed/ implemented by all members. 

The core motivation for the currently illustrated WHIP process is to have a simplistic but effective process for the core team to reach decisions transparently, involving already the community. 

# Rationale

It is okay to restrict the decision decision making to the core team at the moment as these are the individuals that represent by far the greatest voting power in the WiHi ecosystem. As soon as other individuals will have voting power in the system, this will be adjusted with priority.

