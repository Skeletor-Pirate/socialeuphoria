# Social Euphoria // HopShop Design System Replication

The web portal for **Social Euphoria** (Dehradun, Uttarakhand, India) has been completely redesigned to replicate the exact architecture, aesthetic, and interaction model of **[hopshop.app](https://hopshop.app)**, re-skinned with the authentic story, imagery, sound curves, and curation of **Social Euphoria** founded by **Abhay Rawat**.

---

## 1. Visual Identity & Color System (HopShop Palette)

| Token | Hex | Role |
| :--- | :--- | :--- |
| `--hs-sand` | `#DACDB1` | Vintage Dotted Matrix Canvas Background |
| `--hs-linen` | `#EDE4D0` | Warm Textured Linen Paper |
| `--hs-paper` | `#FFFDF7` | Card Containers & Ticket Inserts |
| `--hs-ink` | `#1A1410` | Primary Typography & Outlines |
| `--hs-brick` | `#A3281C` | Primary Accent / Step 01 / Attention Slabs |
| `--hs-butter`| `#F4D95B` | Mustard Yellow / Step 03 / CTAs & Highlights |
| `--hs-lagoon`| `#5E9C95` | Vintage Teal / Step 02 / Approval Badges |
| `--hs-dusk`  | `#5F7FA0` | Slate Blue / Step 04 / Gate Badges |
| `--hs-oxblood`| `#3A0A0A` | Deep Wine / Status Portal Card Container |
| `--hs-coal`  | `#141211` | Brutalist Black Footer & Step 05 |
| `--hs-terracotta`| `#D9822B` | Event Page Modal Container (`hopshop.app/e/...`) |

---

## 2. Replicated Sections & Architecture

### I. Top Navigation
- Chunky brandmark for **Social Euphoria** with custom SVG icon.
- Nav items (`HOME`, `WHAT'S ON`, `HOW IT WORKS`, `THE FORMULA`, `CHECK STATUS`, `35MM VAULT`) with animated color underline bars (`#A3281C`, `#F4D95B`, `#5E9C95`, `#5F7FA0`).
- Pill action button: `REQUEST INVITE ↗`.

### II. Hero Section (`hopshop.app` Hero)
- Dotted matrix background canvas (`radial-gradient` with 24px pitch) and yellow SVG gridline vector.
- Curated header box: `SOCIAL EUPHORIA · INVITE AND ACCESS` · `CURATED MOUNTAIN ROOMS` · `STRICT GATE LOCK 21:00`.
- Monumental cutout display typography: **SOCIAL EUPHORIA** in `Anton` / `Syne`.
- Subtitle: *"CURATING HELL TO HAVE FUN — DEHRADUN"*.
- **Interactive Spherical Photo Cluster**: Orbiting collage of real party photographs (`sunset_real_1.jpg`, `afterdark_real_2.jpg`, `h2oli_real_2.jpg`, `cameraroll_3.jpg`, `founder.jpg`, `gallery_1.jpg`) with center `DOON 138 BPM` badge.
- Coordinate badge: `[ 30.3165° N, 78.0322° E ] · PRIVATE HIMALAYAN ESTATES`.
- Bouncing `SCROLL TO ENTER ↓` indicator.

### III. What’s On (`hs-float-grid`)
- Section heading with red accent slab mask: `WHAT’S [ ON ]`.
- Staggered floating 3:4 poster tiles for all 5 core editions + founder curation dossier:
  1. **Sunset Soirées Vol. III** (Himalayan Villa / Afro-House & Melodic Techno)
  2. **Sin City Nocturne** (Secret Industrial Bunker / 138 BPM Techno & Acid)
  3. **H²OLI Color Rave** (Estate Poolside / Organic Color Cannons & Heavy Bass)
  4. **The White Lotus Gala** (Private Cliffside Resort / All-White Masquerade NYE)
  5. **Project X Himalayan Lock-In** (Undisclosed Mountain Retreat / 8-Hour Session)
  6. **The Doon Protocol** (Curated by Abhay Rawat / Architect’s Note)
- Click any card to launch the **HopShop Event Detail Overlay** (`hopshop.app/e/...`) with 3D tilted poster, date, time, venue, and `Request Invite for Dehradun ↗`.

### IV. How It Works (`hopshop.app/how-it-works`)
- Header: `FROM REQUEST TO THE EVENT` with ghost `PROCESS` watermark.
- Wavy SVG connecting thread.
- 5 color-coded vintage ticket blocks:
  - **01 REGISTER** (`#A3281C` Brick Red): 1-minute invite application.
  - **02 VETTED / WAITLIST** (`#5E9C95` Teal): Batch committee reviews.
  - **03 PASS ISSUED** (`#F4D95B` Butter): Holographic QR pass in inbox/wallet.
  - **04 [ SCANNED AT GATE ]** (`#5F7FA0` Slate Blue): 21:00 absolute gate lock.
  - **05 THE NIGHT IS KEPT** (`#141211` Charcoal): Exclusive 35mm Vault dump.

### V. The Formula (`hs-thesis`)
- Sticky left column: `THE FORMULA` with step progress tracks (`01 THE CROWD`, `02 THE RHYTHM`, `03 THE SANCTUARY`).
- Right column word reveals:
  - *"The right crowd. A little curation. A very good time."*
  - *"Good music. Better vibes."*
  - *"Come by invitation. Leave with a story and some new friends."*

### VI. Check Your Status (`hopshop.app/status`)
- Centered header: `CHECK YOUR STATUS`.
- Deep oxblood card (`#3A0A0A`) with email/phone search input.
- Real-time status response with live verified dossier badge (`SE-2026-9842X`), guest identity, gate assignment, and procedural QR code pass.
- One-click `Download Pass PNG ↗` for Instagram Stories.

### VII. The 35mm Vault
- Unfiltered disposable flash roll dump featuring analog photos from past events.
- Full-screen lightbox viewer.

### VIII. Brutalist Footer
- Coal black bar (`#141211`).
- Social Euphoria brandmark, links (`HOW IT WORKS`, `CHECK STATUS`, `INSTAGRAM`).
- Copyright: `© 2026 Social Euphoria. All rights reserved.`
- Signature tagline: `DM us on Instagram. That’s where we live.`

---

## 3. Local Verification

The site is served locally on port `4321`:
```bash
python -m http.server 4321 --directory .\socialeuphoria
```
Open **`http://localhost:4321`** in any desktop or mobile browser.
Playwright verification confirmed **0 console errors** and **0 page exceptions** across both 1440×900 and 390×844 viewports.
