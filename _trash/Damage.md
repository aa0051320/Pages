---
title: "Damage"
slug: "Damage"
order: 
published: false
---

# {{ page.title }}

|                             Game                             | Patch |     Realm     |  Class   |
| :----------------------------------------------------------: | :---: | :-----------: | :------: |
| [Diablo IV](https://diablo4.blizzard.com/){:target="_blank"} | 1.2.0 | Eternal Realm | Sorcerer |

# Priority
1. Lucky Hit Chance > Resource Generation > Maximum Mana
2. Critical Strike Chance > Movement Speed
3. Attack Speed
4. Intelligence > All Stats
5. Additive Damage
6. Skill / Effect

# Skill

## Greater Chain Lightning 5

### Multiple enemies
DamageN = Base Damage% * ( 1 + 5% * ( N - 1 ) )
  1st: 50 * ( 1 + 5% * ( 1 - 1 ) ) = 50
  2nd: 50 * ( 1 + 5% * ( 2 - 1 ) ) = 52.5
  3rd: 50 * ( 1 + 5% * ( 3 - 1 ) ) = 55
  4th: 50 * ( 1 + 5% * ( 4 - 1 ) ) = 57.5
  5th: 50 * ( 1 + 5% * ( 5 - 1 ) ) = 60
  6th: 50 * ( 1 + 5% * ( 6 - 1 ) ) = 62.5
  7th: 50 * ( 1 + 5% * ( 7 - 1 ) ) = 65
  8th: 50 * ( 1 + 5% * ( 8 - 1 ) ) = 67.5
  9th: 50 * ( 1 + 5% * ( 9 - 1 ) ) = 70
  10th: 50 * ( 1 + 5% * ( 10 - 1 ) ) = 72.5

SumN = Base Damage% * ( N + 5% * N * ( N - 1 ) / 2)
  1st: 50 * ( 1 + 5% * 1 * ( 1 - 1 ) / 2 ) = 50
  2nd: 50 * ( 2 + 5% * 2 * ( 2 - 1 ) / 2 ) = 102.5
  3rd: 50 * ( 3 + 5% * 3 * ( 3 - 1 ) / 2 ) = 157.5
  4th: 50 * ( 4 + 5% * 4 * ( 4 - 1 ) / 2 ) = 215
  5th: 50 * ( 5 + 5% * 5 * ( 5 - 1 ) / 2 ) = 275
  6th: 50 * ( 6 + 5% * 6 * ( 6 - 1 ) / 2 ) = 337.5
  7th: 50 * ( 7 + 5% * 7 * ( 7 - 1 ) / 2 ) = 402.5
  8th: 50 * ( 8 + 5% * 8 * ( 8 - 1 ) / 2 ) = 470
  9th: 50 * ( 9 + 5% * 9 * ( 9 - 1 ) / 2 ) = 540
  10th: 50 * ( 10 + 5% * 10 * ( 10 - 1 ) / 2 ) = 612.5
  7th~10th: 65 + 67.5 + 70 + 72.5 = 275 * 0.4 = 110

### Single enemy (Odd times is hit, even times is not hit)
DamageN = Base Damage% * ( 1 + 10% * ( N - 1 ) )
  1st: 50 * ( 1 + 10% * ( 1 - 1 ) ) = 50
  2nd: 50 * ( 1 + 10% * ( 2 - 1 ) ) = 55
  3rd: 50 * ( 1 + 10% * ( 3 - 1 ) ) = 60
  4th: 50 * ( 1 + 10% * ( 4 - 1 ) ) = 65
  5th: 50 * ( 1 + 10% * ( 5 - 1 ) ) = 70

SumN = Base Damage% * ( N + 10% * N * ( N - 1 ) / 2)
  1st: 50 * ( 1 + 10% * 1 * ( 1 - 1 ) / 2 ) = 50
  2nd: 50 * ( 2 + 10% * 2 * ( 2 - 1 ) / 2 ) = 105
  3rd: 50 * ( 3 + 10% * 3 * ( 3 - 1 ) / 2 ) = 165
  4th: 50 * ( 4 + 10% * 4 * ( 4 - 1 ) / 2 ) = 230
  5th: 50 * ( 5 + 10% * 5 * ( 5 - 1 ) / 2 ) = 300

## Greater Chain Lightning 9

### Multiple enemies
DamageN = Base Damage% * ( 1 + 5% * ( N - 1 ) )
  1st: 65 * ( 1 + 5% * ( 1 - 1 ) ) = 65
  2nd: 65 * ( 1 + 5% * ( 2 - 1 ) ) = 68.25
  3rd: 65 * ( 1 + 5% * ( 3 - 1 ) ) = 71.5
  4th: 65 * ( 1 + 5% * ( 4 - 1 ) ) = 74.75
  5th: 65 * ( 1 + 5% * ( 5 - 1 ) ) = 78
  6th: 65 * ( 1 + 5% * ( 6 - 1 ) ) = 81.25
  7th: 65 * ( 1 + 5% * ( 7 - 1 ) ) = 84.5
  8th: 65 * ( 1 + 5% * ( 8 - 1 ) ) = 87.75
  9th: 65 * ( 1 + 5% * ( 9 - 1 ) ) = 91
  10th: 65 * ( 1 + 5% * ( 10 - 1 ) ) = 94.25

SumN = Base Damage% * ( N + 5% * N * ( N - 1 ) / 2)
  1st: 65 * ( 1 + 5% * 1 * ( 1 - 1 ) / 2 ) = 65
  2nd: 65 * ( 2 + 5% * 2 * ( 2 - 1 ) / 2 ) = 133.25
  3rd: 65 * ( 3 + 5% * 3 * ( 3 - 1 ) / 2 ) = 204.75
  4th: 65 * ( 4 + 5% * 4 * ( 4 - 1 ) / 2 ) = 279.5
  5th: 65 * ( 5 + 5% * 5 * ( 5 - 1 ) / 2 ) = 357.5
  6th: 65 * ( 6 + 5% * 6 * ( 6 - 1 ) / 2 ) = 438.75
  7th: 65 * ( 7 + 5% * 7 * ( 7 - 1 ) / 2 ) = 523.25
  8th: 65 * ( 8 + 5% * 8 * ( 8 - 1 ) / 2 ) = 611
  9th: 65 * ( 9 + 5% * 9 * ( 9 - 1 ) / 2 ) = 702
  6th~10th: 81.25 + 84.5 + 87.75 + 91 + 94.25 = 438.75 * 0.4 = 175.5

### Single enemy (Odd times is hit, even times is not hit)
DamageN = Base Damage% * ( 1 + 10% * ( N - 1 ) )
  1st: 65 * ( 1 + 10% * ( 1 - 1 ) ) = 65
  2nd: 65 * ( 1 + 10% * ( 2 - 1 ) ) = 71.5
  3rd: 65 * ( 1 + 10% * ( 3 - 1 ) ) = 78
  4th: 65 * ( 1 + 10% * ( 4 - 1 ) ) = 84.5
  5th: 65 * ( 1 + 10% * ( 5 - 1 ) ) = 91

SumN = Base Damage% * ( N + 10% * N * ( N - 1 ) / 2)
  1st: 65 * ( 1 + 10% * 1 * ( 1 - 1 ) / 2 ) = 65
  2nd: 65 * ( 2 + 10% * 2 * ( 2 - 1 ) / 2 ) = 136.5
  3rd: 65 * ( 3 + 10% * 3 * ( 3 - 1 ) / 2 ) = 214.5
  4th: 65 * ( 4 + 10% * 4 * ( 4 - 1 ) / 2 ) = 299
  5th: 65 * ( 5 + 10% * 5 * ( 5 - 1 ) / 2 ) = 390

## Ice Shards
Ice Shards 5
  ( 35 + 25 ) * 5 = 300
Ice Shards 5 * Avalanche
  ( 35 + 25 ) * 5 * ( 1 + 0.4 ) = 420
Ice Shards 9
  ( 45 + 25 ) * 5 = 350
Ice Shards 9 * Avalanche
  ( 45 + 25 ) * 5 * ( 1 + 0.4 ) = 490

Ice Shards 5 + Storm Swell Aspect
  ( 35 + 25 ) * 5 * ( 1 + 0.3 ) = 390
Ice Shards 9 + Storm Swell Aspect
  ( 45 + 25 ) * 5 * ( 1 + 0.3 ) = 455

# Frozen Orb
Frozen Orb 5
  50 + 48 = 98
Frozen Orb 9
  65 + 61 = 126
Frozen Orb 5 + Frozen Orbit
  50 + 48 * ( 1 + 2 * 0.4 ) = 136.4

# Chain Lightning
Chain Lightning 5
  50 * 5 = 250
Chain Lightning 9
  65 * 5 = 325
Chain Lightning 5 + Aspect of the Unbroken Tether
  50 * ( 5 + 0.4 * 4 ) = 330
Chain Lightning 9 + Aspect of the Unbroken Tether
  65 * ( 5 + 0.4 * 4 ) = 429

## Greater Chain Lightning
Chain Lightning 5
  275
Chain Lightning 5 + Aspect of the Unbroken Tether
  275 + 0.4 * 325 = 405

# Comparison

## Ice Shards
Ice Shards 5 * Aspect of Frozen Memories * Storm Swell Aspect
  ( 35 + 25 ) * 5 * ( 1 + 0.2 * ( 1 + 0.4 ) * 2 ) * ( 1 + 0.3 ) = 608.4

Ice Shards 5 * Aspect of Frozen Memories * ( Storm Swell Aspect + Conceited Aspect )
  ( 35 + 25 ) * 5 * ( 1 + 0.2 * ( 1 + 0.4 ) * 2 ) * ( 1 + 0.3 + 0.25 ) = 725.4

## Frozen Orb Enchantment
Ice Shards 5 + Frozen Orb Enchantment 5 + Frozen Orbit
  ( 35 + 25 ) * 5 + 0.3 * ( 50 + 48 * ( 1 + 2 * 0.4 ) ) = 340.92

( Ice Shards 5 + Frozen Orb Enchantment 5 + Frozen Orbit ) * Aspect of Frozen Memories
  ( ( 35 + 25 ) * 5 + 0.3 * ( 50 + 48 * ( 1 + 2 * 0.4 ) ) ) * ( 1 + 0.2 * ( 1 + 0.4 ) * 2 ) = 531.8352

( Ice Shards 5 + Frozen Orb Enchantment 5 + Frozen Orbit ) * Aspect of Frozen Memories * Storm Swell Aspect
  ( ( 35 + 25 ) * 5 + 0.3 * ( 50 + 48 * ( 1 + 2 * 0.4 ) ) ) * ( 1 + 0.2 * ( 1 + 0.4 ) * 2 ) * ( 1 + 0.3 ) = 691.38576

( Ice Shards 5 + Frozen Orb Enchantment 5 ) * Aspect of Frozen Memories * Storm Swell Aspect
  ( ( 35 + 25 ) * 5 + 0.3 * ( 50 + 48 ) ) * ( 1 + 0.2 * ( 1 + 0.4 ) * 2 ) * ( 1 + 0.3 ) = 668.0232

## Chain Lightning Enchantment
Ice Shards 5 + Chain Lightning Enchantment 5 Greater + Aspect of the Unbroken Tether
  ( ( 35 + 25 ) * 5 + ( 30 / 100 ) * 405 ) = 421.5

( Ice Shards 5 + Chain Lightning Enchantment 5 Greater + Aspect of the Unbroken Tether ) * Shattered Aspect
  ( ( 35 + 25 ) * 5 + ( 30 / 100 ) * 405 ) * ( 1 + 0.25 ) = 526.875
  ( ( 35 + 25 ) * 5 + ( 30 / 100 ) * 405 ) * ( 1 + 0.25 + 0.4) = 695.475

( Ice Shards 5 + Chain Lightning Enchantment 5 Greater + Aspect of the Unbroken Tether ) * Shattered Aspect * Storm Swell Aspect
  ( ( 35 + 25 ) * 5 + ( 30 / 100 ) * 405 ) * ( 1 + 0.25 ) * ( 1 + 0.3 ) = 684.9375
  ( ( 35 + 25 ) * 5 + ( 30 / 100 ) * 405 ) * ( 1 + 0.25 + 0.4) * ( 1 + 0.3 ) = 904.1175

( Ice Shards 5 + Chain Lightning Enchantment 5 Greater ) * Shattered Aspect * Storm Swell Aspect
  ( ( 35 + 25 ) * 5 + ( 30 / 100 ) * 275 ) * ( 1 + 0.25 ) * ( 1 + 0.3 ) = 621.  5625
  ( ( 35 + 25 ) * 5 + ( 30 / 100 ) * 275 ) * ( 1 + 0.25 + 0.4) * ( 1 + 0.3 ) = 820.4625
