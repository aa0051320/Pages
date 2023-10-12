---
title: "DPS Calculation"
slug: "DPS Calculation"
order: 
published: false
---

# {{ page.title }}

# Greater Chain Lightning Calculation

## Multiple enemies, each time damage
DamageN = Base Damage% * ( 1 + 5% ** ( N - 1 ) )
  1st: 50 * ( 1 + 5% * ( 1 - 1 ) ) = 50
  2nd: 50 * ( 1 + 5% * ( 2 - 1 ) ) = 52.5
  3rd: 50 * ( 1 + 5% * ( 3 - 1 ) ) = 55
  4th: 50 * ( 1 + 5% * ( 4 - 1 ) ) = 57.5
  5th: 50 * ( 1 + 5% * ( 5 - 1 ) ) = 60
  6th: 50 * ( 1 + 5% * ( 6 - 1 ) ) = 62.5
  7th: 50 * ( 1 + 5% * ( 7 - 1 ) ) = 65
  8th: 50 * ( 1 + 5% * ( 8 - 1 ) ) = 67.5
  9th: 50 * ( 1 + 5% * ( 9 - 1 ) ) = 70

## Multiple enemies, total damage
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

## Single enemy, each time damage (Odd times is hit, even times is not hit)
DamageN = Base Damage% * ( 1 + 10% ** ( N - 1 ) )
  1st: 50 * ( 1 + 10% * ( 1 - 1 ) ) = 50
  2nd: 50 * ( 1 + 10% * ( 2 - 1 ) ) = 55
  3rd: 50 * ( 1 + 10% * ( 3 - 1 ) ) = 60
  4th: 50 * ( 1 + 10% * ( 4 - 1 ) ) = 65
  5th: 50 * ( 1 + 10% * ( 5 - 1 ) ) = 70

## Single enemy, total damage (Odd times is hit, even times is not hit)
SumN = Base Damage% * ( N + 10% * N * ( N - 1 ) / 2)
  1st: 50 * ( 1 + 10% * 1 * ( 1 - 1 ) / 2 ) = 50
  2nd: 50 * ( 2 + 10% * 2 * ( 2 - 1 ) / 2 ) = 105
  3rd: 50 * ( 3 + 10% * 3 * ( 3 - 1 ) / 2 ) = 165
  4th: 50 * ( 4 + 10% * 4 * ( 4 - 1 ) / 2 ) = 230
  5th: 50 * ( 5 + 10% * 5 * ( 5 - 1 ) / 2 ) = 300

# Ice Shards
Ice Shards 5
  ( 35 + 25 ) * 5 = 300
Ice Shards 9
  ( 45 + 25 ) * 5 = 350
Ice Shards 5 + Storm Swell 2
  ( 35 + 25 ) * 5 * ( 1 + 0.3 * 2 ) = 480
Ice Shards 5 + Control 2
  ( 35 + 25 ) * 5 * ( 1 + 0.35 * 2 ) = 510

# Chain Lightning
Chain Lightning 5
  50 * 5 = 250
Chain Lightning 9
  65 * 5 = 325
Chain Lightning 5 + Unbroken Tether
  50 * 5 * ( 1 + 0.4 * 4 ) = 650
Chain Lightning 5 + Unbroken Tether 2
  50 * 5 * ( 1 + 0.4 * 2 * 4 ) = 1050
Chain Lightning 9 + Unbroken Tether
  65 * 5 * ( 1 + 0.4 * 4 ) = 845
Chain Lightning 9 + Unbroken Tether 2
  65 * 5 * ( 1 + 0.4 * 2 * 4 ) = 1365

# Ice Shards + Chain Lightning Enchantment
Ice Shards 5 + Chain Lightning Enchantment 5
  300 + ( 30 / 100 ) * 250 = 375
Ice Shards 5 + Chain Lightning Enchantment 5 + Unbroken Tether
  300 + ( 30 / 100 ) * 650 = 495
Ice Shards 5 + Chain Lightning Enchantment 5 + Unbroken Tether 2
  300 + ( 30 / 100 ) * 1050 = 615

# Gloves
Frostburn 5
  26.2
Ice Shards 4 + Attack Speed
  ( 45 - 35 ) * ( 1 + 0.15 ) = 11.5
Ice Shards 4 + Forst Orb 4 + Frozen Orbit
  ( 45 - 35 ) + 0.3 * ( ( 65 - 50 ) + ( 61 - 48 ) * ( 1 + 2 * 0.4 ) ) = 21.52
Ice Shards 4 + Chain Lightning 4 + Unbroken Tether
  ( 45 - 35 ) + ( 30 / 100 ) * ( ( 65 - 50 ) * ( 5 + 0.4 * 4 ) ) = 39.7
Ice Shards 9 + Chain Lightning Enchantment 9 + Unbroken Tether 2
  350 + ( 30 / 100 ) * 1365 = 759.5

# Weapon
Wand + Focus
  (21.0 + 26.2 + 35.3 + 29.2) * 1.2 * 1.3 * 1.35 = 235.2402
Staff
  (42.0 + 52.5 + 70.5 + 58.5) * 1 * 1.6 = 357.6
    357.6 - 235.2402 = 122.3598
