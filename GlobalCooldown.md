# Global Cooldown

The Global Cooldown (GCD) limits casting spells. There are different types of GCDs, the type affecting you depends **not on your spec but is spell-specific**. Most spells within a spec will have similar GCDs, but very few specs are 100% consistent.

## Scaling GCD

Some spells scale with Haste. Calculating a scaling GCD can be done using this formula:

```
GCD = base duration / (100% + Haste %)
```

If your base duration is the common 1.5sec, the formula would be `GCD = 1.5 / (100% + Haste %)`. If you have 15% Haste your GCD would be `1.5 / (100% + 15%)` = 1.3sec.

Scaling GCDs have a minimum. In the case of 1.5sec this is 0.75sec. I'm unsure if the minimum is always 0.75sec, or 50% of the base duration. Looking at specs with a 1 sec base GCD duration, it looks like it's a static 0.75sec minimum.

## Static GCD

Some spells have a static GCD, unaffected by Haste. These types of spells are most common on energy-based classes and specs such as Hunters, Rogues, Monks and Feral Druids. None of the specs mentioned are 100% consistent, most spells have a 1 sec static GCD, but some spells have scaling GCDs with a 1 sec base, and some scale with a 1.5 sec base.

## Off the GCD

Some spells are off the GCD. 

## Spell/group specific GCD

Some spells, such as a Brewmaster Monk's brews, have a GCD that only affect the spell being cast.
