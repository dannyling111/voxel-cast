# 方块人偶 · Voxel Cast

3D Minecraft-style figure studio. Nine reference characters are rebuilt as
Steve-rigged voxel dolls, then remixed by swapping **head / body / arms / legs**.

**Live GitHub Page:** https://dannyling111.github.io/voxel-cast/

## What you can do

- **原作** — 3×3 cast copied from the reference sheet (Dan, Kero, Nana, Cross, Rex, Iris, Frost, Kerodan, Draft)
- **生成** — 12 mix-and-match figures; **换一批** rolls a new random set (8⁴ − 8 = 4088 unique combos)
- **工坊** — pick each slot yourself, spin, download a 64×64 Minecraft skin PNG
- **工法** — the five-step method (split, paint, rig, swap, generate)

## Method (short)

1. **Split** every doll into four slots on the classic Steve skeleton (head 8³, body 8×12×4, limbs 4×12×4).
2. **Paint** a 64×64 Minecraft UV skin, nearest-neighbor, one kit per original.
3. **Rig** the skin onto boxes with a 3/4 studio pose and orbit camera.
4. **Swap** any slot — Kerodan = Kero head + Dan clothes, already in the sheet.
5. **Generate** random recipes from the eight kits.

## Run locally

This GitHub Page is a static bundle (`index.html` + `app.js`). Open it as any static site, or:

```bash
python3 -m http.server 8080
```

Source skins live in the app as procedural pixel painters (no image assets).
