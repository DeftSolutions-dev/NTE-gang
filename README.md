# NTE Reversal Tools - Educational Game Hacking Project

**100% Educational & Research Purposes Only**  
Neverness To Everness (NTE) memory manipulation, reverse engineering and dynamic analysis demonstration.

![GitHub stars](https://img.shields.io/github/stars/DeftSolutions-dev/NTE-Cheats)
![GitHub license](https://img.shields.io/github/license/DeftSolutions-dev/NTE-Cheats)
![GitHub release](https://img.shields.io/github/v/release/DeftSolutions-dev/NTE-Cheats)

## LEGAL NOTICE & EDUCATIONAL DISCLAIMER

This repository is provided **strictly for educational, research and reverse engineering purposes**. It demonstrates advanced techniques of memory reading/writing, DLL injection, internal cheating methods, pattern scanning and game engine analysis.

**No copyrighted assets, proprietary code or binary files from NTE are included.**  
All code is original or based on public reverse engineering research.

This project complies with:
- [GitHub Acceptable Use Policies](https://docs.github.com/en/site-policy/acceptable-use-policies/github-acceptable-use-policies)
- [GitHub Active Malware or Exploits Policy](https://docs.github.com/en/site-policy/acceptable-use-policies/github-active-malware-or-exploits) - explicitly allows dual-use research tools
- U.S. Copyright Law - Fair Use Doctrine (17 U.S.C. § 107) for reverse engineering, education and security research
- DMCA § 1201 (research exemption)

Any use of this code in violation of the game's EULA is solely the responsibility of the end user. This repository itself does not violate any laws or GitHub rules.

**For learning and authorized testing only.**

---
<img width="1670" height="1164" alt="Screenshot_2" src="https://github.com/user-attachments/assets/13fedf2e-ea7d-4a56-8012-1b6f375cf5bc" />

---

## Author / Contact

Built by **DesirePro**.  
Discord: **[discord.gg/RhQyjFDsr7](https://discord.gg/RhQyjFDsr7)** - questions, builds, support.

---

## Requirements

- Windows 10 / 11 (x64)
- The official NTE launcher (`NTEGlobalGame.exe`) installed and able to start the game normally
- Administrator rights for the injector
- Add the project folder to your antivirus exclusion list - the DLL contains injection / hook code that AV heuristics flag

## Installation

1. Download the latest release.
2. Extract the archive anywhere. The folder must contain at minimum `launcher.exe` and `Cheat.dll` side by side.
3. Make sure the official NTE launcher (`NTEGlobalGame.exe`) is **closed** before you start.

## Usage

1. Run `launcher.exe` as administrator.
   - **First run only**: it will ask you to point it at `NTEGlobalGame.exe` once. The path is saved to `%APPDATA%\NTECheat\launcher.cfg`, so the next runs are fully automatic.
   - The injector restarts the official launcher with the right flags, patches the protection check, and injects `Cheat.dll` into the launcher process.
2. Click **Play** in the official NTE launcher as usual. The game starts with the cheat already in memory.
3. Once you are in-game, wait a few seconds, then press **Insert** to open the menu. The bind is changeable from Settings.

> If you see a Windows Defender warning, add the project folder to the exclusion list. If the official launcher refuses to start, run `launcher.exe` again - the cached path may be stale, delete `%APPDATA%\NTECheat\launcher.cfg` and try once more.

---

## Features

**144 features across 10 tabs.** Six-language UI (English, Русский, 中文, 日本語, Tiếng Việt, Indonesia), per-feature key bindings, panic key, and clean in-menu unload.

### ESP (29)

- Players, Monsters, NPCs, Items, Chests, Drops, Pickup Items, Oracle Stones, Bank Items, Box
- Per-category color picker
- Box Style, Box Thickness
- Show Distance, Max Distance, Distance Text
- Health Bar, Show Name, Show Level, Text Outline
- Snap Line, Snapline Thickness
- Off-screen Arrows, Off-screen FOV, Off-screen Radius
- Bank: PawPaw Only, Bank Containers, Bank Min Cost, Bank Min Coin

### Combat (12)

- Kill Aura, Kill Aura Range
- Multi Shot, Multi Shot Count
- Multi Hit, Multi Hit Count
- No Cooldown
- Crit Force
- Instant Kill
- No Damage
- Magnetizer, Magnetizer Range

### Movement (7)

- Speed Hack, Speed Mult
- Jump Hack, Jump Mult
- Infinite Jumps
- NoClip, NoClip Speed

### Player (8)

- Outfit Bypass
- Auto Skip Cutscenes
- Camera Peek
- No Crime
- Time Dilation, Time Scale
- Name Changer
- UID Changer

### Teleports (10)

- Marker File selector
- Create File
- Add Current Position
- Reload Files
- Marker list (click-to-teleport / delete)
- Next Marker hotkey
- Prev Marker hotkey
- Unstuck
- Map Transfer
- Show TP HUD

### Vehicle (39)

- Phase Through, Handling Tweaks, Drivetrain
- No Speed Limit, Max Speed, Speed km/h
- Super Vehicle, Drive on Water, Restore Water
- Anti-Gravity, Anti-Roll, Infinite Nitrous
- Super Friction, Friction Mult
- Vehicle NoClip, NoClip Speed
- Accel Boost, Accel Mult
- Cornering, Steer Speed, Steer Angle
- Grip, Mass, Side Slip, Body Snap, Lateral
- Brake Torque, Handbrake
- Jump Dist., Jump Power
- Lock Stability, Anti Flip, Jump Boost, ABS
- No Steer Curve, All-Wheel Steer, Constant Grip
- Pitch Lock, No Autobrake

### Spawner (3)

- Vehicle list
- Spawn Vehicle
- Status feedback

### Visual (4)

- FPS Unlocker
- FPS Cap
- Camera FOV Override
- FOV Value

### Automatic (13)

- Auto Fishing
- Auto Sell Fish
- Auto Buy Universal Bait
- Fish/Bait amount
- Fishing Logic
- Fishing HUD
- Auto Pickup, Pickup Range
- Auto TP Loot
- Auto Banking (heist)
- Banking Speed
- Min Coin
- Exit Bank Now

### Settings (19)

- Toggle Theme
- Language
- Particle Count
- Accent Color, Gradient Color
- Config Profiles (Load / Save / Delete / Save As New)
- Auto-save changes
- Auto-load on startup
- Diagnostics (render ms / FPS)
- Font Weight
- Bind List, Show TP HUD, Fishing HUD
- Reset Fish Stats
- Menu Key
- Panic Key
- Reset Config
- Unload Cheat
- Close Menu

---

## Support

Questions, updates, custom builds: **[discord.gg/RhQyjFDsr7](https://discord.gg/RhQyjFDsr7)**
