# Quest Structure Summary

## Overview
Total Quest Files: 6
- 1 Main configuration file (quests.snbt)
- 5 Chapter files (one per questline)

## Quest Statistics

### Main Configuration
- **File:** `config/ftbquests/quests.snbt`
- **Contains:** Welcome quest and main configuration
- **Lines:** 50

### Adventure Questline
- **File:** `config/ftbquests/quests/chapters/adventure.snbt`
- **Theme:** Exploration, biomes, dimensions
- **Color:** Blue (&b)
- **Total Quests:** 12
- **Lines:** 329
- **Quest IDs:** 1000000000000001 - 1000000000000035

**Quest Progression:**
1. Plains Explorer → Forest Explorer → Ocean Explorer → Desert Wanderer → Taiga Explorer
2. Mountain Climber (depends on Plains)
3. Jungle Adventurer (depends on Forest)
4. River Tracker (depends on Ocean)
5. Biome Master (capstone quest requiring 5 biome quests)
6. Into the Nether (depends on Biome Master)
7. Journey to the End (depends on Biome Master)

### Catching Questline
- **File:** `config/ftbquests/quests/chapters/catching.snbt`
- **Theme:** Catching Pokémon, types, evolutions
- **Color:** Orange (&6)
- **Total Quests:** 18
- **Lines:** 669
- **Quest IDs:** 2000000000000001 - 2000000000000052

**Quest Progression:**
1. First Catch → Growing Collection (10) → Expanding Horizons (25) → Master Collector (50)
2. Type-specific catches: Water, Fire, Grass, Electric, Psychic, Dragon, Ghost, Dark
3. Starter Type Master (requires Fire, Water, Grass)
4. Evolution chains: First Evolution → Evolution Expert
5. Shiny Hunter (rare challenge)

### Battling Questline
- **File:** `config/ftbquests/quests/chapters/battling.snbt`
- **Theme:** Battles, defeating Pokémon, trainers
- **Color:** Red (&4)
- **Total Quests:** 16
- **Lines:** 630
- **Quest IDs:** 3000000000000001 - 3000000000000049

**Quest Progression:**
1. First Battle → Battle Training (10) → Experienced Battler (25) → Battle Master (50)
2. PvP: Rival Battle → Competitive Battler
3. NPC: NPC Challenger → NPC Conqueror
4. Type-specific: Fire, Water, Grass, Dragon
5. Level-based: Tough Opponent (lvl 30+) → Elite Challenger (lvl 50+)

### Progression Questline
- **File:** `config/ftbquests/quests/chapters/progression.snbt`
- **Theme:** Crafting, items, training
- **Color:** Green (&2)
- **Total Quests:** 17
- **Lines:** 622
- **Quest IDs:** 4000000000000001 - 4000000000000069

**Quest Progression:**
1. Poké Ball chain: First Poké Ball → Better Balls → Ultimate Balls
2. Healing chain: Healing Basics → Better Healing → Advanced Healing → Master Healer
3. Revival chain: Second Chance → Full Restoration
4. Essential items: Storage System (PC) → Pokémon Center (Healing Machine)
5. Resources: Gathering Herbs, Apricorn Collector → Rainbow Collection
6. Training: Training Progress (lvl 10) → Halfway There (lvl 50) → Maximum Power (lvl 100)
7. Crafting Master (capstone requiring multiple prerequisites)

### Utility Questline
- **File:** `config/ftbquests/quests/chapters/utility.snbt`
- **Theme:** Miscellaneous tasks, utility actions
- **Color:** Purple (&d)
- **Total Quests:** 15
- **Lines:** 601
- **Quest IDs:** 5000000000000001 - 5000000000000055

**Quest Progression:**
1. Ball throwing: First Throw → Ball Thrower (50)
2. Scanning: Research Assistant → Dedicated Researcher (25)
3. Trading: First Trade → Trade Complete
4. Pokédex: Pokédex Started (10) → Growing Database (25) → Expert Researcher (50)
5. Evolution Stones → Stone Collector
6. Berries: Berry Picker → Berry Expert
7. Sweet Treat (Rare Candy), Tough Choices (Release)

## Total Quest Count
- **Welcome Quest:** 1
- **Adventure:** 12
- **Catching:** 18
- **Battling:** 16
- **Progression:** 17
- **Utility:** 15
- **TOTAL:** 79 unique quests

## Dependencies Structure

### Global Dependencies
- All questlines start from "Welcome to Cobblemon!" (ID: 0000000000000002)

### Internal Dependencies
Each questline has its own dependency chain:
- Linear progressions (easy → medium → hard)
- Parallel paths (type-specific quests)
- Capstone quests (requiring multiple prerequisites)

### No Cross-Questline Dependencies
- Each questline is independent
- Players can progress through any questline in any order
- Promotes player choice and flexibility

## Reward Distribution

### Common Rewards
- Poké Balls (all types)
- Potions and healing items
- Emeralds, Gold, Diamonds
- Rare Candies

### Rare Rewards
- Master Balls (awarded for major achievements)
- Diamond Blocks
- Large quantities of resources

### Themed Rewards
- Adventure: Location-specific balls (Dive Ball, Nest Ball)
- Catching: Catching tools and storage
- Battling: Healing and revival items
- Progression: Crafting materials
- Utility: Mixed rewards

## Quest Format Verification

All quest files follow proper SNBT format:
✅ Opening and closing braces
✅ Proper field names
✅ Correct data types (strings, numbers, lists)
✅ Valid quest structure
✅ Unique IDs for all quests and tasks
✅ Valid dependency references

## File Integrity
✅ Main configuration file exists
✅ All 5 chapter files exist
✅ Proper directory structure
✅ No syntax errors in SNBT format
