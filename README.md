# RankedSMP - Better

[![Modrinth](https://img.shields.io/badge/Modrinth-Available_Now-00AF5C?style=for-the-badge&logo=modrinth)](https://modrinth.com/plugin/rankedsmp-better)

A PaperMC plugin for Minecraft 1.21.x that adds a competitive ranking system with unique abilities, extra inventory, and more.

**Current Version:** 1.6.0

---

## What It Does

When you run `/rankedsmp start`, every online player gets a random rank from 1 to 50. Lower numbers are better - they get stronger abilities, more health, extra inventory space, and longer potion effects.

New players joining later automatically get a random rank too.

---

## Features

- **Random unique ranks** (1-50, no duplicates)
- **Rank display** in nametags (bold, red, customizable)
- **Rank swap** - kill someone with a better rank to steal it
- **5 unique abilities** based on rank tier
- **Extra inventory** slots for top ranks
- **Extended potion duration** for ranks 1-30
- **Rank-based health** - better ranks get more hearts
- **Action bar display** showing your ability and cooldown
- **Full admin controls** for managing ranks

---

## Abilities

| Rank | Ability | How to Use | Cooldown |
|------|---------|------------|----------|
| 1-5 | Fireball | Right-click Fire Charge | 30s |
| 6-10 | Angel Strike | Right-click Ghast Tear | 60s |
| 11-15 | Sonic Boom | Right-click Echo Shard | 120s |
| 16-20 | Dash | Right-click Feather | 45s |
| 21-50 | None | - | - |

### Fireball (Ranks 1-5)
Shoots an explosive fireball that breaks blocks and sets things on fire. Direct hits deal 10 hearts of damage.

### Angel Strike (Ranks 6-10)
Creates a stationary ring of divine energy at your feet. First hit does 7 hearts, then 2 hearts every 0.1 seconds for 8 seconds. The ring stays where you cast it.

### Sonic Boom (Ranks 11-15)
Warden-style shockwave attack. Deals 8 damage in a 10 block line. Horizontal knockback only.

### Dash (Ranks 16-20)
Instantly dash forward in the direction you're looking.

---

## Health by Rank

Better ranks get more hearts:

| Rank | Hearts |
|------|--------|
| 1 | 16 |
| 2-3 | 15.5 |
| 4-5 | 15 |
| 6-10 | 14.5 |
| 11-15 | 14 |
| 16-20 | 13.5 |
| 21-25 | 13 |
| 26-30 | 12.5 |
| 31-35 | 12 |
| 36-40 | 11.5 |
| 41-45 | 11 |
| 46-50 | 10.5 |

Configurable in `health-config.yml`.

---

## Extra Inventory

Top ranks get bonus storage:

| Rank | Slots |
|------|-------|
| 1-5 | 36 |
| 6-10 | 27 |
| 11-15 | 18 |
| 16-20 | 9 |
| 21+ | 0 |

Use `/ei` to open your extra inventory. Items drop on death.

---

## Commands

### Admin Commands (OP only)

| Command | Description |
|---------|-------------|
| `/rankedsmp start` | Start ranking |
| `/rankedsmp stop` | Stop and clear ranks |
| `/rankedsmp reload` | Reload config |
| `/rankedsmp status` | View status |
| `/rankedsmp unrank <player>` | Remove player's rank |
| `/rankedsmp rankset <player> <rank>` | Set player's rank |
| `/rankedsmp ranklist` | Open GUI with all ranked players |
| `/rankedsmp rankreplace <p1> <p2>` | Swap two players' ranks |
| `/rankedsmp playerinv <player>` | View player's extra inventory |
| `/rr <p1> <p2>` | Shortcut for rankreplace |

### Player Commands

| Command | Description |
|---------|-------------|
| `/extrainventory` | Open extra inventory |
| `/extrainv` | Same as above |
| `/ei` | Same as above |

---

## Configuration Files

### config.yml
Main settings - ranks, display, abilities, potion extension, action bar styling.

### health-config.yml
Health values per rank tier.

### extrainv-config.yml
Extra inventory settings and drop behavior.

---

## Requirements

- PaperMC 1.21.4
- Java 21

---

## Changelog

### v1.6.0
- Added action bar bold/color customization
- Added `/playerinv <player>` command
- Added `/rankset <player> <rank>` command
- Added rank-based health system (separate config)
- Added health-config.yml

---

All Rights Reserved. 
