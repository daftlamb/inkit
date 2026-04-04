# Ink It ✦

> Draw a stroke. Watch it become a sculpture.

Ink It is an experimental drawing tool that turns 2D brushwork into 3D objects in real time. Draw on the left — a rotatable, exportable 3D form appears on the right. Part sketchbook, part sculpture studio.

---

## What it does

You draw freehand strokes on a canvas. Ink It extrudes and lathes them into three-dimensional shapes using Three.js, rendered with physically-based materials. Rotate the result, switch materials, export to GLB or STL — ready for Blender, a 3D printer, or a spatial app.

---

## Tools

| Tool | Shortcut | Description |
|------|----------|-------------|
| **Brush** | `B` | Freehand pressure-sensitive strokes |
| **Pen** | `P` | Bézier curve tool with anchor points |
| **Eraser** | `E` | Remove strokes by hit |
| **Shape** | `S` | Stamp geometric primitives (circle, rect, hexagon, star) |

**Symmetry** — set axis count for radial/mirror drawing (2, 3, 4, 6…)

---

## Materials

Six material presets for the 3D view:

- **Chrome** — reflective mirror finish
- **Matte** — soft diffuse surface
- **Gold** — warm metallic
- **Liquid** — translucent, refractive
- **Steel** — brushed metal with swirl + Fresnel shader
- **Custom** — pick your own color

---

## Export

| Format | Use |
|--------|-----|
| PNG 1× / 2× / 4× | Transparent background, high-res |
| GLB | Import into Blender, Unity, Vision Pro |
| STL | 3D printing |
| Dither | Halftone/risograph-style flat render |

---

## Other features

- **Split view** — canvas on the left, live 3D on the right
- **Dark mode** — toggle light / dark theme
- **Auto-rotate** — slow spin for presentation
- **Draft autosave** — strokes saved to localStorage, restored on reload
- **Keyboard shortcuts** — `B` / `P` / `E` / `S`, `?` for shortcut modal

---

## Tech

- Drawing: Canvas 2D API
- 3D: [Three.js](https://threejs.org/) r160, `LatheGeometry` + `TubeGeometry`
- Materials: `MeshStandardMaterial`, `MeshPhysicalMaterial`, custom `ShaderMaterial` (Steel)
- HDR lighting: studio.hdr
- No framework. No build step. One HTML file.

---

## Try it

→ **[inkit.pages.dev](https://inkit.pages.dev)** *(coming soon)*

Or clone and open `index.html` in a browser.

---

## Made by

Design by [Mog](mailto:daftlamb@gmail.com)

Part of the *\*It* series of single-purpose creative tools.
