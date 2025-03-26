# 🪨 Runtime Virtual Texture (RVT) Setup – *Bleak Horizons*

RVT allows terrain and mesh blending for seamless level integration, especially around modular Level Instances.

---

## ✅ Enable RVT in Landscape Material

- Add RVT output node to Landscape Master Material
- Connect base color, normals, roughness

---

## 🧱 Setup on Level Instance Meshes

1. Use Material Instance with RVT Sampler node
2. RVT Sampler pulls terrain color + normal
3. Blend mask controls falloff between terrain and mesh

---

## 🎛 Additional Tools

- World Position Offset for subtle shifting ground
- Dithered Alpha masks to fade mesh edges
- Use decals and foliage to cover seams

> Make magic ruins feel grown into the ground — not dropped in.
