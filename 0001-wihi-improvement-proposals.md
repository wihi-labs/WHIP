# WHIP-1: WiHi Improvement proposals

## Author(s):

[Mark Ballandies](https://twitter.com/BallandiesMC), [Uroš](https://twitter.com/urosnoetic)


## Type

Governance

# Abstract 

A WiHi Improvement Proposal (WHIP) is a (technical) design document for improving WiHi. WHIPs provide (technical) specifications of a feature and a motivation for it.

WHIPs are to be the primary mechanism of the WiHi DAO for making decisions and achieving community-wide consensus. They are a mechanism to propose new features, to gather community input on a topic, and to document the design decisions that have gone into the growth of WiHi. Once accepted, a WHIP becomes binding. The WHIP  is responsible for building consensus within the community and documenting dissenting opinions.

This first WHIP presents a preliminary mechanism for WHIPs to empower the core team to reach design decisions more effectively. It is envisioned that this WHIP will be replaced once the process will be opened for larger parts of the community or shortcomings are identified.

# Specification 


The WHIP process begins with a new idea for WiHi. Each potential WHIP must have a champion -- someone who writes the initial WHIP using the style and format described below, shepherds the discussions in the appropriate forums, and attempts to build community consensus around the idea. The champion is also automatically an author of the WHIP.

Each WHIP has to have the following structure

- Meta-info
    - Author(s)
    - Type [technical, governance, etc.]
    - acceptance date [when decision becomes final]
    - link/ address of proposal on-chain
- Abstract [max 200 words]
- Specification [of the concrete improvement]
- Motivation [(of the authors) for proposing the improvement]
- Rationale [of design decisions within the specification]

Further (sub)-sections can be added.

The champion is the one editing the proposed WHIP, but can allow others to join editing in which case these have to be added to the list of authors.

A champion can be any community member.

The process for getting a WHIP accepted is as follows

1. The champion creates a WHIP by creating a markdown document that coheres to the above mentioned structure and by creating a pull request for this document to the WHIP repository on github
2. A moderator of the repository must then quickly review the proposal for inappropriate content and approve or reject the pull request with an explanation in the case of rejection. 
2. In case of approval, the moderator creates a corresponing "discussion" on github, and shares the document via the “WHIP” channel in discord as a thread, opening the proposal for community feedback. 
3. The official channel for providing feedback is the relevant discussion section on github; community feedback may be made by various means, but authors are only required to respond to official feedback. 
4. Champions are responsible for getting support for the WHIP (e.g. through community calls, discussions on Discord in the whip's thread, etc.).
5. A WHIP is decided on as follows
    1. The champion informs the moderator that the WHIP is ready to be decided on by stating this clearly in the corresponding github discussion. 
    1. The moderator closes the WHIP discussion and informs the WiHi community that the WHIP is ready to be decided on by stating this in the WHIP’s thread in the WHIP channel on discord. 
    2. The moderator creates a voting proposal within the realms "WiHi DAO" and informs the other core team members in a message in the WHIPs thread on Discord by tagging them and sharing the link to the vote proposal.
    2. The status of WHIPs is changed to "Voting open" by the moderator and the link to the on-chain proposal is added to the WHIP, after which no more changes can be made to the document. 
    2. The vote period is 5 days. 
    2. Each core team member can cast their vote (accept/ reject/ abstain) on-chain on the WHIP via realms. Non-voting is counted as abstaining. For the time being, core team members have one vote each and simple majority decides.  
6. After a decision has been reached, the WHIPs status on github is changed accordingly by the moderator.
7. The process is closed by the moderator sharing the final status in the WHIPs discord thread and changing its status accordingly.

An update of this process has to follow the specified process.

# Motivation

We need a mechanism to improve WiHi that can scale with WiHi's growth. We believe in crowd intelligence and individual initiative and wish to empower individuals from the community to propose ideas. Apart from this, we also want to document the reasoning behind each decision taken so that the motivation may be checked in the future and decisions modified according to changes in understanding.

We have chosen an improvement proposal system to facilitate the above as other web3 project have demonstrated it to be an effective governance tool within decentralized communities. In particular, the system is attractive because it can engage the entire DAO, with bottom-up initiatives being empowered by the fact that they must be considered by a broad group of decision makers before a decision can be made.

The core motivation for the currently illustrated WHIP process is to have a simplistic but effective process for the core team to reach decisions transparently, involving already the community. 

# Rationale

It is okay to restrict the decision making to the core team at the moment as these are the individuals that represent by far the greatest voting power in the WiHi ecosystem. As soon as other individuals will have voting power in the system, this will be adjusted with priority.

