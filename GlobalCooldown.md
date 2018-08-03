# Global Cooldown

The Global Cooldown (GCD) limits casting spells.

## Possible types

There are different types of GCDs, the type affecting you depends **not on your spec but is spell-specific**. Most spells within a spec will have similar GCDs, but very few specs are 100% consistent.

### Scaling GCD

Some spells scale with Haste. Calculating a scaling GCD can be done using this formula:

```
GCD = base duration / (100% + Haste %)
```

If your base duration is the common 1.5sec, the formula would be `GCD = 1.5 / (100% + Haste %)`. If you have 15% Haste your GCD would be `1.5 / (100% + 15%)` = 1.3sec.

Scaling GCDs have a minimum GCD of 0.75sec. This minimum is the same for spells with a base duration of 1.5 sec and 1 sec.

### Static GCD

Some spells have a static GCD, unaffected by Haste. These types of spells are most common on energy-based classes and specs such as Hunters, Rogues, Monks and Feral Druids. None of the specs mentioned are 100% consistent, most spells have a 1 sec static GCD, but some spells have scaling GCDs with a 1 sec base, and some scale with a 1.5 sec base.

### Off the GCD

Some spells are off the GCD. 

### Spell/group specific GCD

Some spells, such as a Brewmaster Monk's brews, have a GCD that only affect the spell being cast.

## Determining the GCD

Using this macro you can see the GCD of each spell as you cast it:
```
/run GCDE=GCDE or CreateFrame('FRAME', 'GCDE');GCDE:RegisterEvent('UNIT_SPELLCAST_SUCCEEDED');GCDE:SetScript('OnEvent', function (_,_,_,_,id) print(select(1,GetSpellInfo(id))..":",(select(2,GetSpellCooldown(id)))*1000);end);
```
*1. `UNIT_SPELLCAST_SUCCEEDED` only works for instant casts, replace it with `UNIT_SPELLCAST_START` for cast time abilities.

Cast a spell and the macro will print the GCD of the ability. If it's a nice round number, it's generally a static GCD. If it's something like `1431` (and your Haste is low) it's safe to assume it has a base GCD of 1500 that scales with Haste. `963` would suggest 1000ms-haste, `1000` would suggest static.
