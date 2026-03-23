<div align="center">
<img width="120" height="120" alt="minecraft_title" src="https://github.com/user-attachments/assets/05bf63d1-f66d-4fbc-823b-27c14a25886f" />

# KaidonEssentials
</div>

> Modular essentials plugin for Minecraft servers — economy, teleportation, chat, homes, warps, administration and utilities in a single, clean and well-structured plugin.

---

## Overview

KaidonEssentials is an essentials plugin built with a focus on clean code, organization and performance. It covers the core needs of any server through dedicated, independent systems — all integrated with Vault and PlaceholderAPI out of the box.

---

## Compatibility


| Platform   | Supported              |
|------------|------------------------|
| Spigot     | 1.19.4+                |
| Paper      | 1.19.4, 1.20.4, 1.21.1 |
| Purpur     | 1.21.1                 |
| Pufferfish | 1.19.4+                |
| Folia      | 1.19.4+                |

> Minimum API version: **1.19**

---

## Requirements

- [Vault](https://www.spigotmc.org/resources/vault.34315/) *(Dependencies — required for economy features)*
- [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/) *(Dependencies — required for placeholders)*

---

## Installation

1. Download the latest `.jar` from [Releases](https://github.com)
2. Place the file in your server's `/plugins` folder
3. Restart the server
4. Configure the plugin in `plugins/KaidonEssentials/config.yml`

---

## Systems & Commands

### Economy
Vault-integrated currency management.


| Command | Usage | Permission | Default |
|---------|-------|------------|---------|
| `/money` | `/money [player]` | `kaidon.command.money` | Everyone |
| `/pay` | `/pay <player> <amount>` | `kaidon.command.pay` | Everyone |
| `/setarmoney` | `/setarmoney <player> <amount>` | `kaidon.admin.money.set` | OP |
| `/removermoney` | `/removermoney <player> <amount\|all>` | `kaidon.admin.money.remove` | OP |

---

### Warps
Interactive GUI for public teleport points.


| Command | Usage | Permission | Default |
|---------|-------|------------|---------|
| `/warps` | `/warps` | `kaidon.command.warps` | Everyone |
| `/kaidonwarp` | `/kaidonwarp` | `kaidon.admin.warps` | OP |

---

### Homes
Per-player personal teleport points.


| Command | Usage | Permission | Default |
|---------|-------|------------|---------|
| `/sethome` | `/sethome <name>` | `kaidonessentials.sethome` | Everyone |
| `/home` | `/home <name>` | `kaidonessentials.home` | Everyone |
| `/delhome` | `/delhome <name>` | `kaidonessentials.delhome` | Everyone |

---

### Teleport
TPA system with accept/deny and server spawn.


| Command | Usage | Permission | Default |
|---------|-------|------------|---------|
| `/tpa` | `/tpa <player>` | `kaidon.command.tpa` | Everyone |
| `/tpaccept` | `/tpaccept` | `kaidon.command.tpaccept` | Everyone |
| `/tpdeny` | `/tpdeny` | `kaidon.command.tpdeny` | Everyone |
| `/spawn` | `/spawn` | `kaidon.command.spawn` | Everyone |
| `/setspawn` | `/setspawn` | `kaidon.command.setspawn` | OP |

---

### Chat
Local and global chat with moderation tools.


| Command | Usage | Permission | Default |
|---------|-------|------------|---------|
| `/g` | `/g <message>` *(alias: /global)* | — | Everyone |
| `/mute` | `/mute <player>` | `kaidon.command.mute` | OP |
| `/unmute` | `/unmute <player>` | `kaidon.command.unmute` | OP |
| `/clearchat` | `/clearchat` | `kaidonessentials.clearchat` | OP |
| `/aviso` | `/aviso <message>` | `kaidon.command.aviso` | OP |

> **Chat Permissions**
> - `chat.spy` — See all local messages (OP)
> - `chat.color` — Use color codes with `&` (disabled by default)
> - `chat.bypass` — Bypass chat cooldown (OP)

---

### Administration
Moderation and inspection tools.


| Command | Usage | Permission | Default |
|---------|-------|------------|---------|
| `/freeze` | `/freeze <player>` | `kaidon.command.freeze` | OP |
| `/invsee` | `/invsee <player>` | `kaidon.command.invsee` | OP |
| `/speed` | `/speed <1-10>` | `kaidon.command.speed` | OP |
| `/speedreset` | `/speedreset` | `kaidon.command.speedreset` | OP |
| `/kireload` | `/kireload` | `kaidon.admin.reload` | OP |

> `kaidon.admin.commandbypass` — Bypass blocked commands defined in config (OP)

---

### Utilities
Quality of life commands for players.


| Command | Usage | Permission | Default |
|---------|-------|------------|---------|
| `/ec` | `/ec` | `kaidonessentials.ec` | Everyone |
| `/trash` | `/trash` | `kaidon.command.trash` | Everyone |
| `/luz` | `/luz` | `kaidon.command.luz` | Everyone |

---

## PlaceholderAPI


| Placeholder | Description |
|-------------|-------------|
| `%kaidon_balance%` | Player's current balance (formatted: K, M, B, T) |

---

## License

This project is proprietary software owned by **Kaidon Studios**. All rights reserved.

See the [LICENSE](LICENSE) file for detailed terms of use and restrictions.

---

## Links

- [Website](https://kaidonstudios.dev)
- [Discord](https://discord.gg/tVes26GfBk)
- [Modrinth](https://modrinth.com/plugin/kaidon-essentials)
- [CurseForge](https://www.curseforge.com/minecraft/bukkit-plugins/kaidon-essentials)

---

<sub>Founded by [Radu](https://github.com/Kaidon-Studios) · Kaidon Studios</sub>
