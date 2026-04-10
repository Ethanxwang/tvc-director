# TVC Director

From product brief to cinematic TVC keyframes — your AI advertising creative director.

A skill that turns your AI agent into a **TVC Advertising Creative Director**, handling the complete creative pipeline for television commercials and brand advertising: from a product brief to production-ready Nano Banana Pro keyframe prompts and Seedance Multi-Phase video scripts.

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

## What It Does

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

## Installation

### Cursor

```bash
git clone https://github.com/Ethanxwang/tvc-director.git ~/.cursor/skills/tvc-director
```

### Claude Code

```bash
git clone https://github.com/Ethanxwang/tvc-director.git ~/.claude/skills/tvc-director
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

## Knowledge Base

Knowledge is organized into 4 role-based reference files:

| Role | File | Content | Phase |
|------|------|---------|-------|
| Creative Director | `creative.md` | 8 TVC narrative models, visual aesthetics (metaphor, color psychology, brand color, product aesthetics, brand world visual language), creative brief template + 2 examples | Phase 2 |
| Prompt Engineer | `prompts.md` | 6-layer prompt structure, art style library (A-E), 12 TVC scene types, TVC composition paradigms, visual design checklist | Phase 3-4 |
| Production | `production.md` | Multi-grid storyboard, video prompt syntax, cinematic product breakdown, brand world shots, match cut, TVC duration templates | Phase 5 |
| Output & Iteration | `infra.md` | Output format templates, iteration guide (11 failure modes) | Phase 4-5-6-7 |

## Relationship to aigc-director

This skill is **distilled from** [aigc-director](https://github.com/Ethanxwang/aigc-director) — sharing the same Nano Banana Pro prompt engineering layer and art style library, but with the creative framework entirely rebuilt for TVC advertising:

| Layer | aigc-director | tvc-director |
|-------|--------------|-------------|
| Prompt Engine | Nano Banana Pro | Nano Banana Pro (same) |
| Art Styles | A-E library | A-E library (same) |
| Narrative Models | 11 general models | 8 TVC-specific models |
| Scene Types | 8 creative scene types | 12 TVC scene types (product/brand/crosscut) |
| Core Capability | Visual storytelling | Product cinematography + Brand world integration |
| Video Prompts | General format | Multi-Phase format with product state changes |

## License

MIT
