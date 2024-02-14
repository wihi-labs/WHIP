# WHIP-4: Idea Market 

## Author(s)
[Mark Ballandies](https://twitter.com/BallandiesMC)

## Type 
Organization

# Abstract 
The idea market is a tool of the WiHi DAO to facilitate the self-organization of its community. The community can crowdsource ideas/tasks leading to WiHi's success, organize, and fund their execution in a decentralized/ bottom-up way. It is a public board illustrating tasks that need to be performed.

The idea market extends the concept of crowed-financing by splitting the mandate of execution from proposing. 

# Specification 

The tool should have the following capabilities:

1. Anyone can submit a task/ idea worth of implementation (e.g. Create a list of DePIN meetups, implement a new dashboard, create public weather station overview, etc.). For this, the following needs to be specified:
    - Title of task
    - Description of task
    - Deliverables/ Milestones
    - The reward (locked tokens for payout)
    - the percentage of rewards that the idea initiator will receive
    - the percentage of rewards that the executor(s) will receive
    - the percentage/ amount of reward that an executor will receive when picking up a task (upfrond payment), resp. after reaching a milestone
    - The reviewer(s) [those who evaluate if (sub)task(s) have been completed]
    - Mode of decision: either by reviewer evaluation or by voting of those who backed the task with tokens or by idea initiator
    - A deadline until when task has to be completed (either fixed, or dependent on starting date)
    - optional: - Category of task, link(s) to idea(s) that motivated the idea (and indication if the idea motivator acknowledges this idea as a successor, in which case backed rewards of idea motivator will be payed out if successing idea has been executed - mutable field)

2. Anyone can back an idea with WiHi or other tokens (tokens get locked in the smart contract)
3. List is sorted based on most stake 
4. Anyone can work on a task (potentially filters can be applied, e.g. a contributor, a supporter, a friend needs to do it (see WHIP-2), etc.) 
    - For this a volunteer/ a group of volunteers has to indicate willingness to work on the task by entering their public address
    - The initiator and/ or the backers (specified by initiator) accept the volunteer(s).
    - Potentially, several different groups can work on the same task (if not, task gets locked preventing others to take it). In this case, rewards might be split among all groups, resp. 
5. Once a task is completed, the volunteer(s) is/are marking it as complete (with the registered public address)
6. Reviewer checks contribution and gives recommendation (e.g. task completed, or not)
7. All people who staked tokens vote if task is completed (Optional, default: Reviewers evaluation is the decision)
    - In case of acceptance, funds are released to the executor(s) and idea generator(s)
8. In case of disagreement on the decision of the idea by backers (by anyone) in case of token-decision mode, a vote by all token holders/ the whole DAO is performed (a contester needs to stake a minimum amount of tokens, but receives a (large) compensation if his contest is accepted) 
9. Modifications
    - Potentially, several payouts for a task (e.g initial release and on completion)

In order to start the self-organization process of the WiHi DAO, for the time being, the above illustrated process will be modified such:

1. The community can crowdsource/ discuss ideas and tasks transparently in a dedicated discord channel
2. Core team enters identified tasks into a google sheet, evaluates if task has been completed and facilitates the rewarding
3. The excel is transparently shared with (subsets) of the community


# Motivation 
DAOs started out as creative centers with a lot of activity. More recently, we have observed that these organizations are becoming increasingly bureaucratic. Improvement proposals in particular are a slow and energy-consuming mechanism to achieve decisions and activities within a DAO. 

In general, Improvement Proposals are a mechanism for collective intelligence answering the ("what should be done")[https://medium.com/coinmonks/complex-systems-part-2-managing-complexity-with-bottom-up-solutions-9d6fadd88cc4] within a DAO. The idea market is a mechanism for self-organization answering the ("how things should be done")[https://medium.com/coinmonks/complex-systems-part-2-managing-complexity-with-bottom-up-solutions-9d6fadd88cc4] within a DAO and thus will complement the improvement proposal mechanism within WiHi (WHIP-1). It is a lower-level tool that enables anyone to express ideas, to work on/ execute ideas, to fund/ support ideas, and to review executions of ideas. In particular, no DAO-wide consensus need to be reached on an idea (in order for it to be added to the idea market or to be funded or executed).

Thus, it is a tool that facilitates bottom-up initiatives to be identified, funded and executed.

The idea market has been inspired by (this work)[https://link.springer.com/chapter/10.1007/978-3-319-90869-4_2]. In future it should be extended by the illustrated combination algorithm, and include more differentiated rewarding functionalities, such that both, ideas are combined such that the best emerge, and solutions are combined such that the most suitable emerges to address an idea. 


# Rationale
It is okay for the time being to have the entering and deciding right to the idea market with the core team as they are the ones representing the greatest economic stake in the ecosystem. 
