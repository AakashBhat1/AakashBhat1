# Banner video prompt — `assets/banner.mp4`

Use this brief with Runway Gen-3, Kling, Luma Dream Machine, Sora, or fal.ai Seedance. Save the output as `assets/banner.mp4` (and optionally `.gif` for broader fallback). The README references both; whichever exists will render.

## Specs

- **Dimensions:** 1500 × 500 (aspect 3:1).
- **Duration:** 6–8 seconds, **seamless loop** (first frame = last frame).
- **Frame rate:** 24 fps.
- **Format:** MP4 (H.264, yuv420p), ≤ 2 MB so GitHub renders it inline without lazy-loading delay. Optionally export a `.gif` ≤ 1.5 MB as fallback.
- **Audio:** none.

## Art direction

Identical visual world to the still banner (`banner_prompt.txt`) — read that first. The video is the same composition with a quiet, almost subliminal motion layer.

- **Background:** static off-white paper texture, no movement.
- **Motion 1 — line-work parallax:** the topographic / wireframe linework on the right third drifts laterally by 8–12 pixels over the loop, then returns. Easing: extremely soft.
- **Motion 2 — bounding box:** the single hairline rectangular bounding box draws itself in (corner → corner, ~1.5 s), holds for 3 s, then fades out (0.5 s). On loop restart the draw begins again, so the box visibly "breathes" once per cycle.
- **Motion 3 (optional):** the two corner crop marks blink in for 200 ms once mid-loop, like a viewfinder cue.
- **No camera move.** No zoom, no pan, no parallax of the whole frame, no dolly.
- **No effects:** no particles, no light leaks, no film grain animation, no chromatic aberration.

## Hard negatives

no people, no faces, no camera motion, no zoom, no pan, no glitch, no purple, no neon, no glow, no 3D, no flashy transitions, no music

## Copy-paste prompts

**Runway Gen-3 / Kling (image-to-video, recommended):**
1. First generate `banner.png` from `banner_prompt.txt`.
2. Use that PNG as the conditioning image.
3. Prompt:
```
seamless 8 second loop, the static off-white paper background does not move; a single hairline rectangular bounding box on the right third draws itself corner to corner over 1.5 seconds, holds for 3 seconds, then fades to invisible; the surrounding topographic linework drifts laterally by 10 pixels and returns; no camera movement, no zoom, no pan, calm and quiet, magazine masthead in motion
```

**Sora / Luma (text-to-video fallback):**
```
A 1500x500 minimalist editorial banner, off-white paper background, deep charcoal hairline linework gathered on the right third. A single thin rectangular bounding box draws itself corner to corner over 1.5 seconds, holds, then fades. The linework drifts 10 pixels laterally and returns. Seamless 8-second loop. No camera movement. Monochrome. No people, no neon, no glow.
```

## Post-processing checklist

- [ ] Confirm first and last frames are visually identical (loop seam invisible).
- [ ] Re-encode with `ffmpeg -i in.mp4 -vcodec libx264 -pix_fmt yuv420p -movflags +faststart -an out.mp4` to keep file size down and ensure inline playback.
- [ ] Verify file ≤ 2 MB. If larger, reduce bitrate or trim to 6 s.

## Save as

`C:\Users\zewan\OneDrive\Desktop\demo\o\AakashBhat1\assets\banner.mp4`
