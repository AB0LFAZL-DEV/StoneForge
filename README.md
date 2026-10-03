# ⚒️ StoneForge

### Independent Minecraft Bedrock Server Software

**StoneForge** is an independent Minecraft Bedrock server software project focused on performance, extensibility, developer freedom, and a powerful multi-language plugin ecosystem.

Built with a modular architecture, StoneForge provides a foundation for creating and running custom Bedrock servers without relying on another server implementation as its core.

<!-- StoneForge Badges -->

![Minecraft Bedrock](https://img.shields.io/badge/Minecraft%20Bedrock-1.21.x-3CB371?style=for-the-badge&logo=minecraft&logoColor=white)
![Go](https://img.shields.io/badge/Go-1.25-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES202x-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Java](https://img.shields.io/badge/Java-21-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-8.x-777BB4?style=for-the-badge&logo=php&logoColor=white)

![Protocol](https://img.shields.io/badge/Protocol-Multi--Version-5865F2?style=for-the-badge)
![Plugin API](https://img.shields.io/badge/Plugin%20API-Multi--Language-7289DA?style=for-the-badge)
![Networking](https://img.shields.io/badge/Networking-Bedrock-5865F2?style=for-the-badge)
![World](https://img.shields.io/badge/World-Chunk%20%2F%20Subchunk-8B5CF6?style=for-the-badge)

![License](https://img.shields.io/badge/License-Open%20Source-2EA44F?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active%20Development-orange?style=for-the-badge)
![GitHub](https://img.shields.io/badge/GitHub-StoneForge-181717?style=for-the-badge&logo=github&logoColor=white)

---

## 🚀 What is StoneForge?

StoneForge is designed to provide server owners and developers with a modern and extensible Minecraft Bedrock server platform.

The project brings together networking, players, worlds, blocks, items, inventories, commands, events, permissions, plugins, configuration, UI systems, and developer APIs into one unified server architecture.

StoneForge is built with one core idea:

> **Forge your own server.**

---

## ✨ Core Features

- 🎮 Minecraft Bedrock server core
- 🌐 Bedrock network & protocol architecture
- 🔀 Multi-version protocol architecture
- 👤 Player & session management
- 🌍 World management
- 🧱 Block & block-position APIs
- 📦 Chunk & subchunk-oriented world architecture
- 🎒 Inventory system
- 🧩 Item & ItemStack APIs
- 💬 Command system
- ⚡ Event system
- 🔐 Permission system
- ⏱️ Scheduler
- 🔌 Plugin architecture
- 💾 Plugin data & configuration
- 🖥️ Server console & administration
- 📊 Scoreboard APIs
- 🟥 BossBar APIs
- 📝 Forms & Bedrock UI APIs
- 📡 Packet-level networking
- 🧬 NBT support
- 📚 Built-in HTML documentation
- 🐍 Python API
- 🟨 JavaScript API architecture
- ☕ Java API architecture
- 🐘 PHP API architecture

---

## 🌐 Multi-Version Architecture

StoneForge is designed around a protocol-adapter architecture that allows the server core to remain independent from individual Bedrock protocol versions.

Instead of building the entire server around a single client version, protocol-specific functionality can be isolated inside dedicated adapters.

This architecture provides a foundation for supporting multiple Minecraft Bedrock releases while keeping higher-level server APIs stable.

---

## 👤 Player API

Players are first-class objects within StoneForge.

The player architecture provides access to concepts such as:

- Player name
- XUID
- Client version
- Protocol ID
- Position
- Rotation
- World
- Inventory
- Permissions
- Session state
- Messaging
- Disconnect handling

Plugins can interact with players through the server API without needing to directly manage low-level network connections.

---

## 🌍 World & Block System

StoneForge provides a block-oriented world architecture based around Minecraft's chunk and subchunk model.

The world API is designed around:

- Worlds
- Dimensions
- Coordinates
- Block positions
- Blocks
- Block states
- Chunks
- Subchunks
- World sessions

This provides the foundation required for custom gameplay, minigames, world editors, protection systems, arenas, and other server-side features.

---

## 🎒 Inventory & Items

StoneForge includes abstractions for inventories, items, and item stacks.

The inventory API provides functionality for:

- Reading slots
- Writing slots
- Adding items
- Removing items
- Managing item stacks
- Synchronizing inventory state

The item architecture is designed to separate item definitions from actual item instances and stacks.

---

## 💬 Commands

StoneForge provides a command architecture for both built-in and plugin commands.

The system is designed to support:

- Command registration
- Arguments
- Permissions
- Player commands
- Console commands
- Command feedback
- Plugin commands

Plugins can extend the server without modifying the StoneForge core.

---

## ⚡ Events & Scheduler

StoneForge uses an event-driven architecture that allows plugins to react to server activity.

The architecture includes events for areas such as:

- Player connections
- Player disconnections
- Player movement
- Chat
- Commands
- Server lifecycle
- Plugin lifecycle

The scheduler provides a controlled way for plugins to run delayed and repeating tasks.

---

## 🔌 Plugin System

Plugins are one of the main pillars of StoneForge.

A plugin can contain its own:

- Entry point
- Commands
- Event listeners
- Permissions
- Configuration
- Persistent data
- Scheduled tasks
- Server functionality

Example:

```text
plugins/
└── example-plugin/
    ├── plugin.json
    ├── main.py
    ├── README.md
    └── data/
