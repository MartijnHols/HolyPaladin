# Beacon of Light

[![Tooltip](https://user-images.githubusercontent.com/4565223/39920688-34f30756-5518-11e8-85b9-8a510ff5e409.png)](https://beta.wowdb.com/spells/53563-beacon-of-light)

- Baseline
- Buff (permanent)
- Any ally
- 500 mana
- Instant - GCD

## About

Places a beacon on a target, transferring a percentage of your **raw healing done** to this target. Healing your Beacon of Light target directly will not transfer any healing through that beacon. Casting [Flash of Light](./FlashOfLight.md) or [Holy Light](./HolyLight.md) on a beacon target will refund some of its mana cost, but it is generally less efficient to directly heal a beacon target due to missing out on the beacon transfer healing.

## Interactions

AoE spells transfer healing to beacons at a reduced 50% efficiency. The exact efficiency amounts are:

| Spell | Efficiency |
| ----- | ---------: |
| Holy Shock | 100% |
| Light of Dawn | 50% |
| Holy Light | 100% |
| Flash of Light | 100% |
| Holy Prism (casting on an enemy) | 50% |
| Holy Prism (direct healing friendly) | 100% |
| Light's Hammer | 50% |
| Tyr's Deliverance | 100% |
| Bestow Faith | 100% |
| Light of the Martyr (Maraad's) | 100% |
| Avenging Crusader | 100% |

Beacon of Light healing does not double-dip from any stats; all stat interactions happen on the original heal. The transferred amount is always 40% (or 28% with Beacon of Faith) of the original raw heal.

For Mastery this means your effectiveness depends on the distance to the original heal's target and not to your beacon. In other words, if your [Holy Shock](./HolyShock.md) had 100% Mastery Efficiency on its target, the beacon transfer heal will match that efficiency regardless of the beacon target being 50 yards away or not.

## Range

![Illustration](/Assets/BeaconTargeting.jpg)

- Requires the Beacon of Light to be within line of sight of the Paladin
- Does **not** require the target being healed to be within line of sight of the Beacon of Light
- Requires the Beacon of Light to be within 60 yards of the Paladin (even if the target being healed is closer)
- Does **not** require the Beacon of Light to be within 60 yards of the target being healed
- Requires the Paladin to be in the same phase as the beacon
