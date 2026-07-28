---
transportation: cart pulled by pcs
speed: normal
exhaustionLevel: 0
hoursPerDay: 8
---

## Calculate speed 
`= round(160 *  ([[Transportation]].movement[[[Current Party]].transportation][[[Current Party]].speed] * choice([[Current Party]].exhaustionLevel > 1, 2, 1)) / 60 / [[Current Party]].hoursPerDay, 0)`


Round = round to nearest whole number. 160 = number of miles to travel . multiplied by the equation of  speed x exhaustion modifier  then divided by 60 and current travel hours per day.

`= [[Transportation]].movement[[[Current Party]].transportation][[[Current Party]].speed]`

This equals the speed of their transportation choice at their travel speed.

`= [[Current Party]].exhaustionLevel`

This is their exhaustion level

`= [[Current Party]].hoursPerDay`

This is how many hours per day they travel