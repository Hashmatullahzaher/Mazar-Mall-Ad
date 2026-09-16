# Higgsfield Production Workflow

## Principle
Do not ask a video model to invent the building and animate it at the same time when identity matters. Establish strong visual anchors first, then animate.

## Current recommended model policy
Model availability changes. Codex must query the connected Higgsfield model catalog at execution time.

As of the current production setup, strong candidates include:
- **Seedance 2.5** — preferred default for reference-heavy architectural image/video work, omni-reference, 4–30s, up to 1080p.
- **Kling 3.0** — strong for cinematic multi-shot / audio-capable generation and high-quality image-to-video.
- **Cinema Studio Video V2** — useful for refined cinematic camera/color treatments.
- **Seedance 2.0** — high-resolution reference-driven fallback, including 4K where supported.
- **MiniMax H3 Max** — fast multimodal/keyframe fallback.

Do not hard-code these forever. Discover before spending credits.

## Required generation strategy

### Stage A — Reference audit
For every shot:
- identify canonical building references;
- identify whether exact site plate exists;
- identify character/interior references;
- assign a continuity risk level: LOW / MEDIUM / HIGH.

### Stage B — Keyframe creation
For high-risk shots, generate or compose a high-quality still first.
Astra must approve:
- building identity;
- camera composition;
- floor placement;
- lighting;
- human scale;
before video generation.

### Stage C — Image-to-video
Animate the approved still using Higgsfield.

Preferred baseline:
- 16:9
- 5–8 seconds per shot
- highest practical quality for selected final candidates
- generate audio only if it adds useful production sound; final mix remains separate

### Stage D — Candidate strategy
For each shot:
- generate low-cost/preflight candidates first when practical;
- keep 2–4 candidates;
- score them;
- promote only selected candidates to expensive/high-quality reruns if needed.

Never regenerate blindly.

### Stage E — Scoring
Score every candidate 1–5:
1. Architecture identity
2. Composition
3. Camera stability
4. Human realism
5. Lighting continuity
6. Physics / motion
7. Editability
8. Emotional value

Reject any candidate with architecture identity <4 even if aesthetically beautiful.

## Shot-specific guidance

### SH01 / SH08 / SH09 exterior hero
Use multiple exterior references. Prioritize facade identity. Camera motion should be slow enough to preserve geometry.

### SH02 street shot
If no true site plate exists, do not claim exact site. Use contextual urban environment and mark SITE_MATCH_UNVERIFIED.

### SH03 vertical reveal
Use a pre-established clean facade frame. Avoid generating long vertical travel from text alone.

### SH04–SH05 balcony
First create a still that proves the person is on Floor 5. Then animate subtle body, steam, wind, and camera motion.

### SH06 interior
Use supplied furnished plan references as style/space evidence, but do not claim a specific legal apartment layout unless mapped and approved.

### SH07 amenities
Favor impressionistic-but-believable short glimpses. Do not invent branded operators.

## Higgsfield tool behavior expected from Codex
If Higgsfield tools are connected:
1. discover models;
2. inspect chosen model constraints;
3. estimate cost before expensive batches when possible;
4. submit generations;
5. wait/poll jobs;
6. save job IDs, model IDs, prompts, parameters, and output URLs;
7. download selected outputs into repo workspace or approved storage;
8. update shot manifest/status;
9. never claim success before job completion.

If Higgsfield is not connected:
- do not fabricate outputs;
- generate complete prompt packs under `prompts/shots/`;
- mark status `BLOCKED_HIGGSFIELD_CONNECTION`.
