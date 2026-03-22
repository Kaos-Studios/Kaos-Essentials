
<img width="512" height="512" alt="minecraft_title" src="https://github.com/user-attachments/assets/05bf63d1-f66d-4fbc-823b-27c14a25886f" />

# KaosEssentials

> Modular essentials plugin for Minecraft servers — economy, teleportation, chat, homes, warps, administration and utilities in a single, clean and well-structured plugin.

---

## Overview

KaosEssentials is an essentials plugin built with a focus on clean code, organization and performance. It covers the core needs of any server through dedicated, independent systems — all integrated with Vault and PlaceholderAPI out of the box.

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

- [Vault](https://www.spigotmc.org/resources/vault.34315/) *(optional — required for economy features)*
- [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/) *(optional — required for placeholders)*

---

## Installation

1. Download the latest `.jar` from [Releases](https://github.com/Kaos-Studios/KaosEssentials/releases)
2. Place the file in your server's `/plugins` folder
3. Restart the server
4. Configure the plugin in `plugins/KaosEssentials/config.yml`

---

## Systems & Commands

### Economy
Vault-integrated currency management.

| Command | Usage | Permission | Default |
|---------|-------|------------|---------|
| `/money` | `/money [player]` | `kaos.command.money` | Everyone |
| `/pay` | `/pay <player> <amount>` | `kaos.command.pay` | Everyone |
| `/setarmoney` | `/setarmoney <player> <amount>` | `kaos.admin.money.set` | OP |
| `/removermoney` | `/removermoney <player> <amount\|all>` | `kaos.admin.money.remove` | OP |

---

### Warps
Interactive GUI for public teleport points.

| Command | Usage | Permission | Default |
|---------|-------|------------|---------|
| `/warps` | `/warps` | `kaos.command.warps` | Everyone |
| `/kaoswarp` | `/kaoswarp` | `kaos.admin.warps` | OP |

---

### Homes
Per-player personal teleport points.

| Command | Usage | Permission | Default |
|---------|-------|------------|---------|
| `/sethome` | `/sethome <name>` | `kaosessentials.sethome` | Everyone |
| `/home` | `/home <name>` | `kaosessentials.home` | Everyone |
| `/delhome` | `/delhome <name>` | `kaosessentials.delhome` | Everyone |

---

### Teleport
TPA system with accept/deny and server spawn.

| Command | Usage | Permission | Default |
|---------|-------|------------|---------|
| `/tpa` | `/tpa <player>` | `kaos.command.tpa` | Everyone |
| `/tpaccept` | `/tpaccept` | `kaos.command.tpaccept` | Everyone |
| `/tpdeny` | `/tpdeny` | `kaos.command.tpdeny` | Everyone |
| `/spawn` | `/spawn` | `kaos.command.spawn` | Everyone |
| `/setspawn` | `/setspawn` | `kaos.command.setspawn` | OP |

---

### Chat
Local and global chat with moderation tools.

| Command | Usage | Permission | Default |
|---------|-------|------------|---------|
| `/g` | `/g <message>` *(alias: /global)* | — | Everyone |
| `/mute` | `/mute <player>` | `kaos.command.mute` | OP |
| `/unmute` | `/unmute <player>` | `kaos.command.unmute` | OP |
| `/clearchat` | `/clearchat` | `kaosessentials.clearchat` | OP |
| `/aviso` | `/aviso <message>` | `kaos.command.aviso` | OP |

> **Chat Permissions**
> - `chat.spy` — See all local messages (OP)
> - `chat.color` — Use color codes with `&` (disabled by default)
> - `chat.bypass` — Bypass chat cooldown (OP)

---

### Administration
Moderation and inspection tools.

| Command | Usage | Permission | Default |
|---------|-------|------------|---------|
| `/freeze` | `/freeze <player>` | `kaos.command.freeze` | OP |
| `/invsee` | `/invsee <player>` | `kaos.command.invsee` | OP |
| `/speed` | `/speed <1-10>` | `kaos.command.speed` | OP |
| `/speedreset` | `/speedreset` | `kaos.command.speedreset` | OP |
| `/kreload` | `/kreload` | `kaos.admin.reload` | OP |

> `kaos.admin.commandbypass` — Bypass blocked commands defined in config (OP)

---

### Utilities
Quality of life commands for players.

| Command | Usage | Permission | Default |
|---------|-------|------------|---------|
| `/ec` | `/ec` | `kaosessentials.ec` | Everyone |
| `/trash` | `/trash` | `kaos.command.trash` | Everyone |
| `/luz` | `/luz` | `kaos.command.luz` | Everyone |

---

## PlaceholderAPI

| Placeholder | Description |
|-------------|-------------|
| `%kaos_balance%` | Player's current balance (formatted: K, M, B, T) |

---

## Building from Source

```bash
git clone https://github.com/Kaos-Studios/KaosEssentials.git
cd KaosEssentials
mvn clean package
```

The compiled `.jar` will be in the `/target` directory.

---

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/my-feature`)
3. Commit your changes (`git commit -m 'Add my feature'`)
4. Push to the branch (`git push origin feature/my-feature`)
5. Open a Pull Request

---

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## Links

- [Website](https://kaostudios.dev)
- [Discord](https://discord.gg/EvV7BdVaAU)
- [Modrinth](https://modrinth.com/plugin/kaosessentials)
- [CurseForge](https://www.curseforge.com/minecraft/bukkit-plugins/kaosessentials)

---

<sub>Made with care by [Radu](https://github.com/Kaos-Studios) · KAOS Studios</sub>
