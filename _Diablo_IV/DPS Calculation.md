---
title: "DPS Calculation"
slug: "DPS Calculation"
order: 
published: false
---

# {{ page.title }}

|                             Game                             | Patch |     Realm     |  Class   |
| :----------------------------------------------------------: | :---: | :-----------: | :------: |
| [Diablo IV](https://diablo4.blizzard.com/){:target="_blank"} | 1.1.4 | Eternal Realm | Sorcerer |

# Greater Chain Lightning Calculation

## Multiple enemies, each time damage
DamageN = Base Damage% * ( 1 + 5% * ( N - 1 ) )
- 1st: 50 * ( 1 + 5% * ( 1 - 1 ) ) = 50
- 2nd: 50 * ( 1 + 5% * ( 2 - 1 ) ) = 52.5
- 3rd: 50 * ( 1 + 5% * ( 3 - 1 ) ) = 55
- 4th: 50 * ( 1 + 5% * ( 4 - 1 ) ) = 57.5
- 5th: 50 * ( 1 + 5% * ( 5 - 1 ) ) = 60
- 6th: 50 * ( 1 + 5% * ( 6 - 1 ) ) = 62.5
- 7th: 50 * ( 1 + 5% * ( 7 - 1 ) ) = 65
- 8th: 50 * ( 1 + 5% * ( 8 - 1 ) ) = 67.5
- 9th: 50 * ( 1 + 5% * ( 9 - 1 ) ) = 70

## Multiple enemies, total damage
SumN = Base Damage% * ( N + 5% * N * ( N - 1 ) / 2)
- 1st: 50 * ( 1 + 5% * 1 * ( 1 - 1 ) / 2 ) = 50
- 2nd: 50 * ( 2 + 5% * 2 * ( 2 - 1 ) / 2 ) = 102.5
- 3rd: 50 * ( 3 + 5% * 3 * ( 3 - 1 ) / 2 ) = 157.5
- 4th: 50 * ( 4 + 5% * 4 * ( 4 - 1 ) / 2 ) = 215
- 5th: 50 * ( 5 + 5% * 5 * ( 5 - 1 ) / 2 ) = 275
- 6th: 50 * ( 6 + 5% * 6 * ( 6 - 1 ) / 2 ) = 337.5
- 7th: 50 * ( 7 + 5% * 7 * ( 7 - 1 ) / 2 ) = 402.5
- 8th: 50 * ( 8 + 5% * 8 * ( 8 - 1 ) / 2 ) = 470
- 9th: 50 * ( 9 + 5% * 9 * ( 9 - 1 ) / 2 ) = 540
- 5th~9th: 60 + 62.5 + 65 + 67.5 + 70 = 325

## Single enemy, each time damage (Odd times is hit, even times is not hit)
DamageN = Base Damage% * ( 1 + 10% * ( N - 1 ) )
- 1st: 50 * ( 1 + 10% * ( 1 - 1 ) ) = 50
- 2nd: 50 * ( 1 + 10% * ( 2 - 1 ) ) = 55
- 3rd: 50 * ( 1 + 10% * ( 3 - 1 ) ) = 60
- 4th: 50 * ( 1 + 10% * ( 4 - 1 ) ) = 65
- 5th: 50 * ( 1 + 10% * ( 5 - 1 ) ) = 70

## Single enemy, total damage (Odd times is hit, even times is not hit)
SumN = Base Damage% * ( N + 10% * N * ( N - 1 ) / 2)
- 1st: 50 * ( 1 + 10% * 1 * ( 1 - 1 ) / 2 ) = 50
- 2nd: 50 * ( 2 + 10% * 2 * ( 2 - 1 ) / 2 ) = 105
- 3rd: 50 * ( 3 + 10% * 3 * ( 3 - 1 ) / 2 ) = 165
- 4th: 50 * ( 4 + 10% * 4 * ( 4 - 1 ) / 2 ) = 230
- 5th: 50 * ( 5 + 10% * 5 * ( 5 - 1 ) / 2 ) = 300

# Ice Shards
- Ice Shards 5
  - ( 35 + 25 ) * 5 = 300
- Ice Shards 9
  - ( 45 + 25 ) * 5 = 350
- Ice Shards 5 + Storm Swell Aspect
  - ( 35 + 25 ) * 5 * ( 1 + 0.3 ) = 390
- Ice Shards 9 + Storm Swell Aspect
  - ( 45 + 25 ) * 5 * ( 1 + 0.3 ) = 455

# Frozen Orb
- Frozen Orb 5
  - 50 + 48 = 98
- Frozen Orb 9
  - 65 + 61 = 126
- Frozen Orb 5 + Frozen Orbit
  - 50 + 48 * ( 1 + 2 * 0.4 ) = 136.4

# Chain Lightning
- Chain Lightning 5
  - 50 * 5 = 250
- Chain Lightning 9
  - 65 * 5 = 325
- Chain Lightning 5 + Aspect of the Unbroken Tether
  - 50 * ( 5 + 0.4 * 4 ) = 330
- Chain Lightning 9 + Aspect of the Unbroken Tether
  - 65 * ( 5 + 0.4 * 4 ) = 429

## Greater Chain Lightning
- Chain Lightning 5
  - 275
- Chain Lightning 5 + Aspect of the Unbroken Tether
  - 275 + 0.4 * 325 = 405

# Comparison

## Ice Shards
- Ice Shards 5 * Aspect of Frozen Memories * Storm Swell Aspect
  - ( 35 + 25 ) * 5 * ( 1 + 0.2 * ( 1 + 0.4 ) * 2 ) * ( 1 + 0.3 ) = 608.4

- Ice Shards 5 * Aspect of Frozen Memories * ( Storm Swell Aspect + Conceited Aspect )
  - ( 35 + 25 ) * 5 * ( 1 + 0.2 * ( 1 + 0.4 ) * 2 ) * ( 1 + 0.3 + 0.25 ) = 725.4

## Frozen Orb Enchantment
- Ice Shards 5 + Frozen Orb Enchantment 5 + Frozen Orbit
  - ( 35 + 25 ) * 5 + 0.3 * ( 50 + 48 * ( 1 + 2 * 0.4 ) ) = 340.92

- ( Ice Shards 5 + Frozen Orb Enchantment 5 + Frozen Orbit ) * Aspect of Frozen Memories
  - ( ( 35 + 25 ) * 5 + 0.3 * ( 50 + 48 * ( 1 + 2 * 0.4 ) ) ) * ( 1 + 0.2 * ( 1 + 0.4 ) * 2 ) = 531.8352

- ( Ice Shards 5 + Frozen Orb Enchantment 5 + Frozen Orbit ) * Aspect of Frozen Memories * Storm Swell Aspect
  - ( ( 35 + 25 ) * 5 + 0.3 * ( 50 + 48 * ( 1 + 2 * 0.4 ) ) ) * ( 1 + 0.2 * ( 1 + 0.4 ) * 2 ) * ( 1 + 0.3 ) = 691.38576

- ( Ice Shards 5 + Frozen Orb Enchantment 5 ) * Aspect of Frozen Memories * Storm Swell Aspect
  - ( ( 35 + 25 ) * 5 + 0.3 * ( 50 + 48 ) ) * ( 1 + 0.2 * ( 1 + 0.4 ) * 2 ) * ( 1 + 0.3 ) = 668.0232

## Chain Lightning Enchantment
- Ice Shards 5 + Chain Lightning Enchantment 5 Greater + Aspect of the Unbroken Tether
  - ( ( 35 + 25 ) * 5 + ( 30 / 100 ) * 405 ) = 421.5

- ( Ice Shards 5 + Chain Lightning Enchantment 5 Greater + Aspect of the Unbroken Tether ) * Shattered Aspect
  - ( ( 35 + 25 ) * 5 + ( 30 / 100 ) * 405 ) * ( 1 + 0.25 ) = 526.875
  - ( ( 35 + 25 ) * 5 + ( 30 / 100 ) * 405 ) * ( 1 + 0.25 + 0.4) = 695.475

- ( Ice Shards 5 + Chain Lightning Enchantment 5 Greater + Aspect of the Unbroken Tether ) * Shattered Aspect * Storm Swell Aspect
  - ( ( 35 + 25 ) * 5 + ( 30 / 100 ) * 405 ) * ( 1 + 0.25 ) * ( 1 + 0.3 ) = 684.9375
  - ( ( 35 + 25 ) * 5 + ( 30 / 100 ) * 405 ) * ( 1 + 0.25 + 0.4) * ( 1 + 0.3 ) = 904.1175

- ( Ice Shards 5 + Chain Lightning Enchantment 5 Greater ) * Shattered Aspect * Storm Swell Aspect
  - ( ( 35 + 25 ) * 5 + ( 30 / 100 ) * 275 ) * ( 1 + 0.25 ) * ( 1 + 0.3 ) = 621.  5625
  - ( ( 35 + 25 ) * 5 + ( 30 / 100 ) * 275 ) * ( 1 + 0.25 + 0.4) * ( 1 + 0.3 ) = 820.4625
