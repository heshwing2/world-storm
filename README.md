# 🌪️ WORLD STORM - Battle Royale

![WORLD STORM](https://img.shields.io/badge/Game-Battle%20Royale-blue?style=flat-square)
![Players](https://img.shields.io/badge/Players-30%20(Solo%2FDuo)-green?style=flat-square)
![Status](https://img.shields.io/badge/Status-Development-yellow?style=flat-square)

## 🎮 Overview

**WORLD STORM** is a 3D third-person battle royale game built with Three.js. Survive on a mysterious island, fight 29 other players, master dynamic weather systems, and capture the legendary Storm Core to control the storm itself!

### ✨ Key Features

✅ **30-Player Battle Royale** (Solo & Duo modes)
✅ **Dynamic Storm System** - 5 special storm types
✅ **Storm Core Mechanic** - Capture to change weather
✅ **15 Island Locations** - Fully explorable world
✅ **6 Weapon Types** - Assault Rifle, SMG, Shotgun, Sniper, Pistol, Melee
✅ **Inventory & Loot System** - Weapons, ammo, healing, armor
✅ **Health & Armor System** - Strategic protection mechanics
✅ **AI Bots** - Realistic enemy behavior (up to 29)
✅ **Storm Warden Boss** - Legendary protector of the core
✅ **Third-Person Camera** - Smooth follow camera
✅ **Mobile Support** - Virtual joystick & touch controls
✅ **Multiplayer Ready** - WebSocket support prepared

---

## 🎯 Game Modes

### SOLO
- 30 individual players
- Last player standing wins
- Full freedom and tactics

### DUO
- 15 teams of 2 players
- Team cooperation required
- One captures core = both get protection
- One elimination = team eliminated

---

## 🗺️ Island Locations (15)

1. **Big City** - Urban center with tall buildings
2. **Small Village** - Rural farming area
3. **Port** - Coastal docks and warehouses
4. **Beach** - Sandy shores with scattered debris
5. **Industrial Area** - Factories and refineries
6. **Mountains** - Rocky peaks and cliffs
7. **Mountain Village** - Highland settlement
8. **Forest** - Dense woodlands
9. **Jungle** - Thick vegetation and undergrowth
10. **Waterfalls** - Cascading water features
11. **Jungle Ruins** - Ancient structures
12. **Caves** - Underground caverns
13. **Underground Paths** - Connected tunnel system
14. **Volcano** - Volcanic mountain with lava
15. **Central Storm Core** - The legendary core location

---

## ⚔️ Weapons & Combat

| Weapon | Damage | ROF | Accuracy | Magazine | Range |
|--------|--------|-----|----------|----------|-------|
| Assault Rifle | 35 | 600 | 0.8 | 30 | 600m |
| SMG | 20 | 900 | 0.7 | 35 | 450m |
| Shotgun | 80 | 100 | 0.5 | 8 | 300m |
| Sniper | 100 | 40 | 1.0 | 10 | 2500m |
| Pistol | 25 | 300 | 0.6 | 15 | 300m |
| Melee | 50 | Instant | 1.0 | - | 2m |

---

## 🌪️ Storm System

### Storm Phases
1. **Safe Zone Appears** - Blue circle indicates safe area
2. **Warning Ring** - Red zone shows damage area
3. **Shrink Phase 1** - First contraction
4. **Damage Ring Active** - Outside zone takes damage
5. **Shrink Phase 2** - Second contraction
6. **Final Zone** - Storm Core location revealed

### Special Storms (5 Types)

🌀 **Tornado**
- High wind effects, knockback
- Reduced visibility
- Damage: 5 HP/second

⚡ **Lightning Storm**
- Electrical strikes, visual effects
- Chain lightning to nearby players
- Damage: 10 HP/second

🔥 **Firestorm**
- Burning damage, fire particles
- Reduced visibility from smoke
- Damage: 8 HP/second

❄️ **Ice Storm**
- Slow movement (50%)
- Freezing visual effects
- Damage: 3 HP/second

💧 **Floodstorm**
- Rising water level
- Environmental obstacles
- Damage: 6 HP/second

---

## 💗 Health & Armor System

### Health
- **Base Health**: 100 HP
- **Medkit**: +75 HP
- **Bandage**: +10 HP
- **Death**: 0 HP = Elimination

### Armor
- **Base Armor**: 100 Armor Points
- **Armor Plate**: +50 Armor
- **Damage Flow**: Armor absorbs 75% of damage first
- **Remaining damage**: Goes to health

### Damage Calculation
```
Incoming Damage: 40
Armor Reduction: 40 × 0.75 = 30
Armor Damage: 30
Health Damage: 40 - 30 = 10
```

---

## 🎮 Controls

### PC
| Action | Key |
|--------|-----|
| Move Forward | W |
| Move Left | A |
| Move Backward | S |
| Move Right | D |
| Sprint | Shift |
| Jump | Space |
| Crouch | C |
| Reload | R |
| Shoot | Left Mouse |
| Aim | Right Mouse |
| Interact | E |
| Inventory | I |
| Map | M |
| Look Around | Mouse Move |
| Free Look | Hold Middle Mouse |

### Mobile
| Action | Control |
|--------|----------|
| Move | Left Joystick |
| Look | Right Joystick |
| Jump | A Button |
| Crouch | X Button |
| Shoot | Fire Button (Right) |
| Reload | Y Button |
| Sprint | Double tap forward |

---

## 🎯 Storm Core & Capture System

### How to Capture
1. Locate the Storm Core (center of map)
2. Enter the capture radius (50m)
3. Progress bar starts filling
4. Enemy interrupts = combat required
5. Successful capture = 30-60 second protection
6. Defend your captured core
7. Storm type changes based on captor

### Storm Warden (Boss)
- **Health**: 200 HP
- **Armor**: 100 Armor Points
- **Damage Per Hit**: 25 HP
- **Special Attacks**: AoE blast, chase sequence
- **AI Behavior**: Idle → Patrol → Detect → Chase → Attack → Retreat
- **Location**: Always at Storm Core
- **Rewards**: Legendary loot + 500 XP

---

## 🤖 AI Bot System

### Bot Behaviors
1. **Explore** - Roam the map
2. **Loot** - Search for weapons and items
3. **Detect** - Spot enemies nearby
4. **Combat** - Engage in fight
5. **Cover** - Take defensive positions
6. **Retreat** - Flee when health low
7. **Storm** - Escape storm damage
8. **Core** - Navigate to Storm Core
9. **Capture** - Attempt core capture
10. **Defend** - Protect captured core

### Bot Progression
- Start: 5 bots
- Mid-game: 15 bots
- Late-game: 25-29 bots
- Difficulty increases with time

---

## 🏆 Victory & Rewards

### Victory Screen
```
POSITION:      #1 (Winner!)
KILLS:         5
DAMAGE:        2,341
SURVIVAL TIME: 12:45
```

### Rewards
- **XP**: Based on position and kills
- **Coins**: In-game currency
- **Skins**: Cosmetic character customization
- **Items**: Weapon skins, trails, emotes
- **Achievements**: Unlockable badges

---

## 📊 Technical Specifications

### Technology Stack
- **Rendering**: Three.js 3D Engine
- **Physics**: Cannon.js (physics simulation)
- **Networking**: WebSocket (multiplayer ready)
- **Audio**: Web Audio API
- **UI**: HTML5/CSS3
- **Mobile**: Touch event handling

### Browser Support
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+
- Mobile (iOS 14+, Android 10+)

### Performance Targets
- 60 FPS on high-end devices
- 30 FPS on low-end devices
- Mobile: 30-60 FPS depending on settings

---

## 📁 Project Structure

```
WORLD-STORM/
├── index.html                    # Main entry point
├── README.md                     # This file
├── LICENSE                       # MIT License
├── .gitignore                   # Git ignore rules
│
├── css/                         # Stylesheets
│   ├── style.css               # Main game styling
│   ├── menu.css                # Main menu
│   ├── hud.css                 # HUD elements
│   ├── inventory.css           # Inventory UI
│   ├── settings.css            # Settings menu
│   └── mobile.css              # Mobile responsive
│
├── js/                         # JavaScript code
│   ├── main.js                 # Game entry point
│   │
│   ├── player/                 # Player systems
│   │   ├── Player.js           # Player class
│   │   ├── PlayerController.js # Input handling
│   │   ├── PlayerHealth.js     # Health & armor
│   │   ├── PlayerInventory.js  # Inventory
│   │   └── PlayerAnimation.js  # Animations
│   │
│   ├── camera/                 # Camera systems
│   │   ├── ThirdPersonCamera.js# Follow camera
│   │   └── CameraController.js # Camera input
│   │
│   ├── world/                  # World systems
│   │   ├── World.js            # World manager
│   │   ├── Terrain.js          # Terrain generation
│   │   ├── Buildings.js        # Building placement
│   │   ├── Roads.js            # Road system
│   │   └── Locations.js        # Location definitions
│   │
│   ├── weapons/                # Weapon systems
│   │   ├── WeaponSystem.js    # Weapon manager
│   │   ├── Weapon.js          # Base weapon class
│   │   ├── AssaultRifle.js    # AR implementation
│   │   ├── SMG.js             # SMG implementation
│   │   ├── Shotgun.js         # Shotgun implementation
│   │   ├── Sniper.js          # Sniper implementation
│   │   ├── Pistol.js          # Pistol implementation
│   │   └── Melee.js           # Melee implementation
│   │
│   ├── loot/                   # Loot systems
│   │   ├── LootSystem.js       # Loot manager
│   │   ├── LootItem.js         # Loot item class
│   │   └── LootSpawner.js      # Spawning system
│   │
│   ├── storm/                  # Storm systems
│   │   ├── StormSystem.js      # Storm manager
│   │   ├── SafeZone.js         # Safe zone logic
│   │   ├── StormDamage.js      # Damage calculation
│   │   └── SpecialStorms.js    # Special storm types
│   │
│   ├── core/                   # Storm Core systems
│   │   ├── StormCore.js        # Core manager
│   │   ├── CaptureSystem.js    # Capture mechanics
│   │   └── CoreEffects.js      # Visual effects
│   │
│   ├── ai/                     # AI systems
│   │   ├── Bot.js              # Bot class
│   │   ├── BotAI.js            # AI decision logic
│   │   ├── BotCombat.js        # Combat AI
│   │   ├── BotLoot.js          # Looting AI
│   │   └── BotNavigation.js    # Navigation AI
│   │
│   ├── boss/                   # Boss systems
│   │   ├── StormWarden.js      # Warden class
│   │   └── WardenAI.js         # Warden AI
│   │
│   ├── game/                   # Game systems
│   │   ├── Game.js             # Game manager
│   │   ├── GameState.js        # Game state
│   │   ├── GameMode.js         # Mode selection
│   │   ├── Match.js            # Match logic
│   │   └── Victory.js          # Victory screen
│   │
│   ├── ui/                     # UI systems
│   │   ├── HUD.js              # Heads-up display
│   │   ├── MainMenu.js         # Main menu
│   │   ├── InventoryUI.js      # Inventory display
│   │   ├── MapUI.js            # Map display
│   │   ├── SettingsUI.js       # Settings menu
│   │   └── Notification.js     # Notifications
│   │
│   ├── audio/                  # Audio systems
│   │   └── AudioManager.js     # Audio playback
│   │
│   ├── effects/                # Effect systems
│   │   ├── ParticleEffects.js  # Particle system
│   │   ├── WeatherEffects.js   # Weather effects
│   │   └── StormEffects.js     # Storm effects
│   │
│   ├── mobile/                 # Mobile systems
│   │   ├── TouchControls.js    # Touch handling
│   │   ├── VirtualJoystick.js  # Virtual joystick
│   │   └── MobileHUD.js        # Mobile UI
│   │
│   └── settings/               # Settings systems
│       ├── GraphicsSettings.js # Graphics options
│       ├── AudioSettings.js    # Audio options
│       └── ControlsSettings.js # Control options
│
├── assets/                     # Game assets
│   ├── models/                # 3D models
│   │   ├── characters/        # Player models
│   │   ├── weapons/           # Weapon models
│   │   ├── buildings/         # Building models
│   │   ├── vehicles/          # Vehicle models
│   │   ├── environment/       # Environment models
│   │   └── boss/              # Boss models
│   │
│   ├── textures/              # Textures
│   │   ├── terrain/           # Terrain textures
│   │   ├── buildings/         # Building textures
│   │   ├── characters/        # Character textures
│   │   └── weapons/           # Weapon textures
│   │
│   ├── sounds/                # Audio files
│   │   ├── weapons/           # Weapon sounds
│   │   ├── player/            # Player sounds
│   │   ├── environment/       # Environmental sounds
│   │   ├── storm/             # Storm sounds
│   │   └── boss/              # Boss sounds
│   │
│   └── effects/               # Effect assets
│       ├── fire/              # Fire effects
│       ├── lightning/         # Lightning effects
│       ├── tornado/           # Tornado effects
│       ├── ice/               # Ice effects
│       ├── flood/             # Water effects
│       └── core/              # Core effects
│
├── data/                      # Game data
│   ├── weapons.json          # Weapon stats
│   ├── items.json            # Item definitions
│   ├── locations.json        # Location data
│   ├── storm.json            # Storm configuration
│   └── game-settings.json    # Game settings
│
├── docs/                      # Documentation
│   ├── GAME_DESIGN.md        # Game design doc
│   ├── CONTROLS.md           # Control guide
│   ├── MAP.md                # Map documentation
│   ├── WEAPONS.md            # Weapon guide
│   ├── STORMS.md             # Storm system guide
│   └── DEVELOPMENT_ROADMAP.md# Development plan
│
└── server/                    # Backend (optional)
    ├── server.js             # Express server
    ├── game-server.js        # WebSocket server
    ├── player-server.js      # Player management
    └── package.json          # Dependencies
```

---

## 🚀 Quick Start

### Prerequisites
- Modern web browser
- Node.js 14+ (for server)
- npm or yarn

### Installation

```bash
# Clone repository
git clone https://github.com/heshwing2/WORLD-STORM.git
cd WORLD-STORM

# Install dependencies
npm install

# Start development server (optional)
node server/server.js

# Open in browser
# http://localhost:3000
```

### Running the Game

1. Open `index.html` in a web browser
2. Click "PLAY" to start
3. Select game mode (Solo/Duo)
4. Drop onto the island
5. Survive and win!

---

## 🎓 Development Guide

### Adding a New Weapon

```javascript
// Create js/weapons/NewWeapon.js
class NewWeapon extends Weapon {
  constructor() {
    super('New Weapon', {
      damage: 40,
      fireRate: 700,
      accuracy: 0.85,
      magazine: 25,
      reloadTime: 2.5,
      range: 800
    });
  }
}
```

### Adding a New Location

```javascript
// Edit data/locations.json
{
  "id": 16,
  "name": "New Location",
  "position": {"x": 500, "y": 0, "z": 500},
  "size": 200,
  "lootTier": "legendary",
  "description": "A mysterious new place"
}
```

### Adding a New Storm Type

```javascript
// Create StormType class in SpecialStorms.js
class CustomStorm extends SpecialStorm {
  constructor() {
    super('Custom Storm', {
      damage: 7,
      duration: 45,
      effect: 'custom'
    });
  }
}
```

---

## 📊 Development Roadmap

### Phase 1-6: Core Systems (Weeks 1-3)
- ✅ Player & Camera
- ✅ Island & Terrain
- ✅ Weapons System
- ✅ Loot & Inventory
- ✅ Storm System
- ✅ Health & Armor

### Phase 7-12: Advanced Gameplay (Weeks 4-6)
- 🔄 Storm Core & Capture
- 🔄 Storm Warden Boss
- 🔄 Special Storms
- 🔄 AI Bots
- 🔄 Solo/Duo Modes
- 🔄 Victory System

### Phase 13-18: Polish & Platforms (Weeks 7-9)
- 🔄 Graphics Optimization
- 🔄 Audio Polish
- 🔄 Performance Testing
- 🔄 Android Build
- 🔄 iOS Build
- 🔄 Windows Build

### Phase 19-24: Launch Prep (Weeks 10-12)
- 🔄 Mobile Optimization
- 🔄 Bug Fixes
- 🔄 Multiplayer (Optional)
- 🔄 Publishing
- 🔄 Marketing
- 🔄 Community

### Phase 25-36: Post-Launch (Months 4-6)
- 🔄 Events & Updates
- 🔄 New Maps
- 🔄 Seasonal Content
- 🔄 Cosmetics
- 🔄 Esports Ready
- 🔄 World Expansion

---

## 🐛 Known Issues

- Mobile performance on older devices needs optimization
- Multiplayer networking layer not yet implemented
- Some storm effects may lag on low-end PCs

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

## 👨‍💻 Authors

- **Lead Developer**: heshwing2
- **Game Design**: WORLD STORM Team

---

## 🙏 Acknowledgments

- Three.js community for amazing 3D library
- Cannon.js for physics simulation
- All contributors and testers

---

## 📞 Support

For issues, questions, or suggestions:
- GitHub Issues: https://github.com/heshwing2/WORLD-STORM/issues
- Discussions: https://github.com/heshwing2/WORLD-STORM/discussions

---

## 🎮 Let's Build WORLD STORM!

**Survive the storm. Control the legend. Be the last standing.** ⛈️

---

*Last Updated: 2024*
*Status: Active Development*