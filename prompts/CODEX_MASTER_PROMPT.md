# CODEX MASTER PROMPT — MAZAR MALL 60-SECOND CGI AD

## Repository
`Hashmatullahzaher/Mazar-Mall-Ad`

## Mission
Build a premium 60-second CGI advertisement for a client presentation of Mazar Mall.

The film must make the client feel that Mazar Mall already exists and that they are briefly experiencing life inside the completed project.

This is not a generic AI real-estate montage.

The approved creative concept is:

**TOMORROW HAS A VIEW**

The signature emotional scene is:
**Floor 5 — the second residential floor — a resident stands on a balcony with coffee in hand, watching the sunset over Mazar.**

You are the production orchestrator.

Use:
- **Astra** as the required cinematic creative-director / reasoning layer when it is available in the execution environment.
- **Higgsfield** as the image/video generation backend.
- repository files as the source of truth for architecture, references, versions, prompts, selections, and QA.

Do not ask me to manually manage each generation. Operate the production systematically and present only meaningful approval gates or true blockers.

---

# 1. FIRST — READ THE REPOSITORY

Before generating anything, read:

1. `README.md`
2. `AGENTS.md`
3. `docs/01_CREATIVE_BRIEF.md`
4. `docs/02_PROJECT_FACTS.md`
5. `docs/03_STORYBOARD_60S.md`
6. `docs/04_VISUAL_CONTINUITY_BIBLE.md`
7. `docs/05_HIGGSFIELD_WORKFLOW.md`
8. `docs/06_ACCEPTANCE_CRITERIA.md`
9. `docs/07_ASSET_MANIFEST.md`
10. `production/shot_manifest.json`
11. `production/status.json`

Inspect all assets under:
- `assets/references/exterior/`
- `assets/references/hero/`
- `assets/references/unit-plans/`
- `assets/references/plans/`
- `assets/site/`

Do not infer that an asset exists without checking it.

---

# 2. CREATE AN ISOLATED PRODUCTION BRANCH

Work on:

`production/v1-cinematic-ad`

Do not destroy or rewrite `main`.

Use small, meaningful commits.

---

# 3. VERIFY ASTRA BEFORE CREATIVE EXECUTION

Astra is the requested creative-director model/capability.

Discover the exact Astra capability available in your environment.

Do not invent a model ID.

If Astra is available:
- use it for cinematic concept validation;
- shot composition;
- transition design;
- prompt refinement;
- continuity analysis;
- candidate critique;
- edit critique.

If Astra is unavailable:
- do not silently claim it was used;
- continue all repository preparation and Higgsfield capability discovery;
- mark `production/status.json` with `ASTRA_UNAVAILABLE`;
- return a precise blocker report before spending significant generation credits.

---

# 4. VERIFY HIGGSFIELD CONNECTION AND MODEL CATALOG

Discover the connected Higgsfield tools and current video model catalog.

Do not hard-code an old model simply because it is named in the docs.

For this production, current strong candidates may include:
- Seedance 2.5
- Kling 3.0
- Cinema Studio Video V2
- Seedance 2.0
- MiniMax H3 Max

But you must inspect the live catalog before generation.

For each candidate model, determine:
- reference-image support;
- start/end frame support;
- multi-reference support;
- duration range;
- resolution;
- audio capability;
- cost;
- suitability for architecture identity.

Record the selected model policy in:

`production/model_selection.md`

Preferred default behavior:
- reference-heavy exterior/architecture shots → strongest identity/reference model;
- multi-shot or controlled cinematic sequence → strongest multi-shot model;
- keyframe / start-frame animation → model with strong image-to-video stability;
- final generation quality over speed once composition is locked.

Estimate cost before expensive generation batches when the connected tools support it.

---

# 5. ASSET TRUTH CHECK

Architecture references are canonical.

The film must preserve:
- curved white/ribbon balconies;
- dark glazing;
- white architectural frame;
- gold-patterned/perforated podium character;
- dark vertical spine/fins;
- crown/top silhouette;
- warm facade lighting.

A beautiful shot with the wrong building is a failure.

Inspect `assets/site/`.

If true site/drone plates are absent:
- set `SITE_MATCH_UNVERIFIED`;
- use a contextual Mazar urban environment only;
- do not claim exact real-world site reconstruction.

Never invent legal unit numbering, tenant brands, prices, phone numbers, or superlative marketing claims.

---

# 6. BUILD THE PRODUCTION IN SHORT SHOTS

Do NOT generate one 60-second video.

Use the nine-shot structure in `production/shot_manifest.json`.

Approximate timeline:

- SH01 0–6s — aerial landmark reveal
- SH02 6–12s — street-level presence
- SH03 12–19s — vertical rise
- SH04 19–27s — arrival at Floor 5
- SH05 27–38s — signature coffee/sunset moment
- SH06 38–45s — balcony-to-home reveal
- SH07 45–51s — lifestyle pulse
- SH08 51–56s — golden hour to blue hour
- SH09 56–60s — night hero / brand close

The edit may shift timing slightly, but final duration must remain 58–62 seconds.

---

# 7. KEYFRAME-FIRST PRODUCTION

For every HIGH or VERY_HIGH continuity-risk shot:

1. Have Astra design the frame.
2. Select exact repository references.
3. Create a high-quality keyframe / start frame.
4. Critique it against architecture and continuity.
5. Do not animate until the keyframe passes.

Create:

`prompts/shots/SHxx_keyframe.md`

for each shot.

Every keyframe prompt must specify:
- exact building features;
- camera height;
- lens feel;
- composition;
- time of day;
- materials;
- human scale;
- sun direction;
- negative constraints;
- reference paths.

Save approved keyframes under:

`outputs/keyframes/SHxx/`

Do not overwrite rejected candidates.

---

# 8. HIGGSFIELD VIDEO GENERATION

Once a keyframe is approved, create:

`prompts/shots/SHxx_video.md`

For each Higgsfield job, record:
- job ID;
- model;
- mode;
- references;
- prompt;
- negative constraints;
- duration;
- resolution;
- seed if available;
- cost estimate if available;
- output URL/path;
- date/time;
- candidate score.

Store metadata under:

`production/jobs/SHxx/`

Use image-to-video / omni-reference where that best protects Mazar Mall identity.

Do not blindly generate many expensive variants.

Candidate strategy:
- first pass: 2–4 targeted candidates when budget permits;
- score them;
- rerun only the most promising composition at higher quality if needed.

---

# 9. ASTRA CANDIDATE REVIEW

Astra must review each candidate against:

1. Architecture identity
2. Composition
3. Camera stability
4. Human realism
5. Lighting continuity
6. Physics/motion
7. Editability
8. Emotional value

Score each 1–5.

Architecture identity is a hard gate.

If Architecture Identity < 4/5:
REJECT.

Record reviews in:

`production/reviews/SHxx.md`

Do not select a visually beautiful but architecturally wrong shot.

---

# 10. SIGNATURE BALCONY SEQUENCE — HIGHEST PRIORITY

SH04 and SH05 are the emotional centerpiece.

The resident must be on:

**Floor 5 — the second residential floor.**

The character should:
- stand naturally on balcony;
- hold coffee casually;
- look at sunset, not camera;
- show subtle breathing;
- have slight wind in clothing/hair;
- have credible hands;
- not dominate the architecture.

The coffee:
- realistic cup/glass;
- subtle steam if visible;
- no morphing;
- no exaggerated product shot.

Camera:
- elegant 50–70mm feel on approach;
- slow;
- stable;
- premium;
- no dramatic FPV dive.

Lighting:
- richest sunset in the film;
- warm rim light;
- glass reflection;
- believable city depth.

Avoid face closeups unless the character remains fully stable.

This sequence gets extra generation budget before less important shots.

---

# 11. CONTINUITY BETWEEN SH04 → SH05 → SH06

These three shots must feel like the same moment.

Lock:
- same character;
- clothing;
- coffee;
- balcony;
- sunset direction;
- apartment;
- general camera side;
- time of day.

SH06 should feel like the camera gently moves backward from the balcony into the home.

Use furnished plan references for interior language, but do not claim an official apartment layout unless verified.

---

# 12. TRANSITIONS

Design transitions in the edit, not by forcing every model to create impossible geometry.

Preferred:
- camera-direction match;
- light-source match;
- reflection match;
- motion match;
- architectural line match;
- controlled dissolve only where elegant.

At most 1–2 “impossible” transitions in the full film.

Never allow a transition to warp the Mazar Mall facade.

---

# 13. SOUND

No voiceover is required for V1 unless separately approved.

Build a cinematic sound plan:
- city air;
- distant traffic;
- subtle architectural ambience;
- balcony wind;
- cup detail;
- tasteful impact/riser;
- night resolution.

If no licensed/approved music is available:
- do not steal or scrape music;
- produce a clean picture edit with temporary clearly-labelled music placeholder or native ambience;
- mark final music as pending.

Do not claim temporary music is cleared for public release.

---

# 14. EDIT AND ASSEMBLY

Use a deterministic local editing pipeline where possible.

Preferred:
- FFmpeg or equivalent reproducible CLI workflow;
- 16:9 timeline;
- 24fps or another explicitly selected cinematic frame rate;
- consistent color transform;
- consistent audio sample rate;
- no variable-framerate surprises.

Create:
- `production/edit/edit_plan.md`
- `production/edit/timeline.json`
- reproducible render script if practical.

Assemble selected shot masters only.

Do not edit with unapproved candidates.

---

# 15. COLOR AND FINISH

Overall arc:
- SH01–03 late golden hour;
- SH04–06 sunset peak;
- SH07 transition;
- SH08 blue hour;
- SH09 refined night.

Apply restrained luxury grading:
- natural skin;
- warm highlights;
- deep but detailed navy/blue shadows;
- controlled gold;
- no orange-teal cliché;
- no oversaturated HDR;
- no crushed blacks.

---

# 16. END CARD

Default:
MAZAR MALL
Tomorrow Has a View.

Keep the final card elegant and readable for roughly 2+ seconds.

Do not add:
- fake contact details;
- prices;
- unverified claims;
- invented launch dates.

Logo treatment must remain clean and undistorted.

---

# 17. QUALITY GATES

Before final selection, reject:
- facade morphing;
- changing floor rhythm;
- warped balconies/windows;
- duplicated people;
- deformed hands;
- morphing coffee cup;
- unstable vehicles;
- fake text;
- logo mutation;
- fisheye distortion;
- camera jitter;
- fantasy skyline presented as exact site;
- neon/cyberpunk lighting;
- inconsistent sun direction.

Run the acceptance criteria in:
`docs/06_ACCEPTANCE_CRITERIA.md`

---

# 18. VERSIONING

Never overwrite final candidates.

Use:

`outputs/keyframes/SH01/v001.*`
`outputs/video/SH01/v001.*`
etc.

Maintain:

`production/status.json`

Statuses:
- PLANNED
- KEYFRAME_IN_PROGRESS
- KEYFRAME_APPROVED
- VIDEO_IN_PROGRESS
- CANDIDATES_READY
- SELECTED
- REJECTED
- BLOCKED
- FINAL

Record the exact selected candidate per shot.

---

# 19. HUMAN APPROVAL GATES

Do not interrupt for every technical choice.

Only request human approval when:
1. architecture references materially conflict;
2. exact site accuracy cannot be resolved;
3. Astra is unavailable;
4. Higgsfield access is unavailable;
5. a factual marketing claim requires confirmation;
6. music/license decision is needed;
7. final master is ready for presentation.

Otherwise continue autonomously.

---

# 20. FINAL DELIVERABLES

Target files:

`outputs/final/Mazar_Mall_60s_Client_Presentation_1080p.mp4`

If source quality supports genuine 4K:
`outputs/final/Mazar_Mall_60s_Client_Presentation_4K.mp4`

Also create:
- `outputs/final/contact_sheet.jpg`
- `outputs/final/final_shot_list.md`
- `outputs/final/generation_credits.md`
- `outputs/final/known_limitations.md`

Do not upscale a weak source merely to label it 4K.

---

# 21. FINAL REPORT

Return:

MAZAR MALL 60S CGI PRODUCTION REPORT

Branch:
Starting SHA:
Final SHA:

Astra:
AVAILABLE / UNAVAILABLE
Exact capability/model used:

Higgsfield:
CONNECTED / BLOCKED

Selected Higgsfield models:

Site plates:
PRESENT / ABSENT

Site match:
VERIFIED / SITE_MATCH_UNVERIFIED

SH01:
FINAL / BLOCKED
Selected candidate:

SH02:
FINAL / BLOCKED
Selected candidate:

SH03:
FINAL / BLOCKED
Selected candidate:

SH04:
FINAL / BLOCKED
Selected candidate:

SH05:
FINAL / BLOCKED
Selected candidate:

SH06:
FINAL / BLOCKED
Selected candidate:

SH07:
FINAL / BLOCKED
Selected candidate:

SH08:
FINAL / BLOCKED
Selected candidate:

SH09:
FINAL / BLOCKED
Selected candidate:

Architecture continuity:
PASS / FAIL

Floor 5 balcony accuracy:
PASS / FAIL

Character continuity:
PASS / FAIL

Lighting continuity:
PASS / FAIL

Camera stability:
PASS / FAIL

Edit:
PASS / FAIL

Audio:
PASS / PENDING / FAIL

Duration:
<seconds>

1080p master:
PASS / FAIL

4K master:
PASS / NOT PRODUCED / FAIL

Known limitations:

FINAL STATUS:
READY_FOR_CLIENT_PRESENTATION
or
NOT_READY

---

# FINAL OPERATING PRINCIPLE

The objective is not “make nine AI videos.”

The objective is:

**direct one coherent luxury architectural film in which every generated asset serves the same Mazar Mall, the same evening, the same architecture, and the same emotional story.**

Protect continuity above novelty.
Protect architectural truth above spectacle.
Make the client feel the future is already real.
