<!-- # Table of Contents -->

- [Adventure Map Spells Overview](#adventure-map-spells-overview)
- [High Magic Mod](#sor-rework)
- [Known Issues](#known-issues)
- [TODOs](#todos)
- [Changelog](#changelog)
- [Credits](#credits)

---

# Adventure Map Spells Overview

![Spells](https://raw.githubusercontent.com/vcmi-mods/adventure-spells-pack/refs/heads/vcmi-1.7/screenshots/screen05.png)

### **Air**
- **Accuracy**: All creatures receive +5/10/15% Damage when attacking at range until the end of the day.
- **Clarity**: All creatures receive mind spell immunity until the end of the day/day/week.
- **Darkness**: Creates a 1/2/3 tile radius of shroud for non-allied players with hero movement until the end of the day.
- **Divine Spirit**: All creatures receive +1/2/3 Morale until the end of the day.
- **Fleet Foot**: Gain +200/300/400 max movement points in next day.
- **Power of Haste**: All creatures receive +1/2/3 Speed until the end of the day.

### **Earth**
- **Dead Luck**: Reduces maximum Luck in combat to +2/+1/negates positive until the end of the day.
- **Death Call**: Increases Necromancy skill by 10/15/20% until the end of the day.
- **Dwarven Luck**: All creatures receive +1/2/3 Luck until the end of the day.
- **Herald of Death**: Reduces maximum Morale in combat to +2/+1/negates positive until the end of the day.
- **Hold Ground**: Creatures receive +3/6/9 Defense when defending in combat until the end of the day.
- **Power of Stone**: Creatures ignore 5/10/15% of enemy Attack until the end of the day.

### **Fire**
- **Demonic Power**: Creatures receive +5/10/15% Damage until the end of the day.
- **Raise Demons**: Necromancy raises Demons/Horned Demons/Horned Demons until the end of the day/day/week.
- **Shattering Strike**: Creatures' attacks ignore 5/10/15% of enemy Defense until the end of the day.

### **Water**
- **Benediction**: Cast all spells at Basic/Advanced/Expert proficiency until the end of the day.
- **Channel Power**: Gain +5/10/15% spell damage until the end of the day.
- **Seafaring**: Removes the boarding and unboarding penalties of ships until the end of the day/day/week.
- **Whirlpool Protection**: Protects the army from whirlpools until the end of the day/day/week.

### Global
- **Arcane Protection**: Creatures receive +5/10/15% spell damage reduction until the end of the day.
- **Empathy**: Nullifies the Morale penalty of mixing good and neutral units until the end of the day/day/week.
- **Griffin Eye**: See 1/2/3 square further into the shroud until the end of the day.
- **Magic Cushion**: Creatures receive +5/10/15% magical resistance until the end of the day.
- **Negotiations**: Reduces the cost of surrendering by -10/20/30% until the end of the day.

---

# High Magic Mod Overview

The mod changes durations, behavior, availability and costs of the spells. The changes listed below indicate spells that are mostly done.

## Changes to the original adventure spells

### Air
- **Accuracy**: casts mass 'Precision' spell at the begenning of a battle. Drains mana per battle -20/-10/-10/-10. Lasts until next week.
- **Clarity**: casts mass 'Mindshield' spell at the beginning of a battle. Drains mana per battle -20/-20/-10/-10. Lasts until next week.
- **Darkness**: A thick shroud of darkness envelops the area surrounding the hero (3/3/4/5 radius), obscuring it from the sight of foes.\r\n\r\nThe spell inflicts a -3/-2/-2/-2 penalty to Knowledge, decreases visibility radius by -3/-2/-2/-1, and reduces the hero’s movement by -1000/-700/-500/-300 points. The effects persist until the next week.
- **Divine Spirit**: Casts Mirth and Sorrow at the beginning of a battle. Drains mana per battle -20/-10/-10/-10. Nullifies the Morale penalty of mixing good and neutral units. Lasts until next week.
- **Fleet Foot**: Fixed original file. Adds +200/400/700/1000 to max movement points. Drains -2/-3/-4/-5 Attack, -2/-3/-4/-5 Defence, -500/-500/-750/-1000 gold and 1 gem daily. The effects persist until the next week.

### Earth
- **Dead Luck**: disabled due to a bugged mechanic.
- **Luck Leech**: replaces Dead Luck; casts Fortune and Misfortune at the beginning of a battle. Drains mana per battle -20/-10/-10/-10. Lasts until next week. 
- **Death Call**: boosts Necromancy skill +5/10/15/20%; drains knowledge -1/-2/-2/-2, Power -1/-1/-2/-2, Mercury 0/0/-1/-1, Sulfur 0/0/0/-1.
- **Dwarven Luck**: disabled due to no ideas about this one, and its features already used in Luck Leech spell.

### Water
- **Benediction**: A Hero can cast all spells at Basic/Basic/Advanced/Expert proficiency at a price of 'Power' -10/-2/-5/-8. Lasts until next week.
- **Channel Power**: A hero gains a solid boost to 'Power' 5/5/7/10, yet the spell drains from the all other primary skills -5/-3/-4/-5 each. The effect lasts until next week.

### Global
- **Arcane Protection**: casts mass 'Spellguard' spell at the beginning of a battle. Drains mana per battle -20/-10/-10/-10. Lasts until next week.
- **Griffin Eye**: disabled, as the Vision spell now has the same buff.
- **Empathy**: disabled, as the Divine Spirit now has the same buff.

## Modifications to the core spells
- **Visions**: Additionally grants +0/1/2/3 to the sight radius. The effect lasts until next week. Drains -1 Power, -1 Knowledge, and -100 movement.
- **Disguise**: The effect lasts until next week. Drains -1 Power, -1 Knowledge, and -100 movement.

## New battle spells
As a consequence of the rework, some new spells were designed to simulate Adventure Spells effects as battle spells. As default, they are set to be not available in mages' guild, but it can be changed with the 'Make it available' mod in the same directory. 

- **Spellguard**: used in **Arcane Protection**, adds 5/10/15/20 spell damage immunity, known from Golems, and 1/2/3/4 magic mirror. The effect is cumulative.

- **Mindshield** used in **Clarity**, gives Mind Immunity, dispels Mind spells, except Mirth, and sets min morale to -/-/0/0.

## NOTES

- Most the spells now work as opening battle spells, so their effects are visible and can also be negated or dispelled.
- Considered **Cancelation spell**, but ultimately no-cancelation showed up as an interesting consequence.
- Artifacts have the advantage over the adventure spells that they are mostly not burdened with consequences.
- Initially considered exactly 7 days duration for the spells, but as long as there is no comfortable option to see are spells currently in use, their duration lasts until new week. This means that entering a new week serves as a signal to renew the spells if necessary. The duration is determined by the timing of when the spells are cast.
---

# Known Issues

- Lack of proper indication in the unit window about true effects of a spell. This also applies if a spell has a cumulating effect. Currently only 'base' stats are displayed. As far as I know, the issue is known to developers and not easy to change.
- There is no way to indicate that adventure spells' duration ended. Partially solved with the durations set to: until next week. So a new week works as a reminder that spells must be renewed.
- A player can cast a spell which drains resources, even if there is nothing to drain. In most cases, values can't drop below zero. Partially solved with variety of costs.
- Resources value can drop below zero, but picking any other treasure resets it to 0 again. Kinda strange, but seems harmless.
- Have in mind that there is no AI support for the spells, which means AI doesn't use them.
- Spells casted at the begining of a battle has always a mass effect despite their level.
- Some spells ignores hero's power when it comes to duration. Partially solved by adjusting fixed durations.
- Casts per day bug: [#6659](https://github.com/vcmi/vcmi/issues/6659) (solved in upcomming 1.7.2 update).
- Original 'Dead Luck' effect doesn't work as intended for unknown reasons. Disabled as default.

---

## TODOs

1. Compatibility mod, as current design have support only for the vanilla factions.
2. Restrictions to the spells - eg. 'Call the Legion' prohibited to a Knights, 'Benediction' prohibited to a Death Knight. Also there should be restrictions to the creatures.
3. Original sounds for additional battle spells and animations, currently they reuse existing ones.

# Changelog

## Version 2.0

### SoR's rework

- [ ] Duration of the spells changed to ONE_WEEK, including Disguise and Visions 
- [ ] Changed behavior and effects of the spells, while staying close to their original bonuses.
- [ ] Variety of spells' costs implemented: mana costs, movement costs, primary skills costs, resources costs...
- [ ] The spells are quite rare to find and pinned to specific factions (max. gain chance = 3; default 0),
- [ ] New battle spells added to simulate some effects. Unavailable as default, but can be enabled.
- [ ] Things kept optional.

### Original files

- [ ] Changed 'Raise Demons' name to 'Call the Legion', assuming potential conflicts with other mods in the future.
- [ ] Reduced duplication by making use of "base" objects (which was not present).
- [ ] Erased comments.
- [ ] Fixed incorrect valueType in basic Fleet Foot.
- [ ] Dead Luck banned, due to bugged mechanic.

### Structure

- [x] Rearranged directory tree, any unnecessary directories deleted. Schools indications moved to Readme-s.
- [x] Further shortening of object chains from e.g. `spell.adventure-spells-pack.air.accuracy.accuracy.description.none` to `spell.ams.original.accuracy.accuracy.description.none`
- [x] New division for original spells, new spells, changes, and miscelaneous content. 
- [ ] Updated paths to content and translations.

### Other

- [ ] Some sound effects louder, some replaced, plus fixed metas,
- [ ] Updated mod.json descriptions
- [ ] Updated Launcher's descriptions and documentation on GitHub
- [ ] Erased comments
- [ ] Credits for new arts used in the mod.

### Tests

- [] New content.
- [] Original content.


### Translations

- [x] Some minor translations lost due to structural changes.
- [ ] Chineese, complete, autogenerated.
- [ ] Spanish, complete, autogenerated.
- [ ] Polish, complete.

---

## Version 1.5

### Modularization

- [x] Spells are now fully "pickable" in the Launcher.

### Casting sounds

- [x] Added 24 .ogg files.

### Documentation

- [x] Added a solid **README.md** to the GitHub repository.
- [x] Included html documentation for the mod in the VCMI Launcher (in English).

### Naming Conventions

- [x] Standardized all file and directory names to begin with lowercase letters. Names with multiple words are now using camelCase for improved clarity.

### Path Fixes

- [x] Configs
- [x] Spells
- [x] Icons
- [x] Translations

---

# Credits
