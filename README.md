# Incremancer 🧙‍♂️💀

An idle necromancer game where you command hordes of zombies to ravage small towns and unlock powerful dark magic. This is a modified version by Chalice featuring quality-of-life improvements and enhanced gameplay mechanics.

![Incremancer Start Screen](https://github.com/user-attachments/assets/c75f59fa-9659-4563-a4b0-5656eeebd79b)

## 🎮 Game Overview

Take control of an undead army and spread chaos across the land! Start with basic zombie summoning and evolve into a master necromancer with access to powerful spells, automated minions, and ancient runes.

### Core Gameplay
- **Summon Zombies**: Click to spawn zombies using energy (10 energy per zombie)
- **Resource Management**: Collect Blood, Brains, Bones, and Parts from your conquests
- **Progressive Upgrades**: Unlock new abilities and structures through a comprehensive tech tree
- **Level Progression**: Conquer increasingly difficult towns with more humans and defenses
- **Prestige System**: Reset for permanent bonuses when you reach higher levels

### Key Features
- 🧟 **Interactive 2D World**: Drag to explore, zoom with mouse wheel
- ⚡ **Automation Systems**: Auto-upgrades, auto-construction, and auto-spawning
- 🏗️ **Construction**: Build structures like Graveyards, Factories, and Runesmithies
- 🎯 **Spell System**: Cast powerful spells with cooldowns and energy costs
- 💀 **Skeleton Companion**: Unlock at level 50+ for additional gameplay
- 📊 **Deep Progression**: Multiple resource types and upgrade paths

## 🛠️ Technical Architecture

### Built With
- **Frontend Framework**: AngularJS for application structure and data binding
- **Graphics Engine**: PIXI.js for 2D sprite rendering and animations
- **Bundling**: JavaScript modules compiled to `dist/bundle.js`
- **Templates**: Modular HTML templates for different game menus
- **Sprites**: JSON-defined sprite sheets for game entities

### File Structure
```
incremancer/
├── index.html          # Main game page
├── dist/bundle.js      # Compiled game logic
├── js/                 # External libraries (Angular, PIXI, etc.)
├── templates/          # HTML templates for game menus
├── sprites/            # JSON sprite definitions
├── images/             # Game assets and icons
└── zombiemancer.css    # Game styling
```

### How to Run
1. Clone the repository
2. Serve the files using any HTTP server:
   ```bash
   python3 -m http.server 8000
   # or
   npx serve .
   ```
3. Open `http://localhost:8000` in your browser
4. Start playing!

## 📈 Complete Tech Tree & Progression Guide

### 🩸 Blood Upgrades (Combat & Survivability)

![Shop - Brains Tab](https://github.com/user-attachments/assets/a6b57ab9-4f06-46a2-80ed-1b6a09c53e6f)

| Upgrade | Cost | Effect | Description |
|---------|------|--------|-------------|
| **Bloodthirst** | 50 Blood | +1 zombie damage | Increases the attack power of your zombies |
| **Like Leather** | 100 Blood | +10 zombie health | Makes your zombies more durable in combat |
| **Cold Storage** | 150 Blood | +50 max brains | Increases brain storage capacity |
| **Recycling is Cool** | 1K Blood | +10% brain recovery chance | Chance to recover brains from defeated zombies |
| **Your Soul is Mine!** | 1.5K Blood | +10% corpse → zombie chance | Higher chance for corpses to become zombies |

### 🧠 Brain Upgrades (Energy & Efficiency)

| Upgrade | Cost | Effect | Description |
|---------|------|--------|-------------|
| **Primal Reflexes** | 5 Brains | +1 zombie speed | Zombies move and attack faster |
| **Master Summoner** | 10 Brains | +5 max energy | Increases energy capacity for more zombie summoning |
| **Energy Rush** | 20 Brains | +0.5 energy/second | Faster energy regeneration |
| **Unholy Construction** | 25 Brains | Unlocks Construction | Access to building system |
| **Blood Harvest** | 50 Brains | +10% max blood | Increases blood storage capacity |

### 🏗️ Construction System

#### Available Structures

**Cursed Graveyard** 
- **Bone Collectors**: Hire minions to gather bones automatically (1 energy/sec each)
- **Auto Spawning**: Set zombies to spawn automatically when energy is full
- **Trophy System**: Collect achievements and bonuses

**Factory**
- **Parts Production**: Machines generate creature parts over time
- **Monster Factory**: Create advanced creatures with higher stats
- **Creature Management**: Set limits and auto-production

**Runesmith**
- **Rune of Life**: Defensive enhancements through resource infusion
  - Blood → Damage Reduction
  - Brains → Health Regeneration  
  - Bones → Damage Reflection
- **Blood Sated System**: Advanced rune mechanics

### 💀 Bone Economy (Mid-Game)
Unlocked via Graveyard construction:
- Bone Collectors gather bones from defeated enemies
- Bones used for advanced construction projects
- Enables automated resource collection

### ⚙️ Parts Economy (Late Game)  
Unlocked via Factory construction:
- Machines produce creature parts over time
- Parts used to create powerful monsters
- Advanced automation and creature management

### 🏆 Prestige System
- Reset progress at higher levels for prestige points
- Permanent upgrades that persist across resets
- Multiplicative bonuses to core game mechanics
- Access to prestige-only upgrades and features

## 💾 Resource Types & Management

### Primary Resources
- **Energy**: Regenerates over time, used for zombie summoning (starts at 10 max)
- **Blood**: Collected when zombies attack humans, used for combat upgrades
- **Brains**: Earned by killing/converting humans (1 per human), used for efficiency upgrades

### Advanced Resources (Unlocked)
- **Bones**: Gathered by bone collectors from casualties, used for construction
- **Parts**: Produced by factory machines, used for creating advanced creatures

### Storage & Capacity
- All resources have maximum storage limits
- Upgrades increase storage capacity
- Higher level areas provide more resources per action

## 🎯 Spell System & Special Abilities

### Energy-Based Spells
- Various spells with cooldown timers
- Energy costs scale with spell power
- Unlocked through progression and upgrades

### Skeleton Companion (Level 50+)
- Persistent companion with its own leveling system
- Can die and resurrect with timers
- Provides additional combat and resource bonuses

## 🌍 Level Progression & Difficulty

### Level Structure
- Each level represents a different town/area
- Increasing human count and defensive capabilities
- New challenges and enemy types introduced
- Boss encounters and special objectives

### Victory Conditions
- Eliminate or convert all humans in the area
- Collect bonus resources upon completion
- Unlock access to next level
- Earn prestige points at higher levels

## 🔧 Quality of Life Features

This modified version includes several improvements:
- **Enhanced UI**: Better visual feedback and information display
- **Automation Options**: Multiple auto-buy and auto-build systems  
- **Improved Controls**: Keyboard navigation (WASD/arrows) and better mouse controls
- **Performance**: Optimized rendering and game loop
- **Balance**: Adjusted progression curves and resource costs

## 🎮 Controls & Interface

### Basic Controls
- **Left Click**: Spawn zombie (requires 10 energy)
- **Shift/Ctrl + Click**: Spawn multiple zombies
- **Mouse Drag**: Move camera around the world
- **Mouse Wheel**: Zoom in/out
- **WASD/Arrow Keys**: Navigate the world

### UI Elements
- **Top Bar**: Level, stats, human/zombie counts
- **Resource Bar**: Energy, Blood, Brains (+ Bones/Parts when unlocked)
- **Side Panels**: Shop, Construction, specialized menus
- **Spell Bar**: Active spells and cooldown timers

## 🔗 Community & Support

- **Discord**: [Join the community](https://discord.gg/TxPyNDh)
- **Original Game**: This is a community modification with enhanced features
- **Bug Reports**: Use GitHub issues for technical problems

---

**Note**: This is an unofficial modification of the original Incremancer game, enhanced with quality-of-life improvements and additional features by Chalice.
