# Devotion Aura

[![Tooltip](https://user-images.githubusercontent.com/4565223/43018363-bc61c862-8c59-11e8-80fc-77938dfe1740.png)](https://beta.wowdb.com/spells/183425-devotion-aura)

- Tier 60 talent
- Passive (Aura)
- Boosted by [Aura Mastery](../../AuraMastery.md)

## About the Aura Mastery effect

During [Aura Mastery](../../AuraMastery.md) this reduces the damage taken of all allies in range by 20%. This aura is similar to [Aura of Sacrifice](./AuraOfSacrifice.md), except that it is weaker but more consistent. Consider using Aura of Sacrifice if people are still struggling to stay alive during Aura Mastery or shortly after.

## About the passive effect

The passive effect is shared with allies within 10 yards, but diminishes based on the number of allies. The formula for the applicable damage reduction is `MAX(3%, 2.25% + (7.75% / n))` where `n` is players in range.

![Passive damage reduction per player](https://user-images.githubusercontent.com/4565223/43329795-b427ddf4-91c1-11e8-99a1-10de8c026cc8.png)

Because the passive effect diminishes slowly as more people get in the aura, its total power gets stronger the more people are affected by it.

![Passive damage reduction total sum of all players](https://user-images.githubusercontent.com/4565223/43329796-b44026b6-91c1-11e8-879e-22b1ee875c94.png)
Research notes: https://docs.google.com/spreadsheets/d/1X7CmptWKHZ4z-TWdoue1AoJissyOI0GGpys42mrGYec/edit?usp=sharing

According to Sigma (Blizzard class designer), the passive `should be asymptotic to 3%`.

## Aura comparison

For a detailed aura comparison, see this article by Dreamguard:
https://sacredshielding.wordpress.com/2018/07/23/reading-the-color-of-your-aura-in-battle-for-azeroth/

## Changes since Legion

- Old: Passive reduces damage of allies by 20%, split by the number of allies within 10 yards 
- New: Passive reduces damage of allies by 10%, diminishing (more slowly) by the number of allies within 10 yards
