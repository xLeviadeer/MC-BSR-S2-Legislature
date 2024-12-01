**Taxes** are the idea that [[Citizen|Citizens]] must pay a sum of Diamonds to the [[Government]] where they are put into the [[Treasure]]. The Diamonds in the [[Treasure]] are then used to fund [[Assignments#Public Assignments|Public Assignments]] which work to better all or a majority of [[Citizen|Citizens]].

---
## Tax Period
Every 10 Minecraft days, if a [[Citizen]] has played for a sum of more than 10 real minutes--not including time AFKing--they are [[Citizen#Requirement to Pay Taxes and Fines|required to pay their taxes]] within a 1 Minecraft day period of when they are next on the [[World]] or not AFK.
AFKing is defined as not speaking, moving or involving with the [[World]]. 
The taxpayer, [[Citizen]], must following the proper [[#Taxpaying Process]].

---
## Taxpaying Process
A [[Citizen]] will receive a signed book which explains how much they owe in taxes in their [[Property Owner#Mailbox Construction and Placement|mailbox]]. They must deliver the signed tax book and the required amount of Diamonds to a *Public Tax Mailbox* within the [[#Tax Period|tax period deadline]]. Tax books should be discarded via destruction (cactus, lava, fire) when they are completed or stored in a vault.

Taking Diamonds or signed tax books from a *Public Tax Mailbox* for personal use (not moving the tax money to the [[Treasure]]) is considered a [[Crime]].

A *Public Tax Mailbox* is a [[Property Owner#Mailbox Construction and Placement|mailbox]] which follows all [[Property Owner#Mailbox Construction and Placement|Mailbox Construction and Placement]] rules but is located in [[Property#Public Property|Public Property]] and owned by the [[Government]] for use in collecting **Taxes**.

---
## Default Tax Amount
The **Default Tax Amount** is the amount of **Taxes** that is paid by default.
#### For Citizens with No Property
[[Citizen|Citizens]] who are not [[Property Owner|Property Owners]] owe the [[Government]] a tax of 3 Diamonds for every 27 stacks of items they own in storage containers where a stack is defined as a Minecraft item slot which contains something.
> [!math]
> $$ \begin{align*}
> & s = \{\text{each set of 27 stacks}\} \\
> & d = 3 * \sum_{i} i_s
> \end{align*} $$
#### For Private Property Owners
[[Property Owner|Property Owners]] must pay the sum of all of their [[Property#Property Metric|Property Metrics]] (p) for all of their properties divided by 200 in Diamonds and all ceilinged.
> [!math]
> $$
> \begin{align*}
> & p = \{\text{all property metrics}\} \\
> & d = \lceil \frac{\sum_{i} p_i}{200} \rceil
> \end{align*} $$
#### For Shared Private Property Owners
[[Property Owner|Property Owners]] who own a [[Property#Shared Private Property|Shared Private Property]] must pay the sum of all their [[Property#Property Metric|Property Metrics]] (p) for all of their properties divided by 200 all multiplied by 1 plus the number of [[Citizen|Citizens]] who have resided (slept, stored, or used as their [[Citizen#Right to be Issued a Primary Residence|primary residence]]) in the [[Property Owner]]'s [[Property#Private Property|Private Property]] (r) divided by 10 and all ceilinged.
> [!math]
> $$ \begin{align*}
> & p = \{\text{all property metrics}\}
> & r = \{\text{all residents}\} \\
> & d = \lceil \frac{\sum_{i} p_i}{200} * (1 + \frac{\sum_{i} r_i}{10}) \rceil 
> \end{align*}
> $$
#### For Owned Property Owners
[[Property Owner|Property Owners]] who own an [[Property#Owned Property|Owned Property]] must pay the sum of all their [[Property#Property Metric|Property Metrics]] (p) for all of their properties divided by 200 all multiplied by 2 and all ceilinged.
> [!math]
> $$ \begin{align*}
> & p = \{\text{all property metrics}\} \\
> & d = \lceil \frac{\sum_{i} p_i}{200} * 2 \rceil 
> \end{align*}
> $$

---
## Circumstantial Tax Value
The **Circumstantial Tax Value** is a value which modifies the [[#Default Tax Amount]] after all calculations. The **Circumstantial Tax Value** (c) + 1 is multiplied by the [[#Default Tax Amount]] (d) and ceilinged.
> [!math]
> $$ \begin{align*} 
> & c = \text{Circumstantial Tax Value} 
> & d = \text{Default Tax Amount} \\
> & t = \lceil (c + 1) * d \rceil 
> \end{align*} $$

[[Elected Officials]] have the ability to adjust the **Circumstantial Tax Value** on each [[#Tax Period]].

---
## Implicit Tax Incentives
**Implicit Tax Incentives** are motives to build or not build in certain [[Landarea]] by increasing or decreasing taxes in said [[Landarea]].
#### Below the Ice Incentive
The **Below the Ice Incentive** aims to incentivize [[Citizen|Citizens]] to build under the ice and disincentivize them from building above the ice.

[[Property]] which does not have ice above, below or inside of it is not considered in this incentive. 

All increases and decreases are added together before being applied to the total tax amount; the tax amount after applying the [[#Circumstantial Tax Value]] and ceilinged.
> [!math]
> $$ \begin{align*}
> & t = \text{total tax amount}
> & u = \{1, \text{and all applied incentive values}\} \\
> & f = \lceil t * (\sum_{i} u_i) \rceil
> \end{align*} $$
###### For Property Owners Under the Ice
[[Property Owner|Property Owners]] who own [[Property]] *under the ice* get a 30% reduction in **Taxes**. 
*Under the ice* is defined as [[Property]] which is underneath the ice and leaves an at least 1 block gap between the ice and the property ([[Terminology Around Coordinates|Y]]61 inclusive).
$$ u \cup \{-0.3\} $$
###### For Property Owners On or Above the Ice
[[Property Owner|Property Owners]] who own [[Property]] *above the ice* get a 30% increase in **Taxes**.
*Above the ice* is defined as [[Property]] which is above the ice ([[Terminology Around Coordinates|Y]]64 inclusive).
$$ u \cup \{0.3\} $$
###### For Property Owners who Puncture the Ice
[[Property Owner|Property Owners]] who own [[Property]] *puncturing the ice* get a 15% increase in **Taxes**.
*Puncturing the ice* is defined as [[Property]] which is at least partially in the ice ([[Terminology Around Coordinates|Y]]62 - 63 inclusive).
$$ u \cup \{0.15\} $$