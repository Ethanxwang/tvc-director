# TVC Director

[中文版](README.md)

From product brief to cinematic TVC keyframes — your AI advertising creative director.

A skill that turns your AI agent into a **TVC Advertising Creative Director**, handling the complete creative pipeline for television commercials and brand advertising: from a product brief to production-ready **Nano Banana Pro** keyframe prompts and **Seedance** Multi-Phase video scripts.

## Key Features

- **End-to-end creative pipeline** — From a one-line brief to deliverable storyboard prompts and video scripts, fully AI-driven
- **8 TVC narrative models** — Problem-solution, cinematic product breakdown, brand world crosscut, and more
- **Cinematic visual system** — 5 art style presets (A-E), 12 scene types, per-second camera choreography
- **Product + brand world dual narrative** — Not just product close-ups, but crosscut storytelling in real-world scenes
- **Copy-paste ready** — Output prompts work directly in Nano Banana Pro / Seedance with no rework needed

## Demo

### Car TVC — Cinematic Product Breakdown

https://github.com/user-attachments/assets/541055ed-d716-4087-86e2-a27d375282ed

### Perfume TVC — Brand World Crosscut

https://github.com/user-attachments/assets/df2d51af-acc2-4f34-a228-8b35ea754345

## Quick Start: Making a Car TVC

A real end-to-end example — from a reference photo to a 15-second commercial.

### Step 1 — Provide a reference image + one-line brief

> "Make a 15-second TVC for this silver sedan"

<img src="https://github.com/user-attachments/assets/f6bd8778-9971-436a-bf8f-11e675a5e4fb" width="400" alt="Reference: silver sedan" />

The AI enters the full creative pipeline: brief analysis → creative concept → art style → asset generation → storyboard + video script.

### Step 2 — AI generates multiview prompts → Nano Banana Pro renders

The AI outputs product multiview prompts. Copy to Nano Banana Pro (edit mode, pass in the reference image) to get standardized multi-angle product shots:

<img src="https://github.com/user-attachments/assets/9d97df38-79f1-4a6a-a6bb-0fdbd731faca" width="600" alt="Product multiview" />

### Step 3 — AI generates 3×3 storyboard prompts → Nano Banana Pro renders

The AI outputs a 3×3 multi-grid storyboard prompt (with per-panel composition, lighting, and camera direction). Copy to Nano Banana Pro (edit mode, pass in multiview + environment images):

<img src="https://github.com/user-attachments/assets/1ca54c8a-e1c2-4a13-8e67-461ea327f2ab" width="600" alt="3×3 storyboard grid" />

### Step 4 — AI generates Multi-Phase video script → Seedance renders video

The AI outputs a Seedance Multi-Phase video script (5 phases / 15s). Use the storyboard grid as the first frame + product multiview as the anchor, dual-image input to Seedance for the final video.

### Output Summary

| Deliverable | Tool | Purpose |
|-------------|------|---------|
| Product multiview | Nano Banana Pro (edit) | Product anchor for subsequent steps |
| 3×3 storyboard grid | Nano Banana Pro (edit) | Video first frame + visual QA |
| Multi-Phase video script | Seedance | Generate 15s final video |
| Creative brief document | — | Full creative brief for archival |

## Design Philosophy

Traditional AI-generated ads tend to be an endless loop of "product + black background + rotation." TVC Director is different:

- **Narrative-driven, not template-filling** — Determine the narrative model and creative direction first, then generate visuals
- **Dual-world crosscutting** — Product close-ups interweave with brand world scenes, telling stories like a real TVC
- **Per-second camera design** — Every storyboard panel has explicit shot size, angle, lighting, and transition logic
- **Progressive human-AI collaboration** — Intervene and adjust at every phase; not a black-box one-click generator

## Two Core Capabilities

### 1. Cinematic Product Breakdown

Not just 360° rotation — multi-phase product micro-films with:

- Component disassembly/assembly animations (floating parts, exploded views, snap-back)
- Feature visualization (screen lighting up, tracking boxes, digits ticking 00:00:00→04:00:00, sensor glow)
- Material macro shots (brushed metal, glass refraction, carbon fiber weave)
- Precise per-second camera choreography (ultra-slow reveal → explosive rotation → macro dive)
- Cinematic studio lighting (low-key, side light silhouettes, light flowing with rotation)

### 2. Brand World Crosscut

Products don't live on black backgrounds — they live in their brand world:

- Outdoor cameras → skydiving, diving, skiing, climbing
- Luxury watches → racing, sailing, formal events
- Skincare → morning rituals, natural springs, sunrise
- Sportswear → urban parkour, marathon, rain-soaked streets

TVC crosscuts between "product close-ups" and "brand world usage scenes", connected via match cuts (skier spinning → product spinning).

## Installation

### Cursor

```bash
git clone https://github.com/Ethanxwang/tvc-director.git ~/.cursor/skills/tvc-director
```

### Claude Code

```bash
git clone https://github.com/Ethanxwang/tvc-director.git ~/.claude/skills/tvc-director
```

## How It Works

```
"帮我做一条户外相机的30秒TVC"
        ↓
  Phase 0: Mode Detection
  Phase 1: TVC Brief Analysis (product/duration)
  Phase 2: TVC Creative Concept (2-3 directions → pick → full brief)
  Phase 3: Art Style Confirmation (A-E)
  Phase 4: Asset Prompts (product multiview, materials, brand world environments)
  Phase 5: Storyboard Prompts + Seedance Multi-Phase Video Scripts
  Phase 6: Iterative Refinement
  Phase 7: Deliverable Organization
        ↓
  Copy-paste-ready Nano Banana Pro prompts,
  Seedance video scripts & creative docs
```

## Entry Modes

| Mode | Trigger | Description |
|------|---------|-------------|
| **A: Full TVC Pipeline** | "帮我做一条xx产品广告" | Brief → Concept → Style → Assets → Keyframes → Package |
| **B: Quick Asset/Prompt** | "帮我做一个产品 Hero Shot" | Skip creative phase, go to asset or keyframe generation |
| **C: Storyboard** | Provide a TVC script/storyboard | Style → Assets → Convert storyboard to keyframes |
| **D: Iteration** | "这张产品图xx不对" | Fix and regenerate specific assets or keyframes |

## TVC Narrative Models

| Model | Name | Core Logic |
|-------|------|-----------|
| A | Problem-Solution | Pain point → product saves the day |
| B | Cinematic Product Breakdown | Multi-phase micro-film revealing USPs |
| C | Brand World Crosscut | Scene ↔ product close-up crosscutting |
| D | Lifestyle Integration | Product woven into aspirational lifestyle |
| E | Emotional Anchor | Emotional story, product as carrier |
| F | Montage Reveal | Visual spectacle → product reveal |
| G | Before/After | Before/after strong contrast |
| H | Brand Anthem | Values-driven, product closes |

## Deliverables

```
my-tvc-project/
├── concept.md                      # TVC creative brief
├── storyboard.md                   # Storyboard (if applicable)
│
├── assets/                         # Product asset prompts (Nano Banana Pro)
│   └── prompts/
│       ├── product-multiview.md
│       ├── product-detail-01.md
│       ├── env-01-extreme-sports.md
│       └── ...
│
├── keyframes/                      # Storyboard keyframe prompts (Nano Banana Pro)
│   └── prompts/
│       ├── grid-01-brand-world.md
│       ├── grid-02-product-world.md
│       ├── endframe.md
│       └── ...
│
└── video-scripts/                  # Multi-Phase video prompts (Seedance)
    ├── segment-01-brand-world.md
    ├── segment-02-product-breakdown.md
    └── ...
```

## How to Use Deliverables

1. **Product multiview** — Copy prompts from `assets/prompts/product-multiview.md` into Nano Banana Pro, edit mode, pass in reference image
2. **Storyboard keyframes** — Copy prompts from `keyframes/prompts/` into Nano Banana Pro, edit mode, pass in multiview + environment images
3. **Video scripts** — Use Multi-Phase scripts from `video-scripts/` with the storyboard grid as first frame + product multiview, input to Seedance

## Knowledge Base Architecture

| Role | File | Content | Loading |
|------|------|---------|---------|
| Core Flow | `SKILL.md` | Entry detection, phase transitions, output specs | Always loaded |
| Creative Director | `creative.md` | 8 TVC narrative models, visual aesthetics, creative brief template + 2 examples | Phase 2 (creative concept) |
| Prompt Engineer | `prompts.md` | 6-layer prompt structure, art style library (A-E), 12 TVC scene types, composition paradigms | Phase 3-4 (style + assets) |
| Production | `production.md` | Multi-grid storyboard, video prompt syntax, cinematic product breakdown, brand world shots | Phase 5 (storyboard) |
| Output & Iteration | `infra.md` | Output format templates, iteration guide (11 failure modes) | Phase 4-7 (on demand) |

## License

MIT
