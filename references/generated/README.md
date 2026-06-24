# Generated Asset Library — IMS Managed Services Site

This folder is the **planned image set** for the upcoming redesign run of
`index.html`. Because the web session that wrote these specs does not have a
raster image generator wired in, the actual PNGs are produced **outside the
session** by pasting the prompts in `PROMPTS.md` into a high-quality image
generator (Midjourney, Gemini, Claude image gen, etc.). The generated files
are then saved into this folder using the filenames listed in `SLOTS.md`.

> The 2 photos already in `/references/` (`Boardroom_CollaborationSpace.png`,
> `Delegate_Assembly_colorgraded.png`) are the **brand mood anchor**. Every
> generated asset must feel like it could sit next to those two without
> looking out of place.

---

## Brand world (read before generating anything)

Anchor every prompt to this world. Drift will be obvious.

| Lever | Direction |
|---|---|
| Palette | Deep Navy `#001833` / `#002D56`, Precision Gold `#ECAE3D`, Technical Blue `#004B8D`, Ink Charcoal `#1A1A1A`, Soft Cream `#F9F9F9` |
| Lighting | Cinematic, controlled, mostly cool ambient with a single warm accent. Practical lights (sconces, screens) provide the warmth. |
| Format | Large-format camera feel. 50–85mm equivalent. Moderate DOF. No fisheye. No fake bokeh. |
| Texture | Faint film grain. Matte surfaces. Brushed metal, walnut, soft wool felt, glass with low reflections. |
| Subject | Real corporate AV environments — boardrooms, NOCs, control rooms, broadcast suites, training rooms, executive lobbies, server/rack rooms, technicians at work. |
| Mood | Quiet competence. Premium. Editorial. Operational, not theatrical. |

### Anti-slop (negative prompt — paste into every generation)

> no glowing holographic UI, no neon, no purple/teal AI gradient, no lens
> flares, no light-streak overlays, no glass orbs, no centered face portrait,
> no fake brand logos, no readable text overlays, no stock-photo handshake,
> no headset call-center cliché, no fisheye, no tilt-shift miniature, no
> heavy vignette, no oversaturation.

---

## Workflow for the redesign run

1. Open `PROMPTS.md`. Each prompt is numbered and matches a filename in `SLOTS.md`.
2. Generate each image at the recommended aspect ratio and resolution.
3. Save the file into this folder using the filename in `SLOTS.md` — do **not** rename.
4. When all 13 core assets are present, the redesign pass can wire them into `index.html` directly using the slot table.
5. The pillar set (`pillar_01` → `pillar_04`) must be generated together in one session for color/light consistency — regenerate the whole set rather than swapping one image.

---

## Files in this folder

- `README.md` — this file (overview, brand world, workflow).
- `PROMPTS.md` — one prompt per asset. Self-contained, paste-and-go.
- `SLOTS.md` — filename → site section → aspect ratio → CSS slot mapping. The redesign pass reads this to wire each image into `index.html`.
