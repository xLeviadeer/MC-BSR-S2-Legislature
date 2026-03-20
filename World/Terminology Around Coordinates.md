---
aliases:
  - X
  - Y
  - Z
  - H
  - K
---
## Ordering
The order of coordinate terms, if multiple are present, should be listed in the order they are listed in below.
1. [[#Scales|Scale]]
2. [[#Spaces]]
3. [[#Positionals]]
4. [[#Wildcards]]

---
# Terms
**Terms** can be applied to any singular coordinate. When multiple singular coordinates are present it forms a coordinate, also known as a coordinate duplet or coordinate triplet.

A given singular coordinate can only have one of each [[#Terms|Term]] present; a singular coordinate cannot have two of the same [[#Terms|Term]] present.

All terms can be either capitalized or lowercase.
## Positionals
**Positionals** explain a specific Minecraft coordinate within the world.
#### **X**, **Y** and **Z** Terms
**X** references the X coordinate within the Minecraft world.
**Y** references the Y coordinate within the Minecraft world.
**Z** references the Z coordinate within the Minecraft world.

---
## Spaces
**Spaces** explain an area of space using [[#Positionals]] where at least one [[#Positionals|Positional]] is a [[#Wildcards|Wildcard]].
#### **Hori** Term
**Hori** references either [[Terminology Around Coordinates#**X**, **Y** and **Z** Terms|X]] or [[Terminology Around Coordinates#**X**, **Y** and **Z** Terms|Y]]  but not both.
**Hori** must be standalone; **Hori** must not coexist with [[Terminology Around Coordinates#**X**, **Y** and **Z** Terms|X]], [[Terminology Around Coordinates#**X**, **Y** and **Z** Terms|Y]] or [[#Wildcards]].
#### **Vert** Term
**Vert** references [[Terminology Around Coordinates#**X**, **Y** and **Z** Terms|Z]].
**Vert** must be standalone; **Vert** must not coexist with [[Terminology Around Coordinates#**X**, **Y** and **Z** Terms|Z]], or [[#Wildcards]].

---
## Wildcards
**Wildcards** explain a set of possible coordinates. **Wildcards** are usually bound by a [[#Positionals|Positional]] constraint.
#### **~** Term
**~** refers to all values of one coordinate. A blank or unlisted value means **~**.
> [!example]
> X10, Z10 would equate to all blocks from bedrock to world height on X coordinate 10 and Z coordinate 10.
> X10~ would equate to all blocks that have a value of X10.
#### **\*** Term
**\*** refers to any one specific value of a coordinate.
> [!example]
> X10, \*, Z10 would equate to any one specific block from bedrock to world height on X coordinate 10 and Z coordinate 10.

---
## Scales
**Scales** explain a multiplier to the coordinate that comes before it.
#### **H** Term
**H** refers to a coordinate with 2 trailing 0's. H, in this case, means "Hundred", hence the 2 zeros.
> [!example] 
> 22H would be the number 2,200
#### **K** Term
**K** refers to a coordinate with 3 trailing 0's.
> [!example]
> 22K would be the number 22,000