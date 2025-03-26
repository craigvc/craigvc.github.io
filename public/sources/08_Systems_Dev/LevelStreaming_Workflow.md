# 📂 Level Streaming Workflow – *Bleak Horizons*

All modular zones are streamed using Blueprint logic with no traditional sublevels.

---

## 🗺 World Partition Streaming

### Key Nodes:
- `LoadLevelInstanceBySoftObjectPtr()`
- `UnloadLevelInstance()`
- `GetStreamingLevel` → check loaded status

### Uses:
- Load `LI_JunkCity` when entering canyon
- Unload `LI_BanditCamp_A` after escape
- Switch `LI_SwampRuins` versions using [[Data Layers]]

---

## 🚪 Portal Transitions

For rift travel:
- Use fade + load level + teleport player
- Optional cutscene or hallucination glitch VFX

---

## 🧠 Memory Efficiency

- Unload previous zones during rift events
- Disable tick on unloaded actors
- Maintain global variables via [[GameInstance]]

> Levels aren’t just spaces — they’re states of memory.
