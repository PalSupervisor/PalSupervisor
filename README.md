# 🎮 PalSupervisor — Palworld Dedicated Server Manager 
<br><br>
# [PalSupervisor Website Here](https://palsupervisor.github.io/PalSupervisor/)
<br><br>
<img width="1500" height="659" alt="image" src="https://github.com/user-attachments/assets/bc608d91-6d3f-40bd-a5b3-bf3eab239644" />
<br><br>
A full-featured, web-based command center for managing Palworld dedicated servers. Built for server owners who want a clean, modern UI and pro-grade tools — without ever touching the command line after initial setup.
From real-time monitoring and surgical player moderation to automated anti-cheat, scheduled backups, and full Nexus Mods integration — PalSupervisor is the only panel you'll ever need.
<br>
[Join Our Discord for free/paid/trial keys HERE](https://discord.gg/VsctnXnKRk)

## ✨ Features

### 🖥️ Server Control
```
- Start, stop, restart, and graceful-shutdown the server from the UI
- Live server status with FPS, frame time, and uptime
- World save on demand
- Broadcast messages and priority alerts to all online players
- Scheduled restarts with configurable interval and custom warning messages ({minutes} placeholder)
- Auto-restart on crash with configurable crash-check interval
- Optional backup-before-restart safety net
```
### 📊 Live Dashboard
```
- Color-coded ring gauges for FPS, frame time, player count, uptime, base camps, in-game days
- CPU, memory, and disk usage bars with health thresholds
- One-click Start · Stop · Restart · Save World · Broadcast
- Online players list with level badges, auto-refreshed every 5 seconds
- API health panel (RCON / PST / Game REST status)
```
### 👥 Player Management
```
- View all online and historical players across all platforms
- Supports Steam, Xbox (GDK/EOS), 32-char hex UIDs, and raw XUIDs (auto-detected)
- Deep inspector: full inventory (every container), owned Pals with IVs/passives/location,
  tech points, Paldeck progress
- Built-in XP-to-level table (up to Lv. 65) — grant XP or set level directly
- Delete individual items or Pals straight from the inspector
- Targeted resets: inventory, Pals, stats, or techs — or reset everything at once
- Rename players from the panel
- Activity log per player
- Kick, ban, unban — one-click moderation
- Full ban list management
- Global item search — find who's carrying what across the server, including guild chests
- Give Items (any ID, any count) and Give Pals (with stats, passives, level, IVs)
- Kit Manager — build/edit starter & custom kits, give any kit to any player in one click
- Starter Kit system — auto-gift new players, with claim tracking and one-click reset
- PalDefender Templates — save named Pal loadouts and gift them to players
```

### 🗺️ Live Map
```
- Real-time positions of players and guild bases
- Loot browser with category filtering
- Teleport any player anywhere on the map
- Teleport yourself to a player, or summon a player to you
- Per-user map display settings (toggle layers individually)
```

### 🏰 Guild Management
```
- Browse every guild on the server
- View members, levels, and bases
- Per-base module breakdown: Energy, Medical, Transport, Passive Effects,
  Gathering, Storage, Workstations, Maintenance
- Live work-task summary per base (building, repair, healing, gathering,
  crafting, farming, defense)
- Real-time raid status with cooldown percentage
- Research/lab tab: current research, total recipes, in-progress count
- Drill into base chests and base Pals (with vitals: HP, sanity, hunger, condition)
- Destroy bases, promote members to guild leader, rename guilds
- Full guild oversight for moderators
```

### 🗓️ Event Scripting Engine
```
- Active / Scheduled / Recurring / History event tabs
- Action types per event: apply config preset, toggle mods, restart server,
  give item, give stat points, give kit, spawn Pal, raid (multi-spawn),
  and steal item (randomly takes from one online player, gifts another)
- Recipients: all online, or random N online, with "don't repeat recipients"
- Mid-event firing control per action: at event start, at a random moment
  in a time window, or repeated on an interval
- Optional "on end" cleanup: revert config, revert mods, restart after
  revert — with its own countdown-warning message
- Save any event as a reusable template
```

### 🛡️ Anti-Cheat
```
- Scheduled automatic scans with configurable cadence
- On-demand manual scans
- Live results + full detection history
- Fine-grained level-gap thresholds (Lv 1–5) for cheat severity
- Kick, ban, reset cheaters, wipe Pals, or delete specific illegal items/Pals
- Resolve flags once reviewed
- Per-flag moderation log
```

### 🔧 Mod Manager
```
- Upload mods with name, version, author, description metadata
- Scan existing mod folders
- Enable / Disable / Toggle mods individually or in bulk
- Drag-style load order editor
- Per-mod config editor
- Dependency validation and update checks
- Profile export/import (share setups across servers)
- Custom mods directory override
```
### 🌐 Nexus Mods Integration
```
- Connect via Nexus API key
- Browse Trending, Latest, and Recently Updated mods
- Search the full Nexus catalog
- View mod details, file lists, and changelogs in-app
- One-click install directly to your server
```
### 💬 Discord Bot Integration
```
- Built-in Discord bot — enable/disable and monitor live status from the panel
- Per-Discord-role permission mapping
- Bot activity status and server-members intent toggle
- Quick setup guide built into the UI
- Snowflake-safe ID handling (no JS float-precision corruption on Discord IDs)
```

### 💾 Backup System
```
- On-demand and scheduled world snapshots
- Configurable interval, max retained, and custom backup folder
- Optional backup-before-restart safety net
- One-click restore of any snapshot
- Restore server config from backup
- List, browse, and delete backups
```

### 📊 Monitoring & Logs
```
- Real-time server stats with historical charts (configurable retention)
- Live alert feed with clear-all support
- Filterable log viewer
- API health/status dashboard (RCON, PST, Game REST)
- Crash detection and reporting
```

### ⌨️ Console
```
- Send raw RCON commands directly from the browser
- Scrollable command history
- Old-school RCON power, modern UX
```

### ⚙️ Configuration
```
- Visual editor for PalWorldSettings / config.yaml
- YAML editor with full, structured, and raw modes
- Apply community presets in one click
- Import / export full config (JSON)
- Path validation
- Test connections (RCON, Game REST, PST) with one click
- Config backup restore — recover from broken edits
```

### 🔐 User & Permission System
```
- Multi-user support with full user management (create, edit, delete, reset password)
- 6-tier role hierarchy: visitor → member → moderator → admin → super_admin → owner
- Fine-grained permissions per page, per tab, per action
  (e.g., players.ban, mods.tab.nexus, dashboard.ui.broadcast)
- Permission-aware sidebar and routes (users only see what they can use)
- JWT auth with auto-logout on expiry
- 30-second permission refresh
- Forced password change on first login
```
### 🎨 Themes & Polish
```
- Multiple curated themes (colors, fonts, animations)
- Customizable card styles, border glow, spacing, shadows, sidebar styles
- Animated particle backgrounds
- Toast notifications
- Fully responsive layout with mobile-friendly sidebar
- Built-in license panel with activation + version info
```
### 🛠️ Advanced Settings (10 Tabs)
```
- Connections — RCON, PST, Game REST with live Test Connection buttons
- Auto-Detect — parses PalWorldSettings.ini + config.yaml and auto-fills
  ports, passwords, addresses, and admin info (with review modal)
- Server — exe path with native file browser, path verification,
  launch args, crash-check interval, auto-restart on crash
- Admin — personal Steam ID for teleport-to-me features
- Backups — automated snapshot rules
- Scheduled Restarts — interval + custom warning message
- Anti-Cheat — thresholds and scan cadence
- Whitelist — add/remove Steam IDs, global enable toggle
- Map Display — fine-tune what appears on the live map
- Discord Bot — role permissions, activity status, quick setup guide
- Themes — full UI customization
- Dashboard Port Manager + Restart App (with auto-reconnect)
- Full Config Export / Import (JSON)
```
## 🚀 Getting Started

### Prerequisites
```
- A running **Palworld dedicated server**
- RCON enabled in `PalWorldSettings.ini` (`RCONEnabled=True`)
- Game REST API enabled (`RESTAPIEnabled=True`)
- PalDefender installed on the server
```

### Installation

[Download latest version from Releases Here](https://github.com/PalSupervisor/PalSupervisor/releases)
```
1. Extract the .rar file
2. Run PalSupervisor.exe
3. The dashboard will open automatically at http://localhost:3000
```
## 🧙 First-Time Setup Wizard
```
On first launch, you'll be guided through a 5-step setup wizard:

Step 1 — Server Location
- Point the panel at your PalServer.exe
- The wizard auto-detects your server executable and save folder
  by scanning common install paths
- Save path is derived automatically from the exe location
- Native file picker available for manual selection

Step 2 — RCON & REST API
- Enter your RCON address, port, and password
- Enter your Game REST API address, port, and password
- Both passwords typically match AdminPassword in PalWorldSettings.ini
- Optional: enable Base64 encoding for RCON if your server requires it

Step 3 — PST Auth
- Configure address, port, username, and password for your PST API
- Credentials automatically synced to config.yaml → auth
- Optionally enter your Steam ID to enable teleport-to-admin features

Step 4 — Memory Management
- Configure memory flush interval (default: 15 min)
- Check interval (default: 30s)
- Threshold (default: 1024 MB)
- Defaults work well for most setups

Step 5 — Complete
- Review your settings summary
- Click Finish Setup to write both config.json and config.yaml
- All settings can be changed later in the Settings page

```
## 🔌 Connection Types

```
| Connection      | Purpose                                          | Default Port |
|-----------------|--------------------------------------------------|--------------|
| RCON            | Player kicks, bans, broadcasts, teleports        | 25575        |
| Game REST API   | Server info, metrics, player list                | 8212         |
| PST API         | Save file inspection, player editing             | 8080         |
```

## 👤 User Roles

```
| Role          | Level | Description                                |
|---------------|-------|--------------------------------------------|
| visitor       | 1     | Read-only access                           |
| member        | 2     | Basic dashboard access                     |
| moderator     | 3     | Player moderation tools                    |
| admin         | 4     | Server management                          |
| super_admin   | 5     | Full server management                     |
| owner         | 6     | Unrestricted access                        |
```
## 🌍 Multi-Language Support
```
- Full UI translation across 10 languages
- Switch language instantly from the Settings page — no restart required
- Per-user language preference (each account remembers its own setting)
- RTL (right-to-left) layout support for Arabic
- Localized dates, numbers, and notifications

Supported languages:
- 🇬🇧 English
- 🇪🇸 Spanish    (Español)
- 🇯🇵 Japanese   (日本語)
- 🇸🇦 Arabic     (العربية)
- 🇫🇷 French     (Français)
- 🇷🇺 Russian    (Русский)
- 🇩🇪 German     (Deutsch)
- 🇹🇷 Turkish    (Türkçe)
- 🇨🇳 Chinese    (中文)
- 🇻🇳 Vietnamese (Tiếng Việt)
```
## 📁 Config Files
```
After setup, two config files are written:

- config.json — panel settings (RCON, REST, paths, backup, anti-cheat, etc.)
- config.yaml — PST / YAML auth and memory management settings

Both can be edited in the Settings page, or exported/imported as JSON.
```
## 🏆 Why PalSupervisor?
```
🎮 Stop babysitting your server. Start commanding it.
PalSupervisor — run Palworld like a pro.
- One dashboard — total control over your entire Palworld operation
- Zero command-line work after setup
- Built for solo operators AND multi-staff communities
- Permission-aware UI keeps your team focused on what they can actually do
- Automated anti-cheat keeps your world fair
- Scheduled backups keep your world safe
- Native mod + Nexus integration keeps your world fresh
```
## 📜 License
```
For free, trial, and paid keys — plus full community support, updates, and feedback:
Join https://discord.gg/VsctnXnKRk
```
# Admin View
<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/98267ef2-86fb-4d27-b1ee-0e7da77020f2" />
<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/00d023a1-d75c-4d7d-b04e-783af847887d" />
<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/7834660f-9ba2-49ad-b785-80828a2e3f92" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/684e8d13-e935-4dc5-b5c1-351c686714f0" />

<br><br>
<img width="1570" height="1079" alt="image" src="https://github.com/user-attachments/assets/96643511-1e54-4c44-a532-3e957ab969e0" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/6c891c66-d753-4ebc-bfd7-57aeee420a05" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/ea0975cf-6722-47ad-b33c-9a98f4d52613" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/d9fb1ab5-7f17-4421-97ba-e6dc7743b59b" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/20de41a5-a3f5-4217-9d84-74aff8860594" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/5ce3e37b-99d7-46eb-8815-b6a0a44e13a2" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/c9ba1ee5-60bf-4091-82a4-d0ae957c03b5" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/b1d22099-dade-4ad6-92e2-f904fc41a324" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/a6db48fb-604b-45ff-be9b-c90a7746b5d1" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/064d29da-debe-4980-835f-f9638c4ba6f1" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/e7f9c0e6-f8b7-483d-9c3d-274a4f196aae" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/315e7d48-f5a2-4fc6-b451-60c7b0992f5d" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/8c3b815c-1ebb-4bb2-8c76-e7536a205b2e" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/b8bab674-21e1-4869-945d-214c543c2009" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/5d652800-3a16-4f4a-bace-b1bb2a967ba2" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/d338b069-1fbc-488f-abd6-d1c79eec5634" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/8b70c5ec-6ed5-47bc-9174-7a83090773d9" />
<br><br>
<br><br>


# Guest View 
<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/e6615cba-f05e-439b-9e52-316fae6eb8bd" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/0022dc63-dc3a-4369-83ed-3b8255e08e55" />

<br><br>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/7f212bc8-a1d9-46fb-9a5d-d339ba546406" />




