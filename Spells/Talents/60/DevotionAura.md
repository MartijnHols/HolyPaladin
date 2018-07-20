# Devotion Aura

[![Tooltip](https://user-images.githubusercontent.com/4565223/43018363-bc61c862-8c59-11e8-80fc-77938dfe1740.png)](https://beta.wowdb.com/spells/183425-devotion-aura)

- Tier 60 talent
- Passive (Aura)
- Boosted by [Aura Mastery](../../AuraMastery.md)

## About the Aura Mastery effect

During [Aura Mastery](../../AuraMastery.md) this reduces the damage taken of all allies in range by 20%. This aura is similar to [Aura of Sacrifice](./AuraOfSacrifice.md), except that it is weaker but more consistent. Consider using Aura of Sacrifice if people are still struggling to stay alive during Aura Mastery or shortly after.

## About the passive effect

The passive effect is shared with allies within 10 yards, but diminishes based on the number of allies. The formula for the applicable damage reduction is `2.25% + (7.75% / n)` where `n` is players in range.

![image](https://user-images.githubusercontent.com/4565223/43018656-98f1ef32-8c5a-11e8-9a53-89cdf8869f79.png)

Research notes: https://docs.google.com/spreadsheets/d/1X7CmptWKHZ4z-TWdoue1AoJissyOI0GGpys42mrGYec/edit?usp=sharing

## Changes since Legion

- Old: Passive reduces damage of allies by 20%, split by the number of allies within 10 yards 
- New: Passive reduces damage of allies by 10%, diminishing (more slowly) by the number of allies within 10 yards
