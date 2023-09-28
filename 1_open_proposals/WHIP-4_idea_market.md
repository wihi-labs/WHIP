# WHIP-4: Idea Market 

## Author(s)
[Mark Ballandies](https://twitter.com/BallandiesMC)

## Type 
Organization

# Abstract 
The idea market is a tool of the WiHi DAO to harness the collective intelligence and facilitate the self-organization of its community. The community can crowdsource ideas/tasks leading to WiHi's success and fund their execution in a decentralized/ bottom-up way. It is a public board illustrating tasks that need to be performed.

# Specification 

The tool should have the following capabilities:

1. Anyone can submit a task/ idea worth of implementation (e.g. Create a list of DePIN meetups, implement a new dashboard, create public weather station overview, etc.). For this, the following needs to be specified:
- Title of task
- Description of task
- Category of task (optional)
- Deliverables/ Milestones
- The reward (lock tokens for payout)
- The reviewer(s) [those who evaluate if task has been completed]
- Mode of decision: either by reviewer evaluation or by voting of those who backed the task with tokens
- A deadline until when task has to be completed (either fixed, or dependent on starting date)

2. Anyone can back an idea with WiHi or other tokens (tokens get locked in the smart contract)
3. List is sorted based on most stake 
4. Anyone can work on a task (potentially filters can be applied, e.g. a contributor, a supporter, a frieds needs to do it (see WHIP-2), etc.) 
- For this a volunteer/ a group of volunteers has to indicate willingness to work on the task by entering their public address
- The initiator and/ or the backers (specified by initiator) accept the volunteer(s) (task gets locked preventing others to take it)
5. Once a task is completed, the volunteer(s) is marking it as complete (with the registered public address)
6. Reviewer checks contribution and gives recommendation (e.g. task completed, or not)
7. All people who staked tokens vote if task is completed (Optional, default: Reviewers evaluation is the decision)
- In case of acceptance, funds are released to the implementor
8. In case of disagreement on the decision of the idea by backers (by anyone) in case of token-decision mode, a vote by all token holders/ the whole DAO is performed (a contester needs to stake a minimum amount of tokens, but receives a (large) compensation if his contest is accepted) 
9. Modifications
- Potentially, several payouts for a task (e.g initial release and on completion)

In order to start the collective intelligence and self-organization process of the WiHi DAO, for the time being, the above illustrated process will be modified such:

1. The community can crowdsource/ discuss ideas and tasks transparently in a dedicated discord channel
2. Core team enters identified tasks into an excel, evaluates if task has been completed and facilitates the rewarding
3. The excel is transparently shared with the community


# Motivation 

Collective intelligence and self-organizaiton have been identified to govern and control complex systems more effectively than top-down approaches (e.g. see [1](https://www.researchgate.net/publication/364949613_Democracy_by_Design_Perspectives_for_Digitally_Assisted_Participatory_Upgrades_of_Society) and [2](https://link.springer.com/book/10.1007/978-3-030-62330-2)) as demonstrated for instance by Bitcoin.
The idea market will complement the improvement proposal mechanism (WHIP-1) to develop the WiHi system. In particular, it is a lower-level tool that enables anyone to express ideas, to reason about them in privacy, and to see transparently the activities/ tasks at hand to make WiHi a success (as required for collective intelligence, see [3](https://medium.com/coinmonks/complex-systems-part-2-managing-complexity-with-bottom-up-solutions-9d6fadd88cc4)). Moreover, it enables anyone to act and to provide feedback to the system (as required for self-organization, see [3](https://medium.com/coinmonks/complex-systems-part-2-managing-complexity-with-bottom-up-solutions-9d6fadd88cc4)).


# Rationale
It is okay for the time being to have the entering and deciding right to the idea market with the core team as they are the ones representing the greates economic stake in the ecosystem. 