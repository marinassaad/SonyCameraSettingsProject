# Camera Configuration Project — Sony A6700

## For: Marina

This document describes a project to systematically configure your Sony A6700 camera so that you can walk into any shooting situation, turn a dial, and start shooting with confidence — without fumbling through menus.

This is the same process your uncle Nelson went through with his Lumix G9 cameras. The camera is different, the menus are different, but the photography principles are identical.

---

## What This Project Will Produce

By the end, you will have:

1. **A JSON configuration file** — the single source of truth for every setting on your camera. What's saved in each memory slot, what the global "set and forget" settings are, and why each choice was made.

2. **Printable field reference cards** — iPhone-sized laminated cards you carry in the field. The front tells you what to physically set up; the back explains why.

3. **A PWA (Progressive Web App)** — the same cards accessible on your iPhone, working offline. No app store needed.

4. **Deep understanding** — you won't just have settings. You'll understand WHY each parameter has that value, WHEN to change it in the field, and WHAT it affects in the photo.

---

## Your Gear

**Cameras:**
- **Sony A6700** (ILCE-6700) — 26MP APS-C, the camera you're configuring

**Lenses (in order of focal length):**
- **Sony E 11mm f/1.8** — ultra-wide prime (gift from Nelson). 16.5mm equivalent. Extremely fast f/1.8 for astrophotography, low-light interiors, dramatic wide scenes.
- **Sigma 10-18mm f/2.8 DC DN Contemporary** — ultra-wide zoom (15-27mm equivalent). Versatile for landscapes and architecture.
- **Sigma 18-50mm f/2.8 DC DN Contemporary** — standard zoom (27-75mm equivalent). Your everyday walk-around lens. Constant f/2.8 across the range.
- **Sony E 70-350mm f/4.5-6.3 G OSS** — telephoto zoom (105-525mm equivalent). Wildlife, birds, distant subjects.

**Coverage:** 10mm → 350mm (effectively 15mm → 525mm) with a small gap between 50mm and 70mm. Strong, balanced kit.

**Why the 11mm f/1.8 gift matters:** You already have the 10-18mm covering this focal range. The 11mm prime wins for **astrophotography**: f/1.8 vs f/2.8 means it gathers 2.25× more light, which lets you keep ISO lower or shutter shorter — critical for sharp stars.

**Image format:** RAW only (.ARW). Maximum editing flexibility. You'll edit in Lightroom/Capture One/similar.

---

## The Core Concept: Memory Recall Modes

Your Sony A6700 can memorize complete camera configurations and recall them instantly:

- **3 dial positions** (MR1, MR2, MR3) — turn the mode dial to recall. Stored permanently in the camera.
- **4 card slots** (M1–M4) — recalled via menu. Stored on the SD card (lost if you format the card — always keep a JSON backup).

**Total: 7 custom configurations.**

### What Gets Saved in a Memory Slot

Everything: exposure mode (A/S/M), aperture, shutter speed, ISO settings, autofocus mode, autofocus area, subject detection settings, drive mode (single/burst), white balance, image stabilization mode, metering, photo style — the entire camera state.

### What Does NOT Get Saved (Physical Actions)

Some things require your hands:
- **Which lens** is mounted
- **The focus mode switch** on the lens (AF/MF) — if applicable
- **The OSS switch** on the lens (stabilization ON/OFF)
- **Tripod** mounted or not

The field cards will remind you of these physical steps.

---

## Your 7 Scenarios

Below are your chosen scenarios, described in photography terms (not camera-menu language). You and Claude will translate these into specific Sony A6700 menu settings together.

### Tier 1 — Mode Dial (instant access)

These are your most-used scenarios. One click on the dial and you're ready.

#### MR1: Landscapes
- **What:** Vistas, mountains, waterfalls, forests, architecture, sweeping scenes
- **Lens:** Sigma 10-18mm f/2.8 (primary — versatile wide zoom), or 70-350mm for compressed distant shots
- **Approach:** Aperture Priority. You control depth of field.
- **Starting aperture:** f/8 (sweet spot — maximum sharpness, deep DoF)
- **ISO:** 100 (base ISO, cleanest image)
- **Autofocus:** Single-shot AF (AF-S), single area
- **Drive:** Single shot
- **Stabilization:** ON if handheld, OFF if on tripod
- **Why f/8?** Most lenses are sharpest at f/5.6-f/11. Going narrower (f/16+) causes diffraction blur. Going wider loses depth of field.

#### MR2: Wildlife
- **What:** Birds (perched or flying), mammals, reptiles — anything with animal behavior
- **Lens:** 70-350mm
- **Approach:** Manual exposure with Auto ISO. Lock the two critical variables (aperture and shutter), let ISO float.
- **Starting aperture:** f/6.3 (max aperture at 350mm on your lens)
- **Starting shutter speed:** 1/1000s. Enough for most perched or walking animals. In the field, dial UP to 1/2000-1/4000 for birds in flight or fast action.
- **ISO:** Auto, no upper limit. A noisy sharp photo beats a clean blurry one.
- **Autofocus:** Continuous AF (AF-C), Zone or Wide area, Bird/Animal subject recognition ON
- **Drive:** High-speed burst (Hi / Hi+)
- **Stabilization:** ON (Mode 2 if panning)
- **Why Manual + Auto ISO?** You need to guarantee BOTH enough DoF (aperture) AND frozen motion (shutter speed). ISO is the flexible variable.

#### MR3: General / Street
- **What:** Walk-around photography — markets, towns, travel, sightseeing, anything unplanned
- **Lens:** Sigma 18-50mm f/2.8 (primary — this is the "everyday" lens)
- **Approach:** Aperture Priority. The "pick up and shoot" mode.
- **Starting aperture:** f/5.6 (good all-around — sharp, versatile, decent DoF)
- **ISO:** Auto
- **Autofocus:** Single-shot AF (AF-S), Wide area with face detection
- **Drive:** Single shot
- **Stabilization:** ON
- **Why Aperture Priority?** Walk-around situations don't need fast shutter. Aperture is the creative decision (how much background blur). Let the camera handle the rest.

### Tier 2 — Card Slots (menu recall)

Recalled via menu. Slightly slower than the dial but still fast.

#### M1: Portrait / People
- **What:** Posed or candid photos of people
- **Lens:** Sigma 18-50mm f/2.8 at 50mm (best current option — constant f/2.8), or 70-350mm at 70mm for tighter framing
- **Approach:** Aperture Priority. Wide aperture for background blur (bokeh).
- **Starting aperture:** f/2.8 (with the 18-50mm) — widest available
- **ISO:** Auto
- **Autofocus:** AF-S with **Eye AF** ON (Human priority)
- **Drive:** Single shot
- **Stabilization:** ON
- **Future upgrade:** A dedicated fast portrait prime (Sigma 56mm f/1.4 ~$400, or Sony 50mm f/1.8 ~$250) would give stronger bokeh and better low-light. The 18-50mm at f/2.8 is already very capable though.

#### M2: Low Light / Dusk-Dawn
- **What:** Handheld shooting at golden/blue hour, indoors, evening scenes — enough light to see, not enough for fast shutter speeds
- **Lens:** 11mm f/1.8 (widest + fastest), or Sigma 18-50mm f/2.8 (everyday low light), or 10-18mm f/2.8 (wide scenes)
- **Approach:** Aperture Priority, wide open, high ISO ceiling
- **Starting aperture:** Widest of whatever lens is mounted (f/1.8 with 11mm, f/2.8 with Sigmas, f/4.5 with 70-350mm at 70mm)
- **Min shutter speed:** 1/60s (handheld limit)
- **ISO:** Auto, no upper limit
- **Autofocus:** AF-S, Wide area
- **Stabilization:** ON
- **Why wide open?** In low light, gathering maximum light is priority #1. Depth of field becomes secondary.

#### M3: Night Sky / Stars ⭐
- **What:** Milky Way, star fields, night landscapes
- **Lens:** 11mm f/1.8 strongly preferred (gathers 2.25× more light than the Sigma 10-18mm f/2.8). The 10-18mm is a backup option if you want a different focal length.
- **Tripod:** REQUIRED
- **Approach:** Full Manual. Every parameter chosen by you.
- **Aperture:** f/1.8 (wide open — gather all available starlight)
- **Shutter speed:** 20 seconds ("500 rule": 500 / 11mm = 45s max, but 20s is safer for sharp stars)
- **ISO:** 3200 (starting point — adjust 1600-6400 based on sky darkness)
- **Focus:** **Manual, set to infinity** — zoom in on a bright star in live view, adjust until pinpoint sharp, then don't touch
- **White balance:** Daylight (or ~3800K) — gives neutral stars, not orange
- **Long Exposure NR:** OFF (would block camera for 20+ seconds between shots)
- **Stabilization:** OFF (on tripod — IS causes drift)
- **Drive:** 2-second timer (avoid shake from pressing the shutter button)
- **Why these values?** At f/1.8 for 20s at ISO 3200, you gather enough light for the Milky Way while stars stay as points. Longer than 20s at 11mm and stars start trailing.

#### M4: Video — Wildlife
- **What:** Moving animal/bird video footage
- **Lens:** 70-350mm
- **Approach:** Manual video, prioritize smooth footage
- **Record format:** 4K 30p or 60p (your preference — 60p gives slow-motion option)
- **Shutter speed:** 1/60s (180° shutter rule for 30p) or 1/125s (for 60p)
- **Aperture:** f/6.3 (max at 350mm)
- **ISO:** Auto, no upper limit
- **Autofocus:** AF-C with Bird/Animal subject recognition
- **Stabilization:** ON with **Active SteadyShot** for extra smoothness
- **Picture Profile:** Standard (or S-Log3 if you want to color-grade in post)
- **Why different from MR2 (photo wildlife)?** Video has different shutter speed needs (match to frame rate), benefits from stronger stabilization, and needs video-specific AF settings.

---

## Global "Set and Forget" Settings

Settings you configure ONCE and never touch. They apply across all modes.

### Image Quality
- **File format:** RAW only (.ARW)
- **Compression:** Lossless Compressed (smaller files, no quality loss) or Uncompressed
- **Aspect ratio:** 3:2 (native sensor ratio)

### Display
- **Grid lines:** Rule of thirds (helps composition)
- **Histogram:** ON (learn to read it — it never lies about exposure)
- **Level gauge:** ON (keeps horizons straight)
- **Peaking (MF assist):** ON, Red, Medium level (critical for astro focus)

### Autofocus
- **Subject recognition:** ON globally (individual modes override)
- **AF assist illuminator:** ON
- **Eye priority:** ON

### Playback
- **Auto review:** 2 seconds

### Custom Buttons (initial assignments — refine with Claude)
- **C1:** ISO
- **C2:** White Balance
- **C3:** Focus Mode toggle (AF-S / AF-C / MF)
- **AEL:** Eye AF (hold to track eyes)

---

## The Process — How to Work With Claude

### Step 1: Get the Camera Manual

1. Go to **https://helpguide.sony.net/ilc/2320/v1/en/** (Sony A6700 online help guide) — or search "Sony A6700 help guide PDF"
2. Download the full PDF manual for the ILCE-6700
3. Check your firmware: **Menu → Setup → Version** on the camera
4. Save the PDF in your project folder under `reference/manuals/`
5. Ask Claude to read it — this gives Claude the exact menu structure for YOUR camera

### Step 2: Set Up the Project

Create a GitHub repository and this folder structure:

```
your-project/
├── data/                  # Single source of truth
│   └── camera-config-a6700.json
├── docs/                  # PWA (GitHub Pages)
├── tools/                 # Card generators, utilities
├── guides/                # Written guides, walkthroughs
├── reference/             # Manuals (gitignored — too large)
│   └── manuals/
├── output/                # Generated PDFs
└── review/                # Sample photos for analysis (gitignored)
```

Claude will help you set this up.

### Step 3: Global Settings ("Set and Forget")

Go through the camera menu systematically with Claude:
1. Claude reads the manual and identifies every menu item
2. For each setting, discuss: What does it do? Set-and-forget or per-scenario?
3. Configure the set-and-forget ones on the camera
4. Document everything in the JSON file with rationale

**This is the longest step.** Takes time, but you only do it once.

### Step 4: Program the 7 Scenarios

For each memory slot (MR1, MR2, MR3, M1, M2, M3, M4):
1. Set all values on the camera manually
2. Save: **Menu → Shooting → Camera Set. Memory** (select slot)
3. Test by recalling and verifying

### Step 5: Create Field Reference Cards

Claude builds `field-cards.json`, a Python script generates printable PDF cards.

### Step 6: Build the iPhone App (PWA)

Claude creates an HTML app that reads from the JSON. Enable GitHub Pages, add to home screen in Safari, done.

### Step 7: Field Test and Iterate

**Most important step.** Shoot, come back, tell Claude what didn't work:
- "Birds were blurry at 1/1000 — need faster"
- "Landscapes at f/8 weren't sharp enough in the corners"
- "Night sky ISO 3200 was too noisy"

Claude updates the JSON, regenerates cards, updates the app. Iterate until every mode feels right.

---

## Key Principles

1. **Understand before configuring.** For every value, ask "why?" until you understand. Nelson spent hours debating every parameter with Claude. That's the process.

2. **Settings are a starting point, not a religion.** The saved mode gets you 80% there. The last 20% is adjusting dials in the field.

3. **Physical setup is as important as software.** Perfect mode + wrong lens switch = bad photo.

4. **Test in real conditions.** Indoor testing is mostly useless. Go outside, find subjects, shoot, review, adjust.

5. **Start with your biggest interest.** Wildlife is probably it — get MR2 (Wildlife) dialed in first, then expand.

6. **The JSON is your single source of truth.** Change a camera setting? Update the JSON. Forget a value? Read the JSON. Everything else (cards, app) regenerates from the JSON.

---

## Getting Started

Open Claude Code (or Claude in your IDE), paste this document, and say:

> "I'm Marina, starting a Sony A6700 configuration project. My uncle Nelson did the same with his Lumix G9 cameras. Here's the project description he wrote for me. I understand the exposure triangle and have shot in Manual mode before. Let's begin with Step 1 — finding and downloading the camera manual."

Claude will guide you from there. Have fun and good shooting!

---

*This project template was created by Nelson Salgado based on his experience configuring two Lumix G9 cameras. The methodology is camera-agnostic — photography principles are universal. Reference project: https://github.com/nksalgado-proton/LumixCameraSettingsProject*
