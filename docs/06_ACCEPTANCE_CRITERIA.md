# Acceptance Criteria

## Final master
- Duration: 58–62 seconds.
- Primary aspect ratio: 16:9.
- Minimum presentation master: 1080p.
- Preferred high-quality master: 4K if source generations/edit pipeline support it without upscaling artifacts.
- No black frames, broken transitions, accidental UI, watermarks, or temporary overlays.

## Architecture
PASS only if:
- Mazar Mall is recognizable from supplied references in all relevant shots.
- No obvious facade morphing.
- No unexplained floor-count changes.
- Balcony rhythm remains stable.
- Podium and crown identity remain coherent.

## Signature balcony shot
PASS only if:
- character is visibly on Floor 5 / second residential floor context;
- coffee is natural;
- hand is credible;
- sunset lighting is premium;
- wind/steam movement is subtle;
- no uncanny face or limb artifacts dominate;
- shot feels aspirational, not staged.

## Camera
- Stable.
- Cinematic.
- Physically understandable.
- No AI jitter.
- No accidental fisheye.
- No uncontrolled geometry penetration.

## Lighting
- Golden-hour progression is coherent.
- Transition to blue hour/night feels intentional.
- Night facade lighting does not become neon.

## Site truth
- Exact-site claim only with verified site plates.
- Otherwise final production log must retain SITE_MATCH_UNVERIFIED.

## Text / branding
- Correct Mazar Mall spelling.
- Logo not distorted.
- No fake contact information.
- No unapproved superlatives.
- End card readable for at least ~2 seconds.

## Technical QA
- No duplicate frames causing stutter.
- Consistent frame rate in final timeline.
- Audio peak and loudness checked.
- No clipping.
- Export opens and plays end-to-end.
- Shot source files and generation metadata retained.

## Client-presentation gate
Final status may be `READY_FOR_CLIENT_PRESENTATION` only when:
- all nine shots selected;
- architecture QA passes;
- balcony signature shot passes;
- final edit passes duration and audio checks;
- end card approved;
- no known high-severity visual defects remain.
