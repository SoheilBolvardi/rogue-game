# \# Rogue Game

# 

# A C-based grid-based dungeon game featuring procedural map generation, combat, items, weapons, spells, player progression, accounts, and persistent game statistics.

# 

# \## Overview

# 

# This project is a console-based Rogue-style game developed in C.

# 

# The game combines a procedurally generated grid-based environment with exploration, combat, resource management, items, weapons, spells, and progression. It also includes a player account system, persistent player data, and a leaderboard.

# 

# The project uses \*\*ncurses\*\* for terminal-based interaction and \*\*SDL2 / SDL\_mixer\*\* for graphical and audio functionality.

# 

# \## Features

# 

# \### Gameplay

# 

# \* Procedurally generated rooms and corridors

# \* Grid-based player movement

# \* Room and door generation

# \* Exploration and visited-position tracking

# \* Multiple enemy types

# \* Close-range and ranged combat

# \* Health, damage, and movement-related mechanics

# \* Food and consumable items

# \* Gold and treasure

# \* Weapons and ammunition

# \* Spell system

# \* Traps and environmental obstacles

# \* Stairs and level progression

# \* Score and step tracking

# \* Game-over and final-state handling

# 

# \### Enemies

# 

# The game contains multiple enemy types with individual position, health, and movement-related state, including:

# 

# \* Demon

# \* Flying/fast monster

# \* Giant

# \* Snake

# \* Undead

# 

# \### Weapons and Items

# 

# The game models several item and weapon types as separate entities:

# 

# \* Arrows

# \* Swords

# \* Daggers

# \* Wands

# \* Food

# \* Gold

# \* Special gold

# \* Health items

# \* Speed items

# \* Damage items

# 

# Weapons can have their own quantities and positions within the game world.

# 

# \## Player \& Account System

# 

# The game includes a complete account and player-data system.

# 

# \### Account functionality

# 

# \* Account creation

# \* Login

# \* Guest mode

# \* Username validation

# \* Password validation

# \* Email validation

# \* Persistent player data

# 

# \### Player progression

# 

# Player state includes information such as:

# 

# \* Username

# \* Level

# \* Difficulty

# \* Health

# \* Food

# \* Gold

# \* Music settings

# \* Number of games

# \* Number of logins

# \* Total collected gold

# 

# \## Leaderboard

# 

# Player performance is persisted and can be compared through a leaderboard system.

# 

# The project includes functionality for:

# 

# \* Loading player data

# \* Saving player data

# \* Comparing players

# \* Sorting player records

# \* Displaying the leaderboard

# 

# \## Map Generation

# 

# The game world is represented as a grid composed of generated rooms and connecting corridors.

# 

# Rooms contain properties such as:

# 

# \* Position

# \* Width and height

# \* Number of doors

# \* Door locations

# \* Spell-related state

# 

# The map-generation system includes validation of positions, room creation, corridor generation, and rendering of the resulting environment.

# 

# \## User Interface

# 

# The game contains several menu and interaction systems, including:

# 

# \* Main menu

# \* Game menu

# \* Settings

# \* Music settings

# \* Food menu

# \* Spell menu

# \* Weapon menu

# \* Quit confirmation

# \* Final/game-over menu

# 

# The terminal interface is implemented using \*\*ncurses\*\*.

# 

# SDL2 and SDL\_mixer are also used for graphical and audio functionality.

# 

# \## Architecture

# 

# The project is implemented in C using structured data types to represent the major entities of the game.

# 

# The main data model includes:

# 

# ```text

# Position

# &#x20;  │

# &#x20;  ├── Player

# &#x20;  ├── Room

# &#x20;  ├── Door

# &#x20;  ├── Pillar

# &#x20;  ├── Trap

# &#x20;  ├── Gold

# &#x20;  ├── Weapons

# &#x20;  ├── Items

# &#x20;  ├── Stairs

# &#x20;  └── Enemies

# ```

# 

# Major gameplay systems include:

# 

# ```text

# &#x20;                   ┌─────────────────┐

# &#x20;                   │   Main Program  │

# &#x20;                   └────────┬────────┘

# &#x20;                            │

# &#x20;         ┌──────────────────┼──────────────────┐

# &#x20;         │                  │                  │

# &#x20;         ▼                  ▼                  ▼

# &#x20;    Account System      Game Menus       Game Engine

# &#x20;         │                  │                  │

# &#x20;         ▼                  ▼                  ▼

# &#x20;  Login / Register     Settings / UI     Map Generation

# &#x20;  Player Data          Inventory         Movement

# &#x20;  Leaderboard          Weapons           Combat

# &#x20;                                            │

# &#x20;                        ┌───────────────────┼──────────────────┐

# &#x20;                        │                   │                  │

# &#x20;                        ▼                   ▼                  ▼

# &#x20;                     Enemies             Items            Progression

# ```

# 

# \## Technologies

# 

# \* \*\*C\*\*

# \* \*\*ncurses\*\*

# \* \*\*SDL2\*\*

# \* \*\*SDL\_mixer\*\*

# \* POSIX/system libraries

# \* `pthread`

# 

# \## Project Structure

# 

# ```text

# Rogue/

# ├── rogue.c

# ├── players.txt

# └── users.txt

# ```

# 

# `rogue.c` contains the core game implementation, including the game state, data structures, map generation, menus, account system, combat, items, and gameplay logic.

# 

# \## Project Context

# 

# This project was developed as part of the \*\*Fundamentals of Programming\*\* coursework at Sharif University of Technology.

# 

# The project focuses on implementing a non-trivial interactive application in C while managing a relatively large game state, multiple interacting entities, procedural map generation, user interaction, persistent data, and gameplay mechanics.

# 

# \## Author

# 

# \*\*Soheil Bolvardi\*\*

# 

# Electrical Engineering \& Mathematics Student



