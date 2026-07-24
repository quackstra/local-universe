# VRL Methodology — Value Retained Locally

> Converts "local economic activity" into "$/sec of leakage recaptured" — the unit the
> Radix community can compare ventures against. Souls: Community-Development Economist ×
> Market-Sizing Specialist. Accessed 2026-07-23.

## The leakage literature (sourced defaults)
- A dollar at a **local independent recirculates ~48%** locally (AMIBA latest ~52.9%); at a
  **chain, only ~13.6%**. Chain→local shift retains an extra **~34–39 pts** locally.
  [AMIBA Local Multiplier](https://amiba.net/local-multiplier/)
- NEF **LM3 / "Plugging the Leaks"**: local spend worth **3–5×** more to the community across
  the first three spending rounds. [NEF LM3](https://www.nefconsulting.com/what-we-do/evaluation-impact-assessment/local-multiplier-3/) · [Plugging the Leaks (PDF)](https://neweconomics.org/uploads/files/9215d0d00f79789377_cxm6bu0ue.pdf)

## Formula
```
VRL (annual $) = leakage_rate × addressable_spend × recapture_fraction
VRL ($/sec)    = VRL_annual ÷ 31,536,000
```

| Term | Default | Range | Basis |
|---|---|---|---|
| `leakage_rate` | 0.65 | 0.52–0.86 | share of a local $ that currently leaves (chain ~86% leaks) — AMIBA |
| `recapture_fraction` | 0.20 | 0.10–0.34 | share of the leak the platform can realistically plug |
| `addressable_spend` | per-tier | see tier_model | local consumer + SMB spend the venture addresses |

## Worked $/sec by tier (defaults)
| Tier | addressable_spend | VRL annual | **VRL $/sec** | Range $/sec |
|---|---|---|---|---|
| T1 | $25M | $3.3M | **~$0.10/s** | $0.03–$0.72 |
| T2 | $10B | $1.3B | **~$41/s** | $10–$290 |
| T3 | $550B | $71.5B | **~$2,270/s** | $570–$16,000 |

## Honesty note
The $/sec metric is rhetorically powerful but **dominated by two soft inputs** —
`addressable_spend` per capita and `recapture_fraction`. Treat **T3's ~$2,270/sec as a ceiling
narrative** and **T1's ~$0.10/sec as the defensible pilot number**. The El Zonte base rate warns
recapture sits toward the low bound early. The single biggest research gap in the whole study is a
primary-source measurement of local spend composition + realistic chain→local shift in one
candidate beachhead town.
