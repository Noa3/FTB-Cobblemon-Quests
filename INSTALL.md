# Quick Installation Guide

## For Players

### What You Need
1. Minecraft with Fabric or Forge
2. Cobblemon mod installed
3. FTB Quests mod installed
4. Cobblemon Quests mod installed

### Installation Steps
1. Download this questpack (the entire repository)
2. Find your Minecraft directory:
   - **Windows:** `%appdata%\.minecraft`
   - **Mac:** `~/Library/Application Support/minecraft`
   - **Linux:** `~/.minecraft`
3. Navigate to the `config` folder in your Minecraft directory
4. Copy the `ftbquests` folder from this questpack into your `config` folder
5. Launch Minecraft
6. Open your quest book (check keybinds, usually a button in inventory or a key)
7. Start with "Welcome to Cobblemon!" quest

## For Server Administrators

### Installation Steps
1. Download this questpack
2. Navigate to your server directory
3. Copy the `config/ftbquests` folder to your server's `config` directory
4. Restart the server
5. Players will automatically receive the quests when they join

### Important Notes
- Quest progress is saved per-player on the server
- If you update quests, existing player progress may be affected
- Always backup the `config/ftbquests` folder before making changes
- Quest files are in SNBT format (similar to JSON)

## For Modpack Creators

### Including in Your Modpack
1. Include the `config/ftbquests` folder in your modpack distribution
2. Make sure to include these mods as dependencies:
   - Cobblemon
   - FTB Quests
   - Cobblemon Quests
3. The quests will be available immediately when players start

### Customization
You can customize:
- Reward amounts (edit the quest files)
- Quest descriptions
- Quest positions in the tree
- Add your own custom quests
- Remove quests you don't want

See README.md for detailed customization instructions.

## Troubleshooting

### Quests Not Showing
- ✅ Check all required mods are installed
- ✅ Verify files are in `config/ftbquests`
- ✅ Restart Minecraft/Server
- ✅ Check console for errors

### Quest Won't Complete
- ✅ Verify you completed the exact task
- ✅ Check dependencies are completed
- ✅ Try relogging
- ✅ Check if it's a Cobblemon task (requires Cobblemon Quests mod)

### Missing Items/Icons
- ✅ Ensure Cobblemon mod is installed
- ✅ Check mod version compatibility
- ✅ Verify all dependencies are met

## Getting Help

1. Read the full README.md
2. Check QUEST_STRUCTURE.md for quest details
3. Visit Cobblemon Discord for support
4. Check Cobblemon Quests mod documentation

## Quick Start for New Players

1. Complete "Welcome to Cobblemon!" quest
2. Choose a questline:
   - Like exploring? → Adventure (Blue)
   - Like collecting? → Catching (Orange)
   - Like battling? → Battling (Red)
   - Like crafting? → Progression (Green)
   - Like variety? → Utility (Purple)
3. Complete quests to earn rewards
4. Use rewards to progress faster
5. Enjoy your Pokémon journey!

---

**Need more help? Check README.md for full documentation!**
