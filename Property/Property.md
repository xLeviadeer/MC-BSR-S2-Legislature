A **Property** is a subsection of [[Land]] which is owned by either a [[Property Owner|Property Owner]] or the [[Government]].
#### Property Proximity
If a **Property** is within 12 blocks (considering only [[Terminology Around Coordinates|X]], and [[Terminology Around Coordinates|Z]] without diagonals) of another **Property** of the same [[Property Owner]] then the properties are required to be merged into one bigger **Property** where the space in-between is owned and [[Taxes|Taxed]],
#### Property Edges
A **Property** edge cannot be shorter than 5 blocks long. 
> [!example]
> A structure with top-down area of dimensions [[Terminology Around Coordinates|X]]1 by [[Terminology Around Coordinates|Z]]10 would be a **Property** of size [[Terminology Around Coordinates|X]]5 by [[Terminology Around Coordinates|Z]]10 with a [[#Property Metric]] of 50.
#### Abstractly Shaped Property
All [[Land]] which isn’t exactly rectangular must be either: 
- Included in one, larger rectangle.
- Subdivided into smaller rectangles. 
Information about what  **Abstractly Shaped Property** means when it comes to [[Property]] size can be found in [[#Property Metric]].
#### Property Verticality
**Property** only includes [[Land]] which is [[Landarea#Surface Landarea|Surface Landarea]] unless a [[Subsurface Land Provisions|Subsurface Land Provision]] has been allocated.

---
## Property Metric
**Property Metric** is always calculated as the total area of a [[Property]] from top-down (considering only [[Terminology Around Coordinates|X]], and [[Terminology Around Coordinates|Z]]). This calculated value is called **Property Metric** or simply, Metric.

> [!example]
> A property with [[Terminology Around Coordinates|X]] size 10 and [[Terminology Around Coordinates|Z]] size 10 would have a **Property Metric** of 100.

The area of subdivisional lines counts twice when calculating the [[Property#Property Metric|Property Metric]].
> [!example] 
> For an abstractly shaped property composed of two rectangles of size 10x10 and 3x4, 
> $$ (10 * 10) + (3 * 4) = 112 $$

---
## Property Volumetric
**Property Volumetric** is always calculated as the total volume of a [[Property]]. This calculated value is called **Property Volumetric** or simply, Volumetric.
> [!example]
> A property with [[Terminology Around Coordinates|X]] size 10, [[Terminology Around Coordinates|Y]] size 3 and [[Terminology Around Coordinates|Z]] size 10 would have a **Property Volumetric** of 300.

---
## Property Size
**Property Size** is a way to classify if a **Property** is "large" or "small". 
#### Small Property
A **Small Property** is a **Property** with a [[#Property Metric]] of *less than or equal to* 400.

#### Large Property
A **Large Property** is a **Property** with a [[#Property Metric]] of *more than* 400.

---
## Public Property
**Public Property** is a type of [[Land#Hard Land|Hard Land]] which is owned by the [[Government]] which all [[Citizen|Citizens]] are allowed to enter.
All [[Land#Hard Land|Hard Land]] which is not **Private Property** or **Shared Private Property** is **Public Property**. 

---
## Shared Private Property
**Shared Private Property** is a type of [[Land#Hard Land|Hard Land]] which is owned by a singular individual, [[Property Owner]], which only this individual along with a select group of other individuals are allowed to enter unless one of the following circumstances is met:
- The [[Property Owner]] gives verbal or written permission for a specific or group of [[Citizen|Citizens]] to enter their **Shared Private Property** for each case that someone wishes to enter other than the [[Property Owner]]. This rule doesn't go into effect if the [[Property Owner]] has a [[Citizen]] currently constructing something on their **Shared Private Property**.
- The [[Property Owner]] or other [[Citizen|Citizens]] residing in the **Shared Private Property** have disobeyed [[Jurisdiction]], in which case [[Elected Officials]] or [[Citizen|Citizens]] provisioned by [[Elected Officials]] can enter the **Shared Private Property**.

---
## Private Property
**Private Property** is a type of [[Land#Hard Land|Hard Land]] which is owned by a singular individual, [[Property Owner]], which only this individual is allowed to enter unless one of the following circumstances is met:
- The [[Property Owner]] gives verbal or written permission for a specific or group of [[Citizen|Citizens]] to enter their **Private Property** for each case that someone wishes to enter other than the [[Property Owner]]. This rule doesn't go into effect if the [[Property Owner]] has a [[Citizen]] currently constructing something on their **Private Property**.
- The [[Property Owner]] has disobeyed [[Jurisdiction]], in which case [[Elected Officials]] or [[Citizen|Citizens]] provisioned by [[Elected Officials]] can enter the **Private Property**.

---
## Unowned Property
**Unowned Property** is a type of [[Land#Soft Land|Soft Land]] which is owned by the [[Government]] which all [[Citizen|Citizens]] are allowed to enter.
All [[Land#Soft Land|Soft Land]] which is not [[#Owned Property]] is *not* **Unowned Property**. **Unowned Property** is typically property that has specific rules about how it should be used, imposed by the [[Government]].
Tunnels and other buildings constructed by the [[Government]] in the Nether are considered **Unowned Property**. Other portions of the Nether are considered [[Land#Free Land|Free Land]].

---
## Owned Property
**Owned Property** is a type of [[Land#Soft Land|Soft Land]] which is owned by a singular individual, [[Property Owner]], which the [[Property Owner|Owned Property Owner]] may claim who can enter the [[Property]] or not, but legally, trespassing is not against [[Jurisdiction]].