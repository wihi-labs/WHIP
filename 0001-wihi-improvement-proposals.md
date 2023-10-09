# WHIP-1: WiHi Improvement proposals

## Author(s):

[Mark Ballandies](https://twitter.com/BallandiesMC)

## Type

Governance

# Abstract 

A WiHi Improvement Proposal (WHIP) is a (technical) design document providing information to the WiHi community, or describing a new feature for WiHi or its processes or environment. The WHIP should provide a concise (technical) specification of the feature and a motivation for the feature.

We intend WHIPs to be the primary mechanisms for proposing new features, for collecting community input on an issue, and for documenting the design decisions that have gone into WiHi. The WHIP champion is responsible for building consensus within the community and documenting dissenting opinions.

WHIP-1 is sketching a preliminary mechanism for WHIPs to empower the core team to reach design decisions of WiHi more efficiently. It is envisioned that this WHIP will be replaced once the process will be opened for larger parts of the community or shortcomings are identified.

# Specification 

The WHIP process begins with a new idea for WiHi. Each potential WHIP must have a champion -- someone who writes the initial WHIP using the style and format described below, shepherds the discussions in the appropriate forums, and attempts to build community consensus around the idea. The champion is also automatically an author of the WHIP.

Each WHIP has to have the following structure

- Meta-infos
    - Author(s)
    - Type [technical, governance, etc.]
    - acceptance date [when accepted and moved to closed_proposals folder]
- Abstract [max 200 words]
- Specification [of the concrete improvement]
- Motivation [(of the authors) for proposing the improvement])
- (Rationale [of design decisions within the specification])

Further (sub)-sections can be added.

The champion is the one editing the proposed WHIP, but can allow others to join editing in which case these have to be added to the list of authors.

For the time being, a champion has to be a core team member. 

The process for getting an WHIP accepted is as follows

1. The champion creates a WHIP by creating a markdown document that coheres to the above mentioned structure and by creating a pull request for this document to the WHIP repository on github
2. A moderator accepts the pull request and creates a corresponding "issue"
2. The moderator shares with others the document via the “WHIP” channel in discord as a thread. 
3. Official Comments *in writing* of the WHIP which must be adressed by the author will be performed via the corresponding "issue" on github
4. The champions are responsible for obtaining support of the WHIP (e.g. via community calls, discussions on discord in the whip's thread, etc.)
5. A WHIP is decided on as follows
    1. The champion informs the core team that the WHIP is ready to be decided on by stating this clearly in the WHIP’s thread in the WHIP channel on discord. In the notification, the champion must
        - either state the result of the decision (accepted/ rejected) 
        - or open the voting process on the WHIP.
    2. WHIPs status is changed to "Voting Open" by a moderator
    2. In either of the two cases, a consolidation phase starts:
        - In case i) (stated result) a one week consolidation phase starts. The decision gets accepted if no core-team member raises a veto in the discord thread of the WHIP or if all core team members approve the decision within the consolidation phase. In case of a veto, the voting process starts with the two week consolidation phase starting from the moment where the veto has been raised.
        - In case ii) each team member can cast their vote (accept/ reject/ abstain) via the discord thread of the WHIP. Non-voting is counted as abstaining. For the time being, core team members have one vote each and simple majority decides.  
6. After a decision has been reached, the WHIP is moved to the “2_closed_proposal” folders, in the title of the WHIP in square brackets the decision is noted (e.g. WHIP-1: improvement proposals [ACCEPTED]), and a pdf has to be created of it. The name of the WHIP is as follows: WHIP-X-short-title-[accepted/ rejected]
The WHIP is accepted after the link to the pdf has been shared via the discord thread of that WHIP. Afterwards the thread has to be closed. 
7. A moderator changes the status of the WHIP to the corresponding status on github.

An update of this process has to follow the specified process.

# Motivation

As agreed in the team call at September 26th, 2023, we want to have WHIPs as the main tool to structure our thoughts and find agreement on system design features and system development. In particular, WHIPs have the purpose to inform (new) community members about the taken decisions that resulted in the current system layout.

An improvement proposal system has been chosen to facilitate this as it has been demonstrated by other web3 systems to be effective to govern decentralized communities. In particular, it is a tool that enables bottom-up initiatives to foster a top-level decision of the WiHi DAO which has to be followed/ implemented by all members. 

The core motivation for the currently illustrated WHIP process is to have a simplistic but effective process for the core team to reach decisions transparently, involving already the community. 

# Rationale

It is okay to restrict the decision decision making to the core team at the moment as these are the individuals that represent by far the greatest voting power in the WiHi ecosystem. As soons as other individuals will have voting power in the system, this will be adjusted with priority.

