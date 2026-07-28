---
file_basename: Ride Along
file_dpath: Perks/Exploration Perks
item_id: ive-got-you
item_index: "06"
item_name: Ride Along
scc:
  - mcdm.heroes.v1:perk.exploration:ive-got-you
scdc:
  - 1.1.1:18.3:06
source: mcdm.heroes.v1
type: perk/exploration
description: Your bond with your companion has permeated your very soul; you are just as much beast as you are beastheart. You can leave behind your mortal body and join your consciousness to that of your companion. You have the Ride Along ability.
---

This perk can be taken only by beastheart characters.

Your bond with your companion has permeated your very soul; you are just as much beast as you are beastheart. You can leave behind your mortal body and join your consciousness to that of your companion. You have the following ability.

```ds-feature
type: feature
feature_type: ability
name: Ride Along
flavor: You ride behind your companion's eyes
keywords:
  - Beastheart
  - Magic
usage: Maneuver
distance: 📐 Melee 1
target: 🎯 Companion
effects:
  - name: Effect
    effect: >-
      Your body disappears, and your consciousness rides along in yoru companion's body. Whiel you are riding along, you can sense waht your companion senses and communicate with them telepathically, but you can't control them. You can't be detected, targeted, or affected by any effect. Any condition or effect on you i stemporarily negated until you regain your body.

      Whenever your companion takes damage while you are riding along, you take the same amount of damage, which can't be reduced in any way. You are unaffected by any effects that don't deal damage that affect your companion.

      While you are riding along, your companion continues to benefit from any magic treasures you are wearing.

      While you are riding along, you can't act except to spend a free maneuver to regain your body. You also regain your body if your companion dies or chooses to eject you. When you regain your body, you reappear in a space adjacent to your companion.
```