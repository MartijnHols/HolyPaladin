# Awakening

[![Tooltip](https://user-images.githubusercontent.com/4565223/39920151-5e5bea6a-5516-11e8-8571-1f1a99ad47de.png)](https://beta.wowdb.com/spells/248033-awakening)

- Tier 90 talent
- Passive

## About

[Light of Dawn](../../LightOfDawn.md) has a small chance to proc [Avenging Wrath](../../AvengingWrath.md) for a short duration. The [Light of Dawn](../../LightOfDawn.md) that triggers [Avenging Wrath](../../AvengingWrath.md) does not gain any of the effects of Avenging Wrath, but since it does incur a GCD you should consider 1 GCD of the uptime wasted by default.

If [Avenging Wrath](../../AvengingWrath.md) is active while Awakening procs, it will extend the duration of the active buff. You can't cast [Avenging Wrath](../../AvengingWrath.md) while already afflicted by an Awakening proc.

## Uptime

With an average of 5 [Light of Dawn](../../LightOfDawn.md) casts per minute, on average Awakening will proc once every 1 minute and 20 seconds.

While each proc lasts 10 seconds (12.5% uptime), the first GCD will go to the LoD that triggered it. If we assume 15% Haste the GCD will be about 1.3seconds (`1.5s / (100% + 15%)`). This means the first 1.3 seconds of the buff is wasted, leaving 8.7 seconds effectively.

In those 8.7 seconds, we can cast `8.7s / 1.3s =` 6.69 GCDs. But there's no such thing as a partial globals so we can actually only cast 6 GCDs during the buff. This leaves `6gcd * 1.3sec =` 7.8 sec of effective uptime, or `7.8s / 80s =` 9.75%.

To play with the numbers you can use [this spreadsheet](https://docs.google.com/spreadsheets/d/1h2Zx2LxgnvF20AsPmPtj8Ikz6nd7K8evYsBstppeckw/edit?usp=sharing).

The gain will be slightly better when using talents such as [Judgment of Light](../75/JudgmentOfLight.md), [Bestow Faith](../15/BestowFaith.md), [Light's Hammer](../15/LightsHammer.md) and [Aura of Mercy](../60/AuraOfMercy.md) because their healing can also occur while waiting on the initial/final GCD.
