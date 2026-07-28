---
item:
  i1: "[[2. Mechanics/Items/Melee Weapons/Battleaxe.md|Battleaxe]]"
  i2: "[[2. Mechanics/Items/Adventuring Gear/Bedroll.md|Bedroll]]"
  i3: "[[2. Mechanics/Items/Ammunitions/Arrow.md|Arrow]]"
  i4: "[[2. Mechanics/Items/Melee Weapons/Dagger.md|Dagger]]"
  i5: "[[2. Mechanics/Items/Adventuring Gear/Waterskin.md|Waterskin]]"
  i6: "[[2. Mechanics/Items/Adventuring Gear/Alchemist's Fire (flask).md|Alchemist's Fire (flask)]]"
  i7: "[[2. Mechanics/Items/Treasures/Gold (gp).md|Gold (gp)]]"
  i8: "[[2. Mechanics/Items/Adventuring Gear/Silk Rope (50 feet).md|Silk Rope (50 feet)]]"
num:
  i1: 2
  i2: 1
  i3: 20
  i4: 3
  i5: 1
  i6: 4
  i7: 1000
  i8: 1
---
# Inventory Mock up

| Name                                                          |                  Amount                  |                              Value                               |                               Weight                               |
| ------------------------------------------------------------- |:----------------------------------------:|:----------------------------------------------------------------:|:------------------------------------------------------------------:|
| `INPUT[suggester(optionQuery("6. Mechanics/Items")):item.i1]` | `INPUT[number(class(nb-mb-css)):num.i1]` | `$=dv.page(dv.current().item.i1).value * dv.current().num.i1` gp | `$=dv.page(dv.current().item.i1).weight * dv.current().num.i1` lbs |
| `INPUT[suggester(optionQuery("6. Mechanics/Items")):item.i2]` | `INPUT[number(class(nb-mb-css)):num.i2]` | `$=dv.page(dv.current().item.i2).value * dv.current().num.i2` gp | `$=dv.page(dv.current().item.i2).weight * dv.current().num.i2` lbs |
| `INPUT[suggester(optionQuery("6. Mechanics/Items")):item.i3]` | `INPUT[number(class(nb-mb-css)):num.i3]` | `$=dv.page(dv.current().item.i3).value * dv.current().num.i3` gp | `$=dv.page(dv.current().item.i3).weight * dv.current().num.i3` lbs |
| `INPUT[suggester(optionQuery("6. Mechanics/Items")):item.i4]` | `INPUT[number(class(nb-mb-css)):num.i4]` | `$=dv.page(dv.current().item.i4).value * dv.current().num.i4` gp | `$=dv.page(dv.current().item.i4).weight * dv.current().num.i4` lbs |
| `INPUT[suggester(optionQuery("6. Mechanics/Items")):item.i5]` | `INPUT[number(class(nb-mb-css)):num.i5]` | `$=dv.page(dv.current().item.i5).value * dv.current().num.i5` gp |  `$=dv.page(dv.current().item.i5).weight * dv.current().num.i5` lbs |
| `INPUT[suggester(optionQuery("6. Mechanics/Items")):item.i6]` | `INPUT[number(class(nb-mb-css)):num.i6]` | `$=dv.page(dv.current().item.i6).value * dv.current().num.i6` gp |  `$=dv.page(dv.current().item.i6).weight * dv.current().num.i6` lbs |
| `INPUT[suggester(optionQuery("6. Mechanics/Items")):item.i7]` | `INPUT[number(class(nb-mb-css)):num.i7]` | `$=dv.page(dv.current().item.i7).value * dv.current().num.i7` gp |  `$=dv.page(dv.current().item.i7).weight * dv.current().num.i7` lbs |
| `INPUT[suggester(optionQuery("6. Mechanics/Items")):item.i8]` | `INPUT[number(class(nb-mb-css)):num.i8]` | `$=dv.page(dv.current().item.i8).value * dv.current().num.i8` gp |  `$=dv.page(dv.current().item.i8).weight * dv.current().num.i8` lbs |
