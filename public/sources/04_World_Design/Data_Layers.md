# 🧩 Data Layers – *Bleak Horizons*

Used for conditional world states in [[World Partition]] and within [[Level Instances]].

## 🏗️ Use Cases

### Environmental Shifts
- `DL_RustTown_Rebuilt`
- `DL_Graveyard_Cleansed`
- `DL_Swamp_Corrupted`

### Faction Control
- `DL_Battalion_Active`
- `DL_HorizonLiberated`

### Rift Influence
- `DL_TimeGlitch_Active`
- `DL_RiftBloom_Overgrowth`

---

## ⚙️ Blueprint Integration

- Toggle with `SetDataLayerState()` node
- Can be triggered from:
  - Story events
  - Player actions
  - Time loop resets

> Layers let us shift the world without loading a new level. They’re your secret narrative weapon.
