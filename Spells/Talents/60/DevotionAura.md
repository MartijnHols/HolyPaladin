# Devotion Aura

[![Tooltip](https://user-images.githubusercontent.com/4565223/43018363-bc61c862-8c59-11e8-80fc-77938dfe1740.png)](https://beta.wowdb.com/spells/183425-devotion-aura)

- Tier 60 talent
- Passive (Aura)
- Boosted by [Aura Mastery](../../AuraMastery.md)

## About the Aura Mastery effect

During [Aura Mastery](../../AuraMastery.md) this reduces the damage taken of all allies in range by 20%. This aura is similar to [Aura of Sacrifice](./AuraOfSacrifice.md), except that it is weaker but more consistent. Consider using Aura of Sacrifice if people are still struggling to stay alive during Aura Mastery or shortly after.

## About the passive effect

The passive effect is shared with allies within 10 yards, but diminishes based on the number of allies. The formula for the applicable damage reduction is `2.25% + (7.75% / n)` where `n` is players in range.

![Passive damage reduction per player](https://user-images.githubusercontent.com/4565223/43288709-fa306030-9128-11e8-887f-b642bdcf2e3e.png)

Because the passive effect diminishes slowly as more people get in the aura, its total power gets stronger the more people are affected by it.

![Passive damage reduction total sum of all players](https://user-images.githubusercontent.com/4565223/43288708-fa17a43c-9128-11e8-8721-0b7be2602d7d.png)

Research notes: https://docs.google.com/spreadsheets/d/1X7CmptWKHZ4z-TWdoue1AoJissyOI0GGpys42mrGYec/edit?usp=sharing

According to Sigma (Blizzard class designer), the passive `should be asymptotic to 3%`. About our findings he said `I think you're getting correct behavior up to 10, and inconsistent behavior above that, but it should just flatten out towards 3%`. It currently almost exactly hits the 3% floor at 10 players in range. This would make sense as a design choice as you super rarely are in range of more players. The jump at 27 players to 2.9% seems weird, it might be caused by a rounding error and there aren't a lot of logs with that many people stacked so that I can properly verify, but that would still be strange as we checked many several events in the logs that are available.

## Changes since Legion

- Old: Passive reduces damage of allies by 20%, split by the number of allies within 10 yards 
- New: Passive reduces damage of allies by 10%, diminishing (more slowly) by the number of allies within 10 yards
