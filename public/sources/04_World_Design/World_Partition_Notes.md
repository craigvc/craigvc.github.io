# 🌍 World Partition Notes – *Bleak Horizons*

## 🗺️ Main World: Wasteland_Main

- Built using [[Unreal Engine 5.5]] World Partition system
- One massive landscape divided into streamed cells
- Contains terrain, ruins, natural biomes, and fast travel zones

### 📦 Streaming Logic
- Always-active cells: player hub zones (e.g., [[Rust Town]])
- Event-triggered loads: Rift surge zones, ambush regions
- Data Layers allow conditional toggling (e.g., Ruined vs. Rebuilt towns)

---

## 🌀 Rift Realm & Other Worlds

- Rift events teleport Alex to alternate dimension maps
- Loaded via `OpenLevel()` Blueprint calls
- Includes:
  - [[Rift Core Zone]]
  - [[Fantasy Kingdom]]
  - [[Swamp of Poor Life Choices]]
  - [[Haunted Rift City]]

---

## 🧠 Streaming Best Practices

- Avoid Sublevels — rely on World Partition + Level Instances
- Use RVT blending for terrain/mesh transitions
- Place persistent level blueprint logic in a global GameInstance or Manager BP
