# 🔧 Unreal Blueprint Notes – *Bleak Horizons*

Blueprint systems drive the game's logic, interaction, and dynamic streaming.

---

## 🧠 Core Systems

### ✅ GameInstance
- Stores global variables: Rift state, player progress, loop count
- Manages transitions between major zones

### 🧭 GameMode / PlayerController
- Supports time loop conditions
- Handles UI transitions, death triggers, event logging

---

## 🗺 World Partition Streaming

### Load Logic:
- `LoadLevelInstanceBySoftObjectPtr()`
- `UnloadLevelInstance()`
- Manual control for seamless transitions (e.g. loading `LI_RustTown` when entering canyon cell)

---

## 🔄 Loop Reset System

- Blueprint macro for time rewind with VFX
- Calls to restore player inventory and anchored variables
- Optional memory shard tracking system

---

## 🎮 Combat + Spellcasting BPs

- Combat blueprint tree links to Animation Graphs
- Valtorin’s magic abilities spawn Niagara effects via `SpawnActorFromClass`
- Cooldowns handled via Timeline nodes

> Blueprint scripting should reflect a warped but intentional flow of logic, like a spell book gone digital.
