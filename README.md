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

- Two-language UI (`English`, `Русский`) - switch on the fly from Settings
- Custom key bindings for the menu, panic key, noclip controls and quick-teleport hotkeys
- Panic key instantly hides every overlay (menu + ESP + watermark)
- Clean cheat unload from inside the menu

---

### ESP

| Feature | Description |
|---|---|
| **Per-category toggles** | Independent on/off for monsters, players, NPCs, harvest items, treasure chests, drop boxes, oracle stones, bank items, pickup items |
| **Per-category colors** | Each category has its own color picker |
| **Max Distance** | Slider in meters; targets beyond range are hidden |
| **Box Style** | Full Box, Cornered, or Filled |
| **Box Thickness / Corner Size** | Tune line thickness and corner length |
| **Distance text** | Shows distance in meters next to each target |
| **Snapline** | Line from screen anchor to target (toggle + thickness) |
| **Off-Screen Arrows** | Pointers to targets outside the viewport with cone FOV and ring radius sliders |

---

### Combat

| Feature | Description |
|---|---|
| **Crit Force** | Every outgoing hit lands as a critical |
| **Multi-Shot** | Soon... |
| **Multi-Hit** | Replays the last damage effect N times per swing |
| **Multi-Hit Hits/Swing** | Slider for how many times the hit is replayed |

---

### Movement

| Feature | Description |
|---|---|
| **Speed Hack** | Increases the player's movement speed |
| **Speed Multiplier** | 1.0x to 10.0x slider |
| **Jump Hack** | Increases jump height |
| **Jump Multiplier** | 1.0x to 10.0x slider |
| **Infinite Jumps** | Jump in mid-air any number of times |
| **Noclip** | Fly through walls and terrain |
| **Noclip Speed** | Movement speed while in noclip (m/s) |
| **Noclip Controls** | Rebindable Forward / Back / Left / Right / Up / Down / Sprint keys |
| **Time Dilation** | Speeds up or slows down the entire game world |
| **Time Dilation Speed** | 0.05x (bullet-time) to 5.0x (fast forward); Reset button returns to 1.0x |

---

### Player

| Feature | Description |
|---|---|
| **No Damage** | Blocks every source of incoming damage |
| **No Fall Damage** | 50/50 soon.. |
| **Auto Skip** | Skips cutscenes and dialog windows automatically (50/50 Works) |

---

### Teleports

| Feature | Description |
|---|---|
| **World Map Teleporter** | Master toggle for the saved-location system |
| **Categories** | Locations grouped per `.txt` file in `Teleports/` |
| **Category combo** | Live progress counter `(collected / total)` per category |
| **TP to Next Pending** | Jumps to the next un-collected entry of the current category |
| **Reset Category** | Clears the collected-state of the active category |
| **Auto-Mark Collected on TP** | Marks a location as collected the moment you teleport to it |
| **Hotkey: TP to Next** | Rebindable key that runs "TP to Next Pending" without opening the menu |
| **Hotkey: Back to Previous** | Rebindable key that returns to the previously visited entry |
| **New File** | Creates a new category file from the menu |
| **Add Current Position** | Saves your current world position into the active category |
| **Entries list** | Per-entry buttons: delete, double-click teleport, Mark / Unmark Selected |
| **Open Folder** | Opens `Teleports/` in Explorer |
| **Reload Files** | Re-reads every `.txt` from disk |
| **HUD** | Optional in-game HUD showing the current category and next pending entry |

---

### Vehicle

| Feature | Description |
|---|---|
| **No Damage** | The vehicle ignores all incoming damage |
| **Super Friction** | Keeps the vehicle glued to the ground; configurable multiplier |
| **Max Speed** | Removes the default top-speed cap; slider in km/h |
| **Acceleration** | Faster acceleration; configurable multiplier |
| **Noclip** | Drive through walls and ground; speed slider in m/s |
| **Phase Through Cars** | Switch collision skip: Off / Pawns only / Vehicles only / Pawns + Vehicles |
| **Better Handling (master)** | Enables a full physics tuning block below |
| **Cornering / Steer Speed / Max Steer Angle** | Tighten or loosen steering response |
| **Tire Grip / Side Slip / Lateral Slip / Body Snap / Chassis Mass** | Per-axis grip and chassis behaviour |
| **Lock Stability** | One-click no-slip + traction-control + no-drift profile |
| **All-Wheel Steering** | Enables 4WS |
| **Pitch Lock** | Prevents nose-dive |
| **Disable Auto-Brake** | Removes the game's auto-brake assist |
| **Brake / Handbrake Torque** | Slider for instant-stop power |
| **Handbrake-Jump Distance / Intensity** | Controls the handbrake-jump effect |
| **Reset to Sharp Preset / Reset to Stock** | Two presets for the handling tuning block |
| **Anti-Gravity** | Disables gravity on the vehicle |
| **Anti-Roll** | Prevents the vehicle from flipping |
| **Infinite Nitrous** | Nitro never runs out |

---

### Spawner

| Feature | Description |
|---|---|
| **Vehicle list** | Combo populated with every driveable vehicle class resolved from the game |
| **Spawn Vehicle** | Spawns the selected vehicle next to you |
| **Status feedback** | Shows last spawn result: Idle / Spawned OK / Class missing or no pawn / ProcessEvent failed |

---

### Visual

| Feature | Description |
|---|---|
| **FOV Override** | Set a custom field of view (slider, 60-130). Restores the game's original FOV on disable. |
| **Peeking** | Admire boobs up close ))) |
| **FPS Unlocker** | FPS Unlock lol |

---

### Automatic

| Feature | Description |
|---|---|
| **Auto Fishing** | Fully automated fishing - cast, wait, reel, repeat |
| **Show stats HUD** | Live counter for caught / failed / per-rarity hauls and the heaviest catch |
| **Reset stats** | Clears the stats counters |

---

### Settings

| Feature | Description |
|---|---|
| **Language** | Switch the menu between English and Russian on the fly |
| **Open Menu bind** | Choose any key to open / close the menu (default: Insert) |
| **Panic Key** | Press once to instantly hide every overlay (menu + ESP + watermark), press again to restore |
| **Name Changer** | Replace your displayed nickname; original is masked, with Show / Hide / Copy buttons |
| **UID Changer** | Replace your displayed UID; original is masked, with Show / Hide / Copy buttons |
| **Unload Cheat** | Cleanly detaches the cheat DLL from the game process without restarting |

---

## Support

Questions, updates, custom builds: **[discord.gg/RhQyjFDsr7](https://discord.gg/RhQyjFDsr7)**
