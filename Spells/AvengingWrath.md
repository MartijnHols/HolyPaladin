# Avenging Wrath

[![image](https://user-images.githubusercontent.com/4565223/39927328-26cc3b7e-5532-11e8-9d05-45140e534a4d.png)](https://beta.wowdb.com/spells/31884-avenging-wrath)

- Baseline
- Throughput cooldown
- Self-cast
- 0 mana
- **Static** cooldown (unaffected by Haste)
- Instant - GCD

## About

Increases your damage, healing and critical strike chance by 30%* for a few seconds.

See also tier 90: [Sanctified Wrath](Talents/90/SanctifiedWrath.md), [Avenging Crusader](Talents/90/AvengingCrusader.md) and [Awakening](Talents/90/Awakening.md).

\* The tooltip on Wowhead/WoWDB will show only a 20% bonus because this is the default for the class, but the Holy Paladin spec gains another 10% from [the spec passive](https://beta.wowdb.com/spells/137029).

### Math

Avenging Wrath increases both healing and critical strike chance by 30%, to calculate its value we need to account for both. The base healing is 100%, the healing increase adds a simple 30%, increasing the total to 130% (that was the easy part).

A critical strike causes a 100% increase of the total healing done, which would make the heal do 260%. But we only get 30% crit chance, so to calculate the gain from the crit chance we need to average it out. We do this by taking the gain from a crit (100% increased healing) and multiplying it by the crit chance (30%). This giving us: `100% * 30% =` 30% average healing gain from crits. Since all heals have a 100% base (the healing of a regular, non crit, heal), the average crit is bonus is 130%.

To get the total gain from Avenging Wrath we can multiply the two values giving us a total gain of `130% * 130% =` 169% before overhealing. The total formula is `regular healing * (base + healing gain) * (regular hit + (crit gain * crit chance))` = `100% * (100% + 30%) * (100% + (100% * 30%))` = 169%.

## Changes since Legion

- Put on the GCD

## Bugs

- Swapping to Avenging Crusader while Avenging Wrath is on cooldown, allows you to cast AC right away #1
- The critical strike gain is not shown in the character pane.
- [Sanctified Wrath](Talents/90/SanctifiedWrath.md) does not currently apply the HS cooldown reduction.
