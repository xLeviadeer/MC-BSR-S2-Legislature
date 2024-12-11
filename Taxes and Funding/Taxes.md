**Taxes** are the idea that [[Citizen|Citizens]] must pay a sum of Diamonds to the [[Government]] where they are put into the [[Treasure]]. The Diamonds in the [[Treasure]] are then used to fund [[Assignments#Public Assignments|Public Assignments]] which work to better all or a majority of [[Citizen|Citizens]].

---
## Tax Period
Every 10 Minecraft days, if a [[Citizen]] has played for a sum of more than 10 real minutes--not including time AFKing--they are [[Citizen#Requirement to Pay Taxes and Fines|required to pay their taxes]] within a 1 Minecraft day period of when they are next on the [[World]] or not AFK.
AFKing is defined as not speaking, moving or involving with the [[World]]. 
The taxpayer, [[Citizen]], must following the proper [[#Taxpaying Process]].

---
## Taxpaying Process
A [[Citizen]] will receive a signed book which explains how much they owe in **Taxes** in their [[Property Owner#Mailbox Construction and Placement|mailbox]]. They must deliver the signed tax book and the required amount of Diamonds to a *Public Tax Mailbox* within the [[#Tax Period|tax period deadline]]. Tax books should be discarded via destruction (cactus, lava, fire) when they are completed or stored in a vault.

Taking Diamonds or signed tax books from a *Public Tax Mailbox* for personal use (not moving the tax money to the [[Treasure]]) is considered a [[Crime]].

A *Public Tax Mailbox* is a [[Property Owner#Mailbox Construction and Placement|mailbox]] which follows all [[Property Owner#Mailbox Construction and Placement|Mailbox Construction and Placement]] rules but is located in [[Property#Public Property|Public Property]] and owned by the [[Government]] for use in collecting **Taxes**.

**Taxes** aren't due on time (within the [[#Tax Period|tax period deadline]]) if the [[Citizen]] who pays the **Taxes** is [[Crime#Imprisonment|Imprisoned]]. Instead, the **Taxes** are due 15 days after they leave [[Crime#Imprisonment|prison]].

---
## Tax Calculation Process
To calculate **Taxes** a [[Citizen]] should:
1. Compute the [[Property#Property Metric|Property Metric]] for all [[Property|Properties]] they own. 
2. Apply [[#Implicit Tax Incentives]] to the [[Property#Property Metric|Property Metrics]]. 
3. Calculate the [[#Default Tax Amount]].
4. Apply the [[#Circumstantial Tax Value]] to their [[#Default Tax Amount]].
5. If there are any [[Crime#Tax Increase|Tax Increases]] they should be applied after everything else.

What this means is that:
- Taxes mainly get larger as the size of a [[Citizen]]'s [[Property#Private Property|Private Property]], [[Property#Shared Private Property|Shared Private Property]] or [[Property#Owned Property|Owned Property]] gets larger *without considering height*.
- [[Elected Officials]] can *partially* control how much money you pay in [[Taxes]].
- Destroying your ([[Property Owner]]'s) [[Property]] can result in increases in taxes and pricing. *Even though you own the property*; you are buying a sub-lease from the [[Government]].
- Buying [[Property]] in certain areas is less expensive or more expensive.
- [[Citizen|Citizens]] with no [[Property]] owe less taxes than those with [[Property#Large Property|Large Property]] but owe more than those with [[Property#Small Property|Small Property]]. 

---
## Default Tax Amount
The **Default Tax Amount** is the amount of **Taxes** that is paid by default.

If a **Default Tax Amount** comes out with more than 2 decimals, it should be rounded to 2 decimal places.
#### For Citizens who are *not* Property Owners
[[Citizen|Citizens]] who are not [[Property Owner|Property Owners]] owe the [[Government]] a tax of 3 Diamonds for every 27 stacks of items they own in storage containers (not including chests, shulker boxes and ender chests).
> [!math]
> $$ \begin{align*}
>  & \text{Let } m \text{ be the amount of item stacks a player stores in containers at their Primary Residence.} \\
> \\
> & \text{Let } d = \lfloor \frac{m}{27} \rfloor * 3 \text{ be the final, default tax amount a Citizen owes.} \\
> \end{align*} $$

If a [[Citizen]] is not a [[Property Owner]] and also doesn't own at least 27 stacks of items in storage containers (not including chests, shulker boxes and ender chests) they owe a flat value of 5 Diamonds to the [[Government]]. This counts as a **Default Tax Amount**.

 a stack is defined as a Minecraft item slot which contains something.
#### For Citizens who are Property Owners
The equation below describes how to tax [[Citizen|Citizens]] with different types of [[Property|Properties]]. 
Generally speaking:
- [[Property#Private Property|Private Property]] [[Property Owner|Owners]] owe the default tax value
- [[Property#Shared Private Property|Shared Private Property]] [[Property Owner|Owners]] owe extra tax based on the number of members who have resided (slept, stored, or used as their [[Citizen#Right to be Issued a Primary Residence|primary residence]]) in their [[Property#Shared Private Property|Shared Private Property]].
- [[Property#Owned Property|Owned Property]] [[Property Owner|Owners]] owe 130% the taxes of a [[Property#Private Property|Private Property]] [[Property Owner|Owner]]. 
> [!math]
> $$
> \begin{align*}
> & \text{Let } P = [p_1, p_2, ..., p_n] \text{ be a list which represents each property metric a Citizen owns} \\
> & \text{where incentives have already been applied.} \\
> \\
> & \text{Let } R = [r_1, r_2, ..., r_n] \text{ be a list which represents the number of residents which have resided in} \\ 
> & \text{each Shared Private Property a Citizen owns.} \\
> & \text{If a Property isn't a Shared Private Property, the value of r should be a default value, 0.} \\
> \\
> & \text{Let }f(p, r) = \begin{cases}
> 	\frac{p}{200}, & \text{if Property is a Private Property} \\
> 	\frac{p}{200} * (1 + \frac{r}{10}), & \text{if Property is a Shared Private Property} \\
> 	\frac{p}{100}, & \text{if Property is an Owned Property} \\
> \end{cases} \\
> & \text{describe the operation to be performed on a Citizen's Property} \\
> & \text{based on what kind of Property the particular property the Citizen owns is.} \\
> \\
> & \text{Let } d = \sum_{i}f(P_i, R_i) \text{ be the default tax amount a Citizen owes.}
> \end{align*}
> $$

---
## Circumstantial Tax Value
The **Circumstantial Tax Value** is a value which modifies the [[#Default Tax Amount]] after all calculations. The **Circumstantial Tax Value** starts at 0.00 and can be [[Elected Officials#Adjust the Circumstantial Tax Value|adjusted by elected officials]] in increments of 0.05 per [[Elected Officials#Elected Official|Elected Official]]. The **Circumstantial Tax Value** is calculated via the equation below. The **Circumstantial Tax Value** cannot go below -0.75 and cannot exceed 3. Attempts to do so will result in no change.
> [!math]
> $$ \begin{align*} 
> & \text{Let } c \text{ be the Circumstantial Tax Value} \\
> & \text{Let } d \text{ be the Default Tax Amount} \\
> \\
> & \text{Let } t = \lceil (c + 1) * d \rceil \text{ be the total tax amount} 
> \end{align*} $$

---
## Implicit Tax Incentives
**Implicit Tax Incentives** are motives to build or not build in certain [[Landarea]] by increasing or decreasing taxes in said [[Landarea]].

**Implicit Tax Incentives** may also be referred to as Incentives or Incentives Programs.

If a [[Property#Property Metric|Property Metric]] with all applicable incentives applied comes out with more than 2 decimals, it should be rounded to 2 decimal places.

All increases and decreases are added together before being applied to the [[Property#Property Metric|Property Metric]] of the [[Property]]. The formula below describes how to compute incentives.
> [!math]
> $$ \begin{align*}
> & \text{Let } x \text{ be the Property Metric of any given Property.} \\
> & \text{Let } U \text{ be a multiset containing 1 and all applicable incentive values.} \\
> \\
> & \text{Let } p = x * (1 + (\sum_{i} U_i)) \text{ be the Property Metric with all applicable incentives applied.}
> \end{align*} $$

---
#### Below the Ice Incentive
The **Below the Ice Incentive** aims to incentivize [[Citizen|Citizens]] to build under the ice and disincentivize them from building above the ice.

[[Property]] which does not have ice above, below or inside of it is not considered in this incentive. 
###### For Property Owners Under the Ice
[[Property Owner|Property Owners]] who own [[Property]] *under the ice* get a 30% reduction in **Taxes**. 
*Under the ice* is defined as [[Property]] which is underneath the ice in a glacier biome, not underground and leaves an at least 1 block gap between the ice and the property ([[Terminology Around Coordinates|Y]]61 inclusive).
[[Property|Properties]] with larger (95% or more [[Property#Property Volumetric|volumetric]]) portions *above the ice* are not considered *under the ice*.
$$ u \cup \{-0.3\} $$
###### For Property Owners On or Above the Ice
[[Property Owner|Property Owners]] who own [[Property]] *above the ice* get a 30% increase in **Taxes**.
*Above the ice* is defined as [[Property]] which is above the ice ([[Terminology Around Coordinates|Y]]64 inclusive) which at least 1 block of sits anywhere above the ice in a glacier biome.
[[Property|Properties]] with larger (95% or more [[Property#Property Volumetric|volumetric]]) portions *under the ice* are not considered *above the ice*.
$$ u \cup \{0.3\} $$
###### For Property Owners who Puncture the Ice
[[Property Owner|Property Owners]] who own [[Property]] *puncturing the ice* get a 15% increase in **Taxes**.
*Puncturing the ice* is defined as [[Property]] which is at least partially in the ice ([[Terminology Around Coordinates|Y]]62 - 63 inclusive) inside of a glacier biome.
$$ u \cup \{0.15\} $$
---
#### Private Property over Owned Property Incentive
The **Private Property over Owned Property Incentive** aims to incentivize [[Citizen|Citizens]] to build within [[Land#Hard Land|Hard Land]]. 

[[Property#Owned Property|Owned Property]] gets a 30% increase in **Taxes**. 
$$ u \cup \{0.30\} $$

