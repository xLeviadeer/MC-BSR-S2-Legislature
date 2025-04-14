An **Election** is an event which occurs every 100 Minecraft days (on days 100, 200, 300, etc.) in which [[Citizen|Citizens]] vote on who to elect into the [[Government]] for the upcoming term (period of 100 days).

---
## Voting Early and/or Remotely
[[Citizen|Citizens]] have the [[Citizen#Right to Vote Early and Remotely|right to vote early and/or remotely]].

---
## Number of Elected Officials
A maximum of 3 elected officials is possible by default. The current [[Elected Officials]] will vote on how many elected officials should be elected in this **Election** if they believe a change is required.

---
## Voting Restrictions
#### Self Voting
[[Elected Officials]] cannot vote for themselves in a position higher than the [[#Number of Elected Officials]] in an [[Election]]. It is considered a [[Crime]] to do so.
#### Lobbying
No [[Citizen]] is allowed to lobby votes during the election. Voters must be able to vote for their preference without restrictions or bribery. This includes [[Citizen|Citizens]] promising currency rewards in any form, even indirectly as a result of voting for a particular candidate.

---
## How to Vote
To vote, a [[Citizen]] must rank the top [[Citizen|Citizens]] they believe should be elected. The number of ranks the [[Citizen]] can vote to is determined by the [[#Number of Elected Officials|amount of elected officials]] plus 2
$$ r = m + 2 \text{ where r is the amount of ranks and m is the amount of elected officials} $$
> [!example]
> 1. Joe
> 2. Mama C
> 3. Calcery

---
## Election Results
Who is elected into the [[Elected Officials#Elected Official|Elected Official]] position is decided by a *unanimity analysis*. 
A *unanimity analysis* is a calculational algorithm I (xLeviadeer) created to asses both the ranking status and unanimity of decision between choices into a unified ranking. What this does is not only account for who was highest voted, but also who was voted the most similarly between votes. This uses ideas of [Pareto Efficiency](https://en.wikipedia.org/wiki/Pareto_efficiency) and [MCDA](https://en.wikipedia.org/wiki/Multiple-criteria_decision_analysis) to find the best result.

The *unanimity analysis* will:
- Take a weighted inverse sum of each ranked [[Citizen]] in the **Election**.
- Take a weighted analysis of the unanimity of each ranked [[Citizen]] in the **Election**.
- Apply both values to a weight to find the cumulative ranking for each [[Citizen]].
	- Ranking has a weight of 0.75
	- Unanimity has a weight of 0.25

The highest finally ranked [[Citizen|Citizens]] of amount equal to the number of [[#Elected Officials]] will be successfully elected into the [[Government]] for this term. 
In the case of a tie, the tying [[Citizen|Citizens]] will be evaluated with strictly ranking. In the case that this is still a tie, the member(s) who voted before the other(s) will be elected.

---
## After the Election
After the **Election** is complete the newly [[Elected Officials]] will hold a [[Governmental Meetings|Governmental Meeting]] on who the [[Treasure#Treasurer|Treasurer]] will be.