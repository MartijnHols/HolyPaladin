# Aura of Sacrifice

[![image](https://user-images.githubusercontent.com/4565223/39911152-b82be084-54fa-11e8-8c3b-dce2defa8132.png)](https://beta.wowdb.com/spells/183416-aura-of-sacrifice)

- Tier 60 talent
- Passive (aura)
- Boosted by [Aura Mastery](../../AuraMastery.md)

## About the Aura Mastery effect

During [Aura Mastery](../../AuraMastery.md) this transfers 30% of damage taken by allies to you, so long as your health stays above 75% ([log](https://www.warcraftlogs.com/reports/GA97YqgtyVzJNbvh#fight=10&type=damage-taken&source=2&start=1568847&end=1574993&view=events)). The damage transfered is reduced by 75%.

This aura is similar to [Devotion Aura](./DevotionAura.md), but reduces 10% more damage on other players at the cost of (part of) the transfered damage being transfered to you and deactivating when you drop below 75% health.

Because the damage transfer deactivates when you drop below 75% health, Aura of Sacrifice will be less reliable than [Devotion Aura](./DevotionAura.md). Reliability is important with raid cooldowns, so using [Devotion Aura](./DevotionAura.md) may be advised.

Activating Aura Mastery while already below 75% may lead to the entire cooldown being wasted.

### Speculation

The Paladin's total damage taken before damage reductions will be 100% of the damage he takes himself plus 75% of 30% of the damage taken by others. In a 20 player group the total damage taken will be `100% + ((100% - 75%) * 30% * 19) =` 243%.

The most common usage of raid-wide damage reductions such as Aura of Sacrifice and Devotion Aura is during periods of high raid damage. With the total damage taken in mind, it seems unlikely you will be able to stay above 75% health for the full duration of [Aura Mastery](../../AuraMastery.md). Because the DR gain from [Devotion Aura](./DevotionAura.md) is likely not going to be the difference in staying alive often, the unreliability is likely only worth it on very rare occasions. Your DR malfunctioning *will* be a big impact when you really need it.

With that in mind, it may be advisable to use [Divine Shield](../../DivineShield.md) with Aura of Sacrifice to ensure you don't drop below 75% health. The standard cooldown of Divine Shield is 5 minutes, but this can be reduced to 3.5 minutes with [Unbreakable Spirit](../30/UnbreakableSpirit.md). You still need to ensure you're above 75% health with Divine Shield active though.

**NOTE:** Spells like _Spirit Link Totem_ **can** still reduce your health below 75% during [Divine Shield](../../DivineShield.md).

## Changes since Legion

- Reworked, old:

![image](https://user-images.githubusercontent.com/4565223/39911211-e6c4e2f6-54fa-11e8-975a-3a9a5531dd7d.png)
