---
name: alchemy-healing-aging-pills
description: >-
  Formulates evidence-grounded healing and anti-aging pill recipes by
  synthesizing longevity research, senolytic science, and alchemical
  transformation stages. Use when the user asks for healing pills, aging
  pills, longevity elixirs, senolytic formulas, geroprotector recipes, or
  wants to transmute raw ingredients into a structured anti-aging regimen.
  Trigger with phrases like "make me a healing pill", "anti-aging elixir",
  "longevity formula", "senolytic recipe", or "aging pill".
---

# Alchemy Healing & Aging Pills

A skill that turns the user's request into a structured, evidence-grounded
pill recipe. It borrows three things from the top skills on GitHub:

1. **Magnum Opus stages** (HermeticOrmus/magnum-opus-skills) — the seven-stage
   transformation pipeline, adapted from software to biology.
2. **Cellular Senescence Agent** (FreedomIntelligence/OpenClaw-Medical-Skills)
   — senescence markers, SASP profiling, and senolytic drug targets.
3. **Longevity skills** (longevity-genie/longevity-skills) — aging research
   synthesis and evidence-weighted intervention review.

## The Seven Stages (Solve et Coagula)

| # | Stage | Operation | Pill meaning |
|---|---|---|---|
| 1 | Calcination | Burn what doesn't serve | Strip out harmful or redundant ingredients |
| 2 | Dissolution | Let understanding flow | Identify the core biological target (e.g. senescence, inflammation) |
| 3 | Separation | Gold from dross | Separate active compounds from fillers |
| 4 | Conjunction | Unite opposites | Combine synergistic compounds (e.g. dasatinib + quercetin) |
| 5 | Fermentation | Trial by failure | Stress-test the formula against contraindications |
| 6 | Distillation | Refine to wisdom | Extract the minimal effective dose and mechanism |
| 7 | Coagulation | Crystallize into form | Output the final recipe with dosing and warnings |

## Workflow

1. **Intake** — Capture the user's goal (healing, anti-aging, specific
   condition), age range, and any known conditions or medications.
2. **Calcination** — List candidate ingredients, then remove anything with
   poor evidence, high toxicity, or known interactions.
3. **Dissolution** — Name the biological target: cellular senescence, NAD+
   depletion, mTOR overactivation, chronic inflammation, oxidative stress.
4. **Separation** — For each remaining ingredient, state the active compound,
   its mechanism, and the evidence tier (in vitro / animal / human trial).
5. **Conjunction** — Pair ingredients that hit different pathways (e.g. a
   senolytic + an NAD+ booster + an antioxidant).
6. **Fermentation** — Run a contraindication check: drug interactions,
   pregnancy, liver/kidney load, sun sensitivity.
7. **Distillation** — Reduce to the smallest effective set with doses.
8. **Coagulation** — Emit the final recipe: name, ingredients with doses,
   timing, cycle, expected effect, and a disclaimer.

## Evidence Tiers

- **Tier 1** — Human clinical trials (e.g. dasatinib + quercetin, fisetin)
- **Tier 2** — Strong animal data (e.g. NMN, rapamycin in mice)
- **Tier 3** — In vitro or mechanistic only (many herbal compounds)
- **Tier 4** — Traditional use, no modern evidence

Prefer Tier 1 and 2. Flag Tier 3 and 4 explicitly.

## Senolytic Reference (from OpenClaw-Medical-Skills)

| Compound | Target | Status |
|---|---|---|
| Dasatinib | Src/tyrosine kinases | Human trials (with quercetin) |
| Quercetin | PI3K, serpins | Human trials (with dasatinib) |
| Fisetin | Multiple | Early human trials |
| Navitoclax | BCL-2/BCL-xL | Trials |
| UBX1325 | BCL-xL | Phase 2 (macular) |

## Senescence Markers to Consider

- Cell cycle: p16INK4a, p21CIP1, p53
- SA-β-gal: GLB1
- SASP: IL-6, IL-8, MMP3, PAI-1
- DNA damage: γH2AX, 53BP1

## Output Format

Always end with:

```
Pill: <name>
Goal: <one line>
Ingredients:
  - <compound> — <dose> — <mechanism> — <evidence tier>
Timing: <when to take>
Cycle: <days on / days off>
Expected effect: <one line>
Warnings: <contraindications>
Disclaimer: Not medical advice. Consult a physician before use.
```

## Disclaimer

This skill produces informational recipes grounded in published research.
It is not medical advice, a diagnosis, or a treatment plan. All formulas
require physician review before any real-world use.
