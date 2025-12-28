# 🍬 Jelly Garden Match-3 Game

<div align="center">

**Language / 语言 / 言語:** [English](README.md) | [中文](README_zh.md) | [日本語](README_ja.md)

![Unity](https://img.shields.io/badge/Unity-2019.4+-black?style=flat-square&logo=unity)
![C#](https://img.shields.io/badge/C%23-8.0-blue?style=flat-square&logo=c-sharp)
![License](https://img.shields.io/badge/License-Proprietary-red?style=flat-square)
![Platform](https://img.shields.io/badge/Platform-iOS%20%7C%20Android-lightgrey?style=flat-square)

A complete Match-3 puzzle game template with modern features, social integration, and monetization ready.

[Features](#-features) • [Getting Started](#-getting-started) • [Project Structure](#-project-structure) • [Documentation](#-documentation) • [Support](#-support)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Getting Started](#-getting-started)
- [Project Structure](#-project-structure)
- [Core Systems](#-core-systems)
- [Integration & Services](#-integration--services)
- [Documentation](#-documentation)
- [Requirements](#-requirements)
- [Build & Deployment](#-build--deployment)
- [Contributing](#-contributing)
- [Support](#-support)
- [License](#-license)

---

## 🎮 Overview

**Jelly Garden Match-3** is a feature-rich Unity puzzle game template designed for mobile platforms. Built with scalability and customization in mind, it includes everything needed to launch a commercial Match-3 game, from level design tools to monetization systems.

### Key Highlights

- 🎯 **Complete Match-3 Mechanics**: Classic swap-and-match gameplay with special items and boosters
- 🗺️ **Smart Level System**: Advanced level editor with 100+ pre-built levels
- 💰 **Monetization Ready**: In-app purchases, ads integration, and virtual currency system
- 🌐 **Social Features**: Facebook integration, leaderboards, and friend systems
- 📱 **Cross-Platform**: iOS and Android support with optimized performance
- 🎨 **Polished UI/UX**: Beautiful animations, particle effects, and responsive design

---

## ✨ Features

### Core Gameplay

- **Match-3 Mechanics**

  - Classic swap-and-match gameplay
  - Special items: Bombs, Horizontal/Vertical Striped, Rainbow items
  - Combo system with visual effects
  - Multiple game modes and objectives

- **Level System**

  - 100+ unique pre-designed levels
  - Progressive difficulty curve
  - Star-based rating system (1-3 stars)
  - Multiple level objectives (score, ingredients, blocks, etc.)

- **Boosters & Power-ups**
  - Pre-game boosters
  - In-game boosters
  - Daily rewards system
  - Lives system with regeneration

### Technical Features

- **Level Editor**

  - Visual level designer
  - Drag-and-drop interface
  - Real-time preview
  - Import/Export functionality

- **Smart Map System**

  - Scrollable level map
  - Unlock progression
  - Visual level status indicators
  - Episode system

- **Animation System**
  - Smooth item transitions
  - Particle effects for matches
  - Screen shake effects
  - Reward animations

### Monetization

- **In-App Purchases**

  - Coin packages
  - Booster bundles
  - Lives purchases
  - Remove ads option

- **Advertisement Integration**

  - Rewarded video ads
  - Interstitial ads
  - Banner ads
  - Ad event system

- **Virtual Economy**
  - Soft currency (coins)
  - Purchase tracking
  - Reward distribution

### Social & Network

- **Facebook Integration**

  - Login system
  - Friend list
  - Avatar loading
  - Score sharing

- **Leaderboards**

  - Global rankings
  - Friend rankings
  - Offline support
  - Score synchronization

- **Cloud Services**
  - GameSparks integration
  - PlayFab integration
  - Data persistence
  - Cross-device sync

---

## 🚀 Getting Started

### Prerequisites

- **Unity**: 2019.4 LTS or higher (2020.3+ recommended)
- **Operating System**: Windows 10/11 or macOS 10.14+
- **IDE**: Visual Studio 2019+ or JetBrains Rider
- **Mobile SDKs**:
  - Android: SDK API Level 19+
  - iOS: Xcode 12+

### Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/NewbieAudioKid/example-jelly-garden-match-3-unity-5.3.4.git
   cd example-jelly-garden-match-3-unity-5.3.4
   ```

2. **Open in Unity**

   - Launch Unity Hub
   - Click "Add" and select the project folder
   - Open with Unity 2019.4 or higher
   - Wait for project initialization and package import

3. **Initial Setup**

   - Navigate to `Assets/JellyGarden/Scenes/`
   - Open `game.unity` scene for gameplay
   - Open `map.unity` scene for level selection

4. **Test the Game**
   - Click Play button in Unity Editor
   - Or build for your target platform

### Quick Configuration

**Basic Settings** (`InitScript.cs`):

```csharp
// Game Configuration
public int startLife = 5;           // Starting lives
public int startCoins = 100;        // Starting coins
public int levelToOpenEditor = 10;  // Level to unlock editor
```

**Level Configuration**:

- Levels stored in: `Assets/JellyGarden/Resources/Levels/`
- Edit levels using the built-in Level Editor
- Access via: Unity Menu → Window → Level Editor

---

## 📁 Project Structure

```
Jelly Garden Match 3/
│
├── Assets/
│   └── JellyGarden/
│       ├── Animation/          # Animation clips and controllers
│       │   ├── Item animations
│       │   ├── UI animations
│       │   └── Effect animations
│       │
│       ├── Audio/              # Sound effects and music
│       │   ├── BGM/
│       │   └── SFX/
│       │
│       ├── Fonts/              # Custom fonts and materials
│       │
│       ├── Materials/          # Particle and shader materials
│       │
│       ├── Prefabs/            # Reusable game objects
│       │
│       ├── Resources/          # Runtime loadable assets
│       │   ├── Levels/        # Level data files (.txt)
│       │   ├── Items/         # Match-3 items
│       │   └── UI/            # UI prefabs
│       │
│       ├── Scenes/             # Unity scenes
│       │   ├── game.unity     # Main gameplay scene
│       │   └── map.unity      # Level selection scene
│       │
│       ├── Scripts/            # C# source code
│       │   ├── System/        # Core game systems
│       │   ├── GUI/           # UI controllers
│       │   ├── Integrations/  # Third-party services
│       │   ├── Leadboard/     # Leaderboard system
│       │   └── Editor/        # Unity Editor extensions
│       │
│       ├── SmartLevelsMap/     # Level map system
│       │
│       ├── Textures/           # Sprites and images
│       │   ├── Items/
│       │   ├── UI/
│       │   └── Backgrounds/
│       │
│       └── Documentation/       # PDFs and guides
│
├── ProjectSettings/            # Unity project settings
├── Packages/                   # Package dependencies
└── README.md                   # This file
```

---

## 🔧 Core Systems

### Game Manager (`InitScript.cs`)

The central hub managing game state, initialization, and core gameplay loop.

**Key Responsibilities:**

- Game initialization and setup
- Level loading and management
- Player data persistence
- Score and objective tracking
- Game state management (playing, paused, completed)

**Important Methods:**

```csharp
InitGame()              // Initialize game systems
LoadLevel(int num)      // Load specific level
CheckWinLose()         // Check game completion conditions
SaveMapPlayerPrefs()   // Save player progress
```

### Match System (`CombineManager.cs`)

Handles all match detection, item combination, and special item generation.

**Features:**

- Match-3+ detection
- Special item creation rules
- Combo chain reactions
- Match scoring system

### Level Manager (`LevelManager.cs`)

Manages level data, objectives, and progression.

**Components:**

- Level data parser
- Objective tracking
- Star calculation
- Level completion logic

### Item System (`Item.cs`, `Square.cs`)

Controls individual game pieces and board squares.

**Item Types:**

- Simple items (6 colors)
- Striped (Horizontal/Vertical)
- Bombs
- Rainbow items
- Package items

---

## 🌐 Integration & Services

### Facebook Integration

**Setup:**

1. Create Facebook App at [developers.facebook.com](https://developers.facebook.com)
2. Add App ID to `FacebookManager.cs`
3. Configure Android/iOS platform settings
4. Enable required permissions (public_profile, user_friends)

**Features:**

- User authentication
- Friend list retrieval
- Avatar loading
- Score posting

### Advertisement Services

**Supported Networks:**

- Unity Ads
- AdMob
- Custom ad network integration

**Configuration:**

- Edit `AdsEvents.cs` for ad placement
- Set ad unit IDs for each platform
- Configure reward values

### Cloud Backends

**GameSparks Integration:**

- Location: `Assets/JellyGarden/Scripts/Integrations/Network/Gamesparks/`
- Features: Player data, leaderboards, achievements

**PlayFab Integration:**

- Location: `Assets/JellyGarden/Scripts/Integrations/Network/PlayFab/`
- Features: Player accounts, virtual economy, statistics

---

## 📖 Documentation

Comprehensive documentation is included in the project:

- **Main Documentation**: `Assets/JellyGarden/JellyGardenDocumentation1.6.pdf`
- **Online Guide**: `Assets/JellyGarden/JellyGarden online doc.pdf`

### Documentation Topics:

1. **Getting Started**

   - Project overview
   - Unity setup
   - Scene structure

2. **Level Design**

   - Using the Level Editor
   - Creating new levels
   - Level balancing tips

3. **Customization**

   - Changing visuals
   - Modifying gameplay parameters
   - Adding new item types

4. **Integration Guides**

   - Facebook setup
   - Ad network integration
   - Backend service configuration

5. **Building & Publishing**
   - iOS build process
   - Android build process
   - App store submission

---

## 💻 Requirements

### Unity Requirements

| Component         | Minimum    | Recommended |
| ----------------- | ---------- | ----------- |
| Unity Version     | 2019.4 LTS | 2020.3 LTS+ |
| .NET Version      | 4.x        | 4.x         |
| Scripting Backend | IL2CPP     | IL2CPP      |

### Platform Requirements

**iOS:**

- iOS 10.0+
- Xcode 12+
- CocoaPods (for dependencies)

**Android:**

- Android 4.4+ (API Level 19)
- Android SDK
- Gradle 6.1.1+

### Hardware Requirements (Development)

- **Processor**: Intel Core i5 / AMD Ryzen 5 or better
- **RAM**: 8GB minimum, 16GB recommended
- **Storage**: 10GB free space
- **Graphics**: DirectX 11/12 compatible GPU

---

## 🏗️ Build & Deployment

### Android Build

1. **Configure Player Settings**

   ```
   File → Build Settings → Android → Player Settings
   - Set Company Name
   - Set Product Name
   - Set Package Name (com.yourcompany.jellygarden)
   - Set Version and Bundle Version Code
   ```

2. **Configure Keystore**

   ```
   Publishing Settings
   - Create or select keystore
   - Enter keystore password
   - Select alias and password
   ```

3. **Build APK/AAB**
   ```
   File → Build Settings → Android
   - Select "Build App Bundle (Google Play)" or "Build APK"
   - Choose output location
   - Click Build
   ```

### iOS Build

1. **Configure Player Settings**

   ```
   File → Build Settings → iOS → Player Settings
   - Set Bundle Identifier
   - Set Version
   - Set Target SDK
   - Configure Signing
   ```

2. **Build Xcode Project**

   ```
   File → Build Settings → iOS
   - Click Build
   - Select output folder
   - Wait for Xcode project generation
   ```

3. **Open in Xcode**
   - Open generated .xcodeproj
   - Configure signing certificates
   - Build and archive for App Store

### Optimization Tips

- **Reduce Build Size**:

  - Enable code stripping
  - Use asset compression
  - Remove unused resources

- **Performance**:
  - Enable GPU instancing
  - Use texture atlases
  - Optimize particle effects
  - Profile with Unity Profiler

---

## 🤝 Contributing

Contributions are welcome! Please follow these guidelines:

### Development Workflow

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Make your changes**

   - Follow C# coding conventions
   - Add comments for complex logic
   - Update documentation if needed

4. **Commit your changes**

   ```bash
   git commit -m "Add amazing feature"
   ```

5. **Push to your branch**

   ```bash
   git push origin feature/amazing-feature
   ```

6. **Open a Pull Request**

### Code Standards

- Follow [Microsoft C# Coding Conventions](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/inside-a-program/coding-conventions)
- Use meaningful variable and method names
- Add XML documentation comments for public APIs
- Keep methods focused and under 50 lines when possible

### Testing

- Test on both iOS and Android before submitting PR
- Ensure no regression in existing features
- Test with different screen resolutions

---

## 💬 Support

### Getting Help

- **Documentation**: Check the PDF guides in `Assets/JellyGarden/`
- **Issues**: Open an issue on GitHub with detailed description
- **Email**: support@yourcompany.com

### Reporting Bugs

When reporting bugs, please include:

- Unity version
- Platform (iOS/Android/Editor)
- Steps to reproduce
- Expected vs actual behavior
- Screenshots/logs if applicable

### Feature Requests

We welcome feature suggestions! Please:

- Check existing issues first
- Provide clear use case
- Describe expected behavior
- Consider implementation complexity

---

## 📄 License

This project is proprietary software. All rights reserved.

**Usage Terms:**

- Educational and personal use allowed
- Commercial use requires license
- Redistribution prohibited without permission
- No warranty provided

For licensing inquiries, contact: license@yourcompany.com

---

## 🎯 Roadmap

### Upcoming Features

- [ ] New game modes (Time Attack, Puzzle Mode)
- [ ] Additional special items
- [ ] Seasonal events system
- [ ] Guild/Team system
- [ ] Chat functionality
- [ ] Live Ops dashboard

### Version History

- **v1.6** (Current)

  - Enhanced level editor
  - Improved performance
  - Bug fixes and stability

- **v1.5**

  - Added PlayFab integration
  - New booster types
  - UI improvements

- **v1.0**
  - Initial release
  - 100 levels
  - Basic social features

---

## 🌟 Credits

### Development Team

- **Lead Developer**: [Your Name]
- **Game Design**: [Designer Name]
- **Art & Animation**: [Artist Name]
- **Sound Design**: [Sound Designer]

### Third-Party Assets

- **UI Framework**: Unity UI
- **Particle Effects**: Custom effects
- **Audio**: Licensed music and SFX
- **Fonts**: Boris Black Bloxx, Candy Script

### Special Thanks

Thanks to all contributors and the Unity community for support and feedback!

---

## 📞 Contact

**Project Maintainer**: [Your Name]

- GitHub: [@NewbieAudioKid](https://github.com/NewbieAudioKid)
- Email: contact@yourcompany.com
- Website: [yourcompany.com](https://yourcompany.com)
- Twitter: [@yourhandle](https://twitter.com/yourhandle)

---

<div align="center">

**Made with ❤️ using Unity**

[⬆ Back to Top](#-jelly-garden-match-3-game)

</div>
