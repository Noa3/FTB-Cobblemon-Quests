# FTB Cobblemon Quests

A comprehensive questpack for the Cobblemon mod using FTB Quests, designed to guide players through their Pokémon journey with structured progression and rewarding challenges.

## 📋 Overview

This questpack provides a complete quest system for Cobblemon, featuring multiple questlines that cover all aspects of the Pokémon experience. Players will explore the world, catch Pokémon, battle trainers, craft essential items, and complete various utility tasks.

## ✨ Features

- **5 Main Questlines** with over 80+ quests
- **Progressive Difficulty** from beginner to master level
- **Rich Rewards** including Poké Balls, items, and resources
- **Dependency System** ensuring logical progression
- **Comprehensive Coverage** of all Cobblemon features

## 📦 Installation

### Prerequisites

1. **Minecraft** (compatible version with Cobblemon)
2. **Fabric Loader** or **Forge** (depending on your setup)
3. **Cobblemon** mod ([Download](https://modrinth.com/mod/cobblemon))
4. **FTB Quests** mod ([Download](https://www.curseforge.com/minecraft/mc-mods/ftb-quests-fabric))
5. **Cobblemon Quests** mod ([Download](https://modrinth.com/mod/cobblemon-quests))

### Installation Steps

#### For Server Administrators:

1. Download this questpack
2. Navigate to your server directory
3. Copy the `config/ftbquests` folder to your server's `config` directory
4. If the folder already exists, merge or replace it (backup existing quests first!)
5. Restart your server
6. Players will see the quests in their FTB Quests book

#### For Single Player:

1. Download this questpack
2. Navigate to your Minecraft instance directory
3. Copy the `config/ftbquests` folder to your instance's `config` directory
4. If the folder already exists, merge or replace it (backup existing quests first!)
5. Launch Minecraft
6. Open your FTB Quests book to see the quests

#### Using a Modpack:

1. If creating a modpack, include the `config/ftbquests` folder in your modpack files
2. Distribute the modpack with these quests pre-installed

## 🗺️ Quest Structure

### Main Questlines

#### 🌍 Adventure Questline (Blue)
Explore the world and discover new biomes and dimensions!

**Quests Include:**
- Biome exploration (Plains, Forest, Ocean, Desert, Taiga, Jungle, Mountains, Rivers)
- Dimension travel (Nether, The End)
- Location discovery challenges
- **Rewards:** Various Poké Balls, emeralds, and exploration gear

**Progression:** Start with basic biomes → Master all biomes → Enter other dimensions

#### 🎯 Catching Questline (Orange)
Build your Pokémon collection!

**Quests Include:**
- First catch milestone
- Collection goals (10, 25, 50+ Pokémon)
- Type-specific catches (Water, Fire, Grass, Electric, Psychic, Dragon, Ghost, Dark)
- Evolution challenges
- Shiny hunting
- **Rewards:** Poké Balls, Rare Candies, Master Balls, and valuable items

**Progression:** Single catch → Type variety → Large collection → Rare finds

#### ⚔️ Battling Questline (Red)
Become a battle master!

**Quests Include:**
- Wild Pokémon battles (1, 10, 25, 50+ battles)
- Player battles (PvP challenges)
- NPC trainer battles
- Type-specific battles
- Level-based challenges (Level 30+, 50+)
- **Rewards:** Potions, Revives, Full Restores, healing items

**Progression:** First battle → Experience building → Advanced challenges

#### 🛠️ Progression Questline (Green)
Craft and develop your tools!

**Quests Include:**
- Poké Ball crafting (Poké Ball → Great Ball → Ultra Ball)
- Medicine crafting (Potions, Super Potions, Hyper Potions, Full Restores)
- Revival items (Revive, Max Revive)
- Essential items (PC, Healing Machine)
- Resource gathering (Apricorns, Medicinal Leeks)
- Pokémon training (Level milestones: 10, 50, 100)
- **Rewards:** Crafting materials, rare items, Master Balls

**Progression:** Basic items → Advanced healing → Ultimate crafting mastery

#### 💎 Utility Questline (Purple)
Complete miscellaneous tasks!

**Quests Include:**
- Poké Ball throwing practice
- Pokédex scanning and registration
- Trading tasks
- Pokémon release management
- Evolution stone collection
- Berry gathering
- **Rewards:** Varied items, resources, and special rewards

**Progression:** Basic utility tasks → Advanced collection goals

### Quest Dependencies

Quests are designed with logical dependencies:

1. **Welcome Quest** - The starting point for all questlines
2. **Early Quests** - Basic tasks that unlock parallel paths
3. **Mid-tier Quests** - Specialized challenges requiring early quest completion
4. **Master Quests** - Final challenges requiring multiple prerequisites

## 🎁 Reward System

### Types of Rewards:

- **Poké Balls:** Poke Ball, Great Ball, Ultra Ball, Master Ball, and specialty balls
- **Medicine:** Potions, Super Potions, Hyper Potions, Full Restores
- **Revival:** Revive, Max Revive
- **Training:** Rare Candies, Evolution Stones
- **Resources:** Emeralds, Diamonds, Gold, Iron
- **Berries:** Oran, Sitrus, Pecha, Cheri berries

### Reward Progression:

- Early quests: Basic Poké Balls and simple items
- Mid-tier quests: Better balls and valuable resources
- Master quests: Master Balls, diamond blocks, and rare items

## 🎮 How to Use

### For Players:

1. **Open Quest Book:** Press the FTB Quests keybind (default: usually assigned in controls)
2. **Start with Welcome Quest:** Complete the introductory quest to unlock questlines
3. **Choose Your Path:** Select which questline interests you most
4. **Complete Tasks:** Follow quest descriptions to complete objectives
5. **Claim Rewards:** Click on completed quests to claim your rewards
6. **Track Progress:** Use the quest book to see your overall progress

### For Quest Pack Creators:

This questpack serves as a template. You can:

- Modify quest rewards to match your server economy
- Add custom NPC names for NPC battle quests
- Adjust difficulty by changing quest requirements
- Add new quests following the existing structure
- Customize descriptions to match your server theme

## 🔧 Quest Customization

### Editing Quest Files:

All quest files are located in `config/ftbquests/quests/`:

- `quests.snbt` - Main quest configuration
- `chapters/adventure.snbt` - Adventure questline
- `chapters/catching.snbt` - Catching questline
- `chapters/battling.snbt` - Battling questline
- `chapters/progression.snbt` - Progression questline
- `chapters/utility.snbt` - Utility questline

### Quest File Format:

Quests use SNBT (Stringified NBT) format. Each quest contains:

```
{
    id: "unique_id"                    // Unique quest identifier
    dependencies: ["quest_id"]          // Required quests
    description: ["Text lines"]         // Quest description
    icon: "item_id"                     // Display icon
    rewards: [...]                      // Quest rewards
    tasks: [...]                        // Quest objectives
    title: "Quest Name"                 // Display name
    x: 0.0d                            // X position in quest tree
    y: 0.0d                            // Y position in quest tree
}
```

### Cobblemon Task Parameters:

Cobblemon quests support these parameters:

- `action`: catch, defeat, evolve, level_up, throw_ball, scan, trade_away, trade_for, etc.
- `amount`: Number required
- `pokemon`: Specific Pokémon species
- `pokemon_type`: Pokémon type (fire, water, grass, etc.)
- `min_level`/`max_level`: Level requirements
- `shiny`: true/false for shiny requirement
- `biome`: Biome requirement
- `dimension`: Dimension requirement
- `gender`: Gender requirement
- `region`: Generation/region
- `form`: Form/aspect requirement

## 📖 Quest Design Philosophy

This questpack follows these principles:

1. **Progressive Difficulty:** Start easy, get harder
2. **Parallel Paths:** Multiple questlines can be completed simultaneously
3. **Meaningful Rewards:** Rewards match quest difficulty
4. **Clear Goals:** Every quest has a clear, achievable objective
5. **Logical Dependencies:** Quests unlock in a sensible order
6. **Balanced Progression:** No single questline gates others excessively
7. **Cobblemon Integration:** All quests use Cobblemon mechanics

## 🐛 Troubleshooting

### Quests Not Appearing:

1. Verify Cobblemon Quests mod is installed
2. Check that FTB Quests mod is installed
3. Ensure files are in the correct `config/ftbquests` directory
4. Restart your game/server after adding quest files
5. Check console for errors related to quest loading

### Quest Not Completing:

1. Verify you meet all task requirements
2. Check quest dependencies are completed
3. For Cobblemon tasks, ensure the action is correctly performed
4. Check server/client logs for errors
5. Try relogging if the quest seems stuck

### Reward Issues:

1. Ensure your inventory has space
2. Check if rewards require specific conditions
3. Verify the quest is actually marked as complete

## 🤝 Contributing

Want to improve this questpack?

1. Fork the repository
2. Make your changes
3. Test thoroughly
4. Submit a pull request with clear descriptions

## 📜 Credits

- **Cobblemon Team:** For the amazing Pokémon mod
- **WinterWolfSV:** For the Cobblemon Quests integration mod
- **FTB Team:** For the FTB Quests framework
- **Quest Pack Creator:** Noa3

## 📄 License

This questpack is released under the MIT License. Feel free to use, modify, and distribute for any purpose.

## 🔗 Useful Links

- [Cobblemon Mod](https://modrinth.com/mod/cobblemon)
- [Cobblemon Quests Mod](https://modrinth.com/mod/cobblemon-quests)
- [FTB Quests](https://www.curseforge.com/minecraft/mc-mods/ftb-quests-fabric)
- [Cobblemon Discord](https://discord.gg/cobblemon)
- [Quest Creation Documentation](https://github.com/WinterWolfSV/Cobblemon_Quests/blob/master/quest-creation.md)

## 📞 Support

For issues or questions:

1. Check this README
2. Review the Troubleshooting section
3. Check the Cobblemon Quests mod documentation
4. Ask in the Cobblemon Discord
5. Open an issue on this repository

---

**Happy Questing, Trainer!** 🎮✨
