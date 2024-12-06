---
aliases:
  - Purchase Land
---
To purchase land, a **Citizen** must speak to an [[Elected Officials#Elected Official|Elected Official]] or in the case of the prospective purchaser being an [[Elected Officials#Elected Official|Elected Official]] they must determine if the [[Land]] is a [[Property#Large Property|Large Property]] and will hence require a [[Governmental Meetings|Governmental Meeting]].

The price of land is decided by taking the [[Property#Property Metric|Property Metric]] and dividing it by 8, ceilinged to an integer.
> [!math]
> $$ \begin{align*}
> & m = \text{property metric} \\
> & n = \lceil \frac{m}{8} \rceil 
> \end{align*} $$

The [[Elected Officials#Elected Official|Elected Official]] will either allocate the land or schedule a [[Governmental Meetings|Governmental Meeting]] to determine if land can be allocated. If land allocation was successful the [[Elected Officials#Elected Official|Elected Official]] must receive payment for the new [[Property]] and submit it into the [[Treasure]] (via the [[Treasure#Treasurer|Treasurer]]).

All [[Signage#Signage Requirements|Signage Requirements]] must be met for the [[Property]] to be valid.
All [[Property]] requirements must be met for the [[Property]] to be purchased.

---
## Land Anti-Mutilation Incentive
The **Land Anti-Mutilation Incentive** works to stop land from being mutilated and instead to incentivize [[Citizen|Citizens]] to build "with the land". If prospectively purchased [[Land]] will be flattened before it is constructed on, depending on the severity of flattening, the price of land is increased. 

*Variance* is defined as the difference in height of [[Landarea#Surface Blocks|Surface Blocks]].
*Total variance* is defined as the total amount of *variance* a [[Property]] has.
*Removal of variance* can occur by making actions (destroying, placing blocks) which result in *total variance* becoming smaller. Additionally, actions which almost change the *total variance*, but not quite (80% of *variance* for a particular X, Z slice of blocks removed) count as as *removing variance*.
When the *total variance* becomes 0, *variance* can no longer be removed.

For every block of *variance* (each [[Terminology Around Coordinates|Y]] level) *removed* for construction before becoming level increases (adds to) the [[Land]] price by 5 Diamonds.
> [!example]
> - Taking 5 blocks off the top of a mountain would cost (5 * 5) 25 Diamonds.
> - Taking [[Land]] which varies in height by 3 blocks and making it flat would cost (5 * 3) 15 Diamonds.

The **Land Anti-Mutilation Incentive** must also be consulted and used to charge [[Citizen|Citizens]] when changes to *variance* are prospected after [[Property]] purchase.

---
> [!example]
> - Taking 5 blocks off the top of a mountain would cost (15 * 5) 75 Diamonds.
> - Taking [[Land]] which varies in height by 3 blocks and making it flat would cost (15 * 3) 45 Diamonds.

The **Land Anti-Mutilation Incentive** must also be consulted and used to charge [[Citizen|Citizens]] when changes to land flatness are prospected after [[Property]] purchase.

---
## Anti-Inflation Incentive
The **Anti-Inflation Incentive** works to stop the value of Diamonds to inflate and hence make currency less valuable.

If a [[Citizen]] wishes to construct a staircase reaching into the ground (cumulatively 20 blocks below the surface) on their land they must pay 30 Diamonds. 

The **Anti-Inflation Incentive** must also be consulted and used to charge [[Citizen|Citizens]] when changes to underground staircase [[Property]] status are prospected after [[Property]] purchase.

---
## Underwater Land Incentive
The **Underwater Land Incentive** works to make it easier to build underwater.
#### Underwater Construction
If [[Citizen|Citizens]] anticipate to construct a [[Property#Private Property|Private Property]] where no less than 80% of the [[Property#Property Volumetric|Property Volumetric]] of the construction is underwater they will receive a 40% floored discount on their [[Property]] purchase. They will be given a book signed by an [[Elected Officials#Elected Official|Elected Official]] signifying this. If the [[Property Owner]] doesn't follow the terms of this deal after buying the [[Property]] they will owe a [[Fines|Fine]] equal to the amount of the Diamonds they were discounted to the [[Government]].
#### Under-ice Construction
If [[Citizen|Citizens]] anticipate to construct a [[Property#Private Property|Private Property]] where no less than 80% of the volume of the construction is underwater and the property is underneath [[Terminology Around Coordinates|Y]]62 in a Glacier biome and not underground they will receive a 80% floored discount on their [[Property]] purchase. They will be given a book signed by an [[Elected Officials#Elected Official|Elected Official]] signifying this. If the [[Property Owner]] doesn't follow the terms of this deal after buying the [[Property]] they will owe a [[Fines|Fine]] equal to the amount of the Diamonds they were discounted to the [[Government]].