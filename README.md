Shadow Puzzle Game

A fun and engaging puzzle game built with Flutter where players match objects with their shadows. Drag, rotate, and match your way through challenging levels!

Game Overview

Shadow Puzzle is a matching puzzle game that challenges players to match colorful emoji objects with their corresponding shadows. The game features beautiful animations, smooth gameplay, and multiple game modes to keep players engaged.

Features

Game Modes
- Normal Mode: Progress through 3 increasingly challenging levels
  - Level 1: 5 objects, 60 seconds
  - Level 2: 8 objects, 90 seconds
  - Level 3: 10 objects, 120 seconds
- Endless Mode: Continuous gameplay where you try to achieve the highest score
  - Complete sets to earn bonus time (+15 seconds per set)
  - Track your high score
  - Challenge yourself to beat your best!

Gameplay Mechanics
- Drag & Drop: Move objects by dragging them across the screen
- Rotation: Double-tap objects to rotate them to match shadow orientation
- Matching: Match objects with their shadows by aligning position and rotation
- Time Challenge: Complete levels before time runs out

Categories
Choose from three emoji categories:
- Animals: Bears, elephants, frogs, octopuses, and more
- Food: Burgers, pizza, ice cream, donuts, and more
- Nature: Flowers, leaves, trees, sun, and more

Additional Features
- Achievement System: Unlock achievements as you play
  - First Match
  - Perfect Level (complete without mistakes)
  - All Levels (complete all 3 levels)
  - 10 Matches
  - Endless 100 (score 100+ in Endless mode)
- Customizable Backgrounds: Choose from 8 beautiful gradient themes
- Audio: Background music and sound effects (toggleable)
- Animations: Smooth Lottie animations for level start, game over, and more
- Progress Tracking: Save your high scores and achievements

Technology Stack

- Framework: Flutter (Dart)
- Dependencies:
  - `lottie: ^2.7.0` - For beautiful animations
  - `audioplayers: ^5.2.1` - For background music and sound effects
  - `shared_preferences: ^2.2.2` - For saving game settings and progress
- Platform Support: Android, iOS, Web, Windows, Linux, macOS

Installation

Prerequisites
- Flutter SDK (>=3.0.0)
- Dart SDK
- Android Studio / Xcode (for mobile development)
- VS Code or Android Studio (recommended IDEs)

Setup Steps

1. Clone the repository
   ```bash
   git clone https://github.com/yourusername/shadow_puzzle.git
   cd shadow_puzzle
   ```

2. Install dependencies
   ```bash
   flutter pub get
   ```

3. Run the app
   ```bash
   flutter run
   ```

Building for Specific Platforms

- Android: `flutter build apk` or `flutter build appbundle`
- iOS: `flutter build ios`
- Web: `flutter build web`
- Windows: `flutter build windows`
- Linux: `flutter build linux`
- macOS: `flutter build macos`

How to Play

1. Start the Game: Launch the app and wait for the splash screen
2. Select Categories: Choose one or more categories (animal, food, nature)
3. Choose Mode: Select Normal Mode or Endless Mode
4. Match Objects:
   - Drag objects from the top to their matching shadows below
   - Double-tap objects to rotate them if needed
   - Match both position and rotation to complete a match
5. Complete Levels: In Normal Mode, complete all matches before time runs out to advance
6. Track Progress: View your achievements and high scores

Project Structure

```
lib/
├── main.dart                 # App entry point
├── models/
│   ├── achievement.dart     # Achievement model and service
│   ├── game_item.dart       # Game item model
│   └── settings.dart        # Settings management
├── screens/
│   ├── splash_screen.dart   # Splash screen with animation
│   ├── home_screen.dart     # Main menu and category selection
│   ├── game_screen.dart     # Main game screen
│   └── achievements_screen.dart # Achievements display
└── services/
    └── level_generator.dart # Game item data and level generation

assets/
├── animations/              # Lottie animation files
├── emojis/                  # Game emoji assets (animal, food, nature)
└── sounds/                  # Audio files (music and effects)
```

Customization

Adding New Categories
1. Add emoji images to `assets/emojis/[category_name]/`
2. Create shadow versions of each emoji
3. Add entries to `emojiData` in `lib/services/level_generator.dart`

Adding New Backgrounds
Edit the `availableBackgrounds` list in `lib/screens/home_screen.dart` to add new gradient themes.

Adjusting Difficulty
Modify level parameters in `lib/screens/game_screen.dart`:
- `objectCount`: Number of objects per level
- `timeLeft`: Time limit per level
- `tolerance`: Matching distance tolerance

Development Team

- Ahmet Boray İncesoy
- Melis Eken
- Umut Berke Şenyayla
- Burak Gökmen Çelik
- Özge Küçükbayram

Resources

- Emojis: [emojiisland.com](https://emojiisland.com)
- Animations: Lottie Files
- Sound Effects: Custom

License

This project is available for educational purposes.

Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

Contact

For questions or suggestions, please open an issue on GitHub.

---

Enjoy playing Shadow Puzzle!
