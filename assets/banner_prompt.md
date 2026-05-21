# Banner image prompt — `assets/banner.png`

Use this brief with Midjourney v6, Imagen, Flux, or any high-quality text-to-image model. Save the output as `assets/banner.png` and the README will pick it up automatically.

## Specs

- **Dimensions:** 1500 × 500 pixels (aspect 3:1). GitHub renders README at ~1012 px wide on desktop; 1500 px gives crisp scaling on retina without forcing a download penalty.
- **File:** PNG, ≤ 600 KB. Strip metadata.
- **Color space:** sRGB.

## Art direction — minimalist editorial

Think a Monocle or Kinfolk masthead, not a tech YouTube thumbnail.

- **Background:** off-white (#F6F4EE) or warm paper grey. No vignette.
- **Palette:** monochrome. Single ink accent in deep charcoal (#1C1C1C) or near-black. Optional one muted secondary (cool grey).
- **Composition:** wide negative space. Strong horizontal axis. Rule of thirds: subject anchored right-third, type lower-left, the middle third intentionally empty.
- **Subject:** abstract topographic line-work, or a low-poly geometric wireframe, suggesting computer vision without being literal. On the right third, a single faint rectangular bounding box drawn in a 1px hairline — readable but never loud. Above or beside it, two tiny corner brackets like crop marks.
- **Texture:** subtle paper grain at very low opacity. No film burn, no glitch, no chromatic aberration.
- **Type (optional — omit if the model handles type poorly):**
  - "AAKASH BHAT" set in a tight-tracked geometric sans-serif (Inter, Söhne, GT America), small caps, 14pt feel.
  - Lower-left, 64 px from the edges.
  - Below it, in a lighter weight: "COMPUTER VISION · FULL-STACK".

## Hard negatives

no people, no faces, no stock photo, no purple, no indigo, no magenta, no neon, no glow, no 3D chrome, no anime, no glitch, no emoji, no rainbow gradient, no laptop on a desk, no abstract galaxy

## Copy-paste prompts

**Midjourney v6:**
```
editorial minimalism magazine masthead banner, off-white paper background #F6F4EE, single deep ink accent #1C1C1C, abstract topographic linework on right third, faint 1px rectangular bounding box and small corner crop marks, vast negative space middle, subtle paper grain, calm and quiet, magazine cover composition, no people, no neon, no purple, no glow, no chrome, no anime, no glitch, monochrome --ar 3:1 --style raw --v 6
```

**Flux / Imagen (natural language):**
```
A minimalist editorial banner, 1500x500. Off-white paper background, one deep charcoal accent, abstract topographic linework gathered on the right third with a single faint hairline bounding box and small corner crop marks. Vast empty space in the middle. Subtle paper grain. Magazine masthead composition, quiet and modern. Monochrome only. No people, no purple or neon, no 3D, no glow.
```

## Save as

`C:\Users\zewan\OneDrive\Desktop\demo\o\AakashBhat1\assets\banner.png`
