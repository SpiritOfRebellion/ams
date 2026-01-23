# For Modders

In the 'sounds' folder, you have backgrounds used on spells with specific school.
In the 'graphics' there are source files in vector format Inkscape .svg and raster grapics in Gimp .xcf
The 'datasheets' folder contains charts made in LibreCalc's .ods files, where you can find spells' stats.

# Project guidelines

1. Mod is standarized for **camelCase naming convention** also to files and folders, to avoid typos and make easier to edit and generate mod files (with shell scripts for example).

2. Remember to update the main documentation files before you finish your work.

3. Whenever possible, leave source files e.g. raw graphics with layers in this directory for future modifications. 

## Pitfalls

1. **Icons** will replace each other if won't be placed in an additional folder, for example: 
- accuracy/content/sprites/**accuracy**/*.png 
- clarity/content/sprites/**clarity**/*.png

Paths to spirtes expample:

```
// herealdOfDeath.json example
...
"graphics": {
  "iconBook": "heraldOfDeath/spellBook",
  "iconScroll": "heraldOfDeath/spellScroll",
  "iconScenarioBonus": "heraldOfDeath/spellBonus",
  "iconEffect": "heraldOfDeath/spellEffect"
}
..
```
3. Object chains in translation files looks like this: `spell.adventure-spells-pack.air.divinespirit.divineSpirit.description.advanced` notice that **divinespirit** has no capital letter, while the second **divineSpirit** has.

---

## Data sets

Were helpful for AI prompts and documentation.

### Spells added
```
json_data='{"accuracy", "clarity", "darkness", "divineSpirit", "fleetFoot", "powerOfHaste"],
    "earth": ["deadLuck", "deathCall", "dwarvenLuck", "heraldOfDeath", "holdGround", "powerOfStone"],
    "fire": ["demonicPower", "raiseDemons", "shatteringStrike"],
    "water": ["benediction", "channelPower", "seafaring", "whirlpoolProtection"],
    "global": ["arcaneProtection", "empathy", "griffinEye", "magicCushion", "negotiations"]
}'
```

### Submods filesystem pattern

```
/{$element} 
/{$element}/mod.json 
/{$element}/mods/{$spell}
/{$element}/mods/{$spell}/mod.json
/{$element}/mods/{$spell}/content/sprites/*.png
/{$element}/mods/{$spell}/content/sounds/*.ogg
/{$element}/mods/{$spell}/content/config/spells/{$spell}.json
```
