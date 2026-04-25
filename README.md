# 🎮 PalSupervisor — Palworld Dedicated Server Manager

A full-featured web-based control panel for managing Palworld dedicated servers. Built for server owners who want a clean UI and powerful tools without touching the command line after initial setup.
<br>
[Join Our Discord for free/paid/trial keys HERE](https://discord.gg/VsctnXnKRk)

## ✨ Features

### 🖥️ Server Control
```
- Start, stop, restart, and graceful-shutdown the server from the UI
- Live server status and performance metrics
- World save on demand
- Broadcast messages to all online players
- Scheduled restarts with configurable intervals
```

### 👥 Player Management
```
- View all online and historical players (Steam, Xbox/GDK, EOS/Epic platforms supported)
- Inspect detailed player info and activity logs
- Kick, ban, and unban players
- Manage the ban list
- Give items and Pals to players
```

### 🗺️ Live Map
```
- See player positions on a live map
- View guild territories
- Teleport players to any location
- Teleport yourself to a player, or pull a player to you
```

### 🏰 Guild Management
```
- List all guilds and view detailed guild info
```

### 🛡️ Anti-Cheat
```
- Automatic and on-demand scan for cheating players
- Review flagged players with full history
- Kick, ban, reset, or wipe the inventory/Pals of flagged players
- Resolve flags individually
```

### 🔧 Mod Manager
```
- Browse, install, enable/disable, and uninstall mods
- Manage mod load order
- Validate mod dependency chains
- Import/export mod profiles
- **Nexus Mods integration** — browse trending, latest, and updated mods; search; install directly from Nexus with API key
```

### 💾 Backup System
```
- Create, restore, list, and delete world backups
- Automated backup scheduling
- Restore config from backup
```

### 📊 Monitoring & Logs
```
- Real-time server stats with history graphs
- Alert system with clear-all support
- Live server logs with filtering
- API health/status dashboard
```

### ⌨️ Console
```
- Send RCON commands directly from the browser
- Command history
```

### ⚙️ Configuration
```
- Visual editor for game config (PalWorldSettings)
- YAML config editor (full, structured, and raw modes)
- Apply community presets
- Import/export full config
- Validate paths, test connections (RCON, REST API, PST)
```

### 🔐 User & Permission System
```
- Multi-user support with role-based access control
- Roles: `visitor`, `moderator`, `admin`, `super_admin`, `owner`
- Granular per-user permissions
- Password management and admin user reset
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

```
[Download latest version from Releases Here](https://github.com/PalSupervisor/PalSupervisor/releases)
extract the rar and start PalSupervisor.exe
a default webpage should open at http://localhost:3000

```
## 🧙 First-Time Setup Wizard
```
On first launch, you'll be guided through a 5-step setup wizard:

**Step 1 — Server Location**
- Point the panel at your `PalServer.exe`
- The wizard will **auto-detect** your server executable and save folder by scanning common install paths
- Save path is derived automatically from the exe location

**Step 2 — RCON & REST API**
- Enter your RCON address, port, and password
- Enter your Game REST API address, port, and password
- Both passwords are typically the same as `AdminPassword` in `PalWorldSettings.ini`
- Optional: enable Base64 encoding for RCON if your server requires it

**Step 3 — PST Auth**
- Configure the address, port, username, and password for your PST API
- These credentials are automatically synced to `config.yaml → auth`
- Optionally enter your Steam ID to enable teleport-to-admin features

**Step 4 — Memory Management**
- Configure memory flush interval (default: 15 min), check interval (default: 30s), and threshold (default: 1024 MB)
- Defaults work well for most setups

**Step 5 — Complete**
- Review your settings summary
- Click **Finish Setup** to write both `config.json` and `config.yaml`
- All settings can be changed later in the Settings page

```
## 🔌 Connection Types

```
| Connection | Purpose | Default Port |
|---|---|---|
| RCON | Player kicks, bans, broadcasts, teleports | 25575 |
| Game REST API | Server info, metrics, player list | 8212 |
| PST API | Save file inspection, player editing | 8080 |
```

## 👤 User Roles

```
| Role | Level | Description |
|---|---|---|
| `visitor` | 1 | Read-only access |
| `moderator` | 2 | Player moderation |
| `admin` | 3 | server management |
| `super_admin` | 4 | Full server management |
| `owner` | 5 | Unrestricted access |
```

## 🎮 Platform Support

```
Player IDs from all Palworld platforms are handled automatically:

- **Steam** — 17-digit SteamID64 (`7656...`)
- **Xbox / GDK** — `gdk_` prefixed XUID
- **Epic / EOS** — 8-8-8-8 hex GUID
- **Raw XUID** — 16-digit numeric ID
```

## 📁 Config Files
```
After setup, two config files are written:

- `config.json` — panel settings (RCON, REST, paths, backup, anticheat, etc.)
- `config.yaml` — PST/YAML auth and memory management settings

Both can be edited in the **Settings** page, or exported/imported for backup.
```

## 📜 License

Join https://discord.gg/VsctnXnKRk

# Admin View
<br><br>
<img width="1875" height="920" alt="image" src="https://github.com/user-attachments/assets/1b696c31-0da8-42c2-9114-5d1677acb052" />
<br><br>
<img width="1876" height="916" alt="image" src="https://github.com/user-attachments/assets/45da7561-8c1c-4219-8cb3-9124f139f654" />
<br><br>
<img width="1875" height="919" alt="image" src="https://github.com/user-attachments/assets/50fa1b25-8cf5-4527-9256-063deb401d24" />
<br><br>
<img width="1876" height="919" alt="image" src="https://github.com/user-attachments/assets/a78bbe38-0cc0-4987-ba18-af199decd76d" />
<br><br>
<img width="1875" height="923" alt="image" src="https://github.com/user-attachments/assets/955e8f1a-dee1-440f-adf6-d081a57ec7ac" />
<br><br>
<img width="1876" height="918" alt="image" src="https://github.com/user-attachments/assets/a5bc39f5-6deb-4981-9412-129116cf3ca5" />
<br><br>
<img width="1875" height="918" alt="image" src="https://github.com/user-attachments/assets/6acd42f9-540b-4773-9c32-8cff7f8412ad" />
<br><br>
<img width="1875" height="919" alt="image" src="https://github.com/user-attachments/assets/8ef124e6-17fb-486b-882e-8e80a0edc373" />
<br><br>
<img width="1877" height="930" alt="image" src="https://github.com/user-attachments/assets/a240b50f-9ae5-48e0-85ce-50aa63609d62" />
<br><br>
<img width="1875" height="925" alt="image" src="https://github.com/user-attachments/assets/5fd01c66-9dc8-4ba3-890d-497c5f0e78da" />
<br><br>
<img width="1875" height="916" alt="image" src="https://github.com/user-attachments/assets/65a4b3eb-977e-45af-8b8a-d92f3b6923df" />
<br><br>
<img width="1875" height="919" alt="image" src="https://github.com/user-attachments/assets/84835f35-543b-44d1-9052-bc2473368ac2" />
<br><br>
<img width="1876" height="915" alt="image" src="https://github.com/user-attachments/assets/2126b26b-d139-45ff-a01b-9b83e1e32917" />
<br><br>
<img width="1876" height="921" alt="image" src="https://github.com/user-attachments/assets/22bd5c2d-8bca-4857-b94e-f1b8c733aae6" />
<br><br>
<img width="1875" height="915" alt="image" src="https://github.com/user-attachments/assets/e86ee22b-420e-4e7c-8247-5a2d842cccfe" />
<br><br>
<img width="1875" height="920" alt="image" src="https://github.com/user-attachments/assets/2996af98-cf52-4eed-b9ef-b86a92838456" />
<br><br>
<img width="1877" height="919" alt="image" src="https://github.com/user-attachments/assets/1090952c-7c7e-4521-808b-c721edcbb1a7" />
<br><br>
<img width="1876" height="924" alt="image" src="https://github.com/user-attachments/assets/06d5daa9-27f4-420b-8bd8-cfeb4c48261a" />
<br><br>
<img width="1875" height="921" alt="image" src="https://github.com/user-attachments/assets/b26fd7cc-4645-457c-a497-e7aaad2a7fb5" />
<br><br>
<img width="1876" height="919" alt="image" src="https://github.com/user-attachments/assets/3fdb759f-4cd6-481c-b470-2c6bf60c78ef" />
<br><br>
<img width="1877" height="918" alt="image" src="https://github.com/user-attachments/assets/5c3c814f-623b-4f53-a747-e35ed3a4dfb1" />
<br><br>
<img width="1877" height="921" alt="image" src="https://github.com/user-attachments/assets/be58157f-6b06-4e28-9062-d8eece67db95" />


# Guest View 
<br><br>
<img width="1876" height="918" alt="image" src="https://github.com/user-attachments/assets/df9c7cb5-053f-4895-9e16-7ac90fa56ea3" />
<br><br>
<img width="1875" height="916" alt="image" src="https://github.com/user-attachments/assets/2c9eb27b-9fd9-4464-a5a2-93296635f14d" />
<br><br>
<img width="1877" height="920" alt="image" src="https://github.com/user-attachments/assets/4ba2b9d8-a998-461e-8e81-764c8c493f37" />



