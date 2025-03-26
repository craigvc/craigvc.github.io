# 💾 SaveGame Systems – *Bleak Horizons*

Saving is tied to narrative logic and player choice, not simple checkpoints.

---

## 🧠 System Overview

### Core Save Object
- Stores:
  - Player stats & position
  - Anchored inventory
  - Rift progression
  - [[Valtorin]] unlocks
  - Faction reputation

### Save Triggers:
- Campsites
- Terminals
- Watch-based checkpoint
- Major loop resets

---

## ⏱ Integration with Time Loops

- Save only carries forward “anchored” variables
- Use loop-aware SaveGame variant to track echoes
- Tracks:
  - Total loops
  - Echo confrontations
  - Unlocked endings

---

## 🔄 Technical Blueprint Setup

- Use `Create SaveGame Object` + `SaveGameToSlot`
- Load with `LoadGameFromSlot`
- Branch logic if no save exists → start intro sequence

---

> You don’t just save the game. You preserve the story you *might* remember.
