---
title: "Paragon Calculation"
slug: "Paragon Calculation"
order: 
published: true
---

# {{ page.title }}

|                             Game                             | Patch |     Realm     |  Class   |
| :----------------------------------------------------------: | :---: | :-----------: | :------: |
| [Diablo IV](https://diablo4.blizzard.com/){:target="_blank"} | 1.2.1 | Eternal Realm | Sorcerer |

1. Starting Board
   - Strength 10
   - Dexterity 39
     - Exploit 8 * ( 39 / 5 ) = 62.4
     - Exploit 8 * ( 39 / 5 ) + 10 = 72.4
   - Intelligence 70
   - Willpower 39
2. Frigid Fate
   - Strength 15
   - Dexterity 29
   - Intelligence 70
     - Enchanter 6.5 * ( 70 / 5 ) = 91
   - Willpower 44
3. Burning Instinct
   - Strength 5
   - Dexterity 49
     - Destruction 20 * ( 49 / 5 ) = 196
     - Destruction 20 * ( 49 / 5 ) + 12 = 208
   - Intelligence 70
   - Willpower 34
4. Icefall
   - Strength 15
   - Dexterity 34
   - Intelligence 55
   - Willpower 54
     - Frostbite 14.9 * ( 54 / 5 ) = 160.92
5. Enchantment Master
   - Strength 5
   - Dexterity 39
     - Control 14.9 * ( 39 / 5 ) + 10 = 126.22
     - Control 14.9 * ( 39 / 5 ) + 20 = 136.22
   - Intelligence 65
   - Willpower 49
6. Elemental Summoner
   - Strength 10
   - Dexterity 34
   - Intelligence 60
   - Willpower 54
     - Imbiber 9.8 * ( 54 / 5 ) = 105.84

## Result

|   #   |       Board        |    Glyph    | Base% |   Multiple    |  Bonus  |     Result%     |
| :---: | :----------------: | :---------: | :---: | :-----------: | :-----: | :-------------: |
|   1   |      Starting      |   Exploit   |   8   | 39 / 5 = 7.8  |   10    |   62.4 ~ 72.4   |
|   2   |    Frigid Fate     |  Enchanter  |  6.5  |  70 / 5 = 14  |         |       91        |
|   3   |  Burning Instinct  | Destruction |  20   | 49 / 5 = 9.8  | 0 ~ 12  |    196 ~ 208    |
|   4   |      Icefall       |  Frostbite  | 14.9  | 54 / 5 = 10.8 |         |     160.92      |
|   5   | Enchantment Master |   Control   | 14.9  | 39 / 5 = 7.8  | 10 ~ 20 | 126.22 ~ 136.22 |
|   6   | Elemental Summoner |   Imbiber   |  9.8  | 54 / 5 = 10.8 |         |     105.84      |

- Min: 62.4 + 91 + 196 + 160.92 + 126.22 + 105.84 = 742.38
- Max: 72.4 + 91 + 208 + 160.92 + 136.22 + 105.84 = 774.38
