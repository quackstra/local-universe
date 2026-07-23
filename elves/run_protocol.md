# Local-Universe — Standard Elf Run Protocol

> One autonomous research run = Steps A–E in order. Re-read after any context
> compaction. Adapted from the Universe-of-Finance protocol; the unit of work is
> a **LoFi venture measured at three adoption tiers**, not a present-day TPS category.

## Inside-Out Prioritisation (by prize size, not present volume)

Because Local-Universe measures a *counterfactual* prize, "the centre" is the
venture with the **largest addressable prize × best precedent**, not the largest
current transaction volume.

```
        ┌─ Movement tier (T3, 1% of local economies)
   ┌────┤
   │    └─ Regional tier (T2) ─┐
   │                           └─ Beachhead tier (T1)
   └─ THE CENTRE: biggest-prize, best-precedented venture (SRU, then CCS)
```

Expand outward: **by prize** (SRU/CCS → DAO-JOBS/Business Ops → SBI/RUBIS),
**by tier** (T1 → T2 → T3), **by lens** (TPS/TTR base numbers first, then MEST
compression and RVC once the base exists).

## Research Capsules

Atomic output = **one lens measured for one venture at the three tiers**, with
finding + sources + methodology + confidence + full calculations. Examples:
- "SRU — TTR-Local (residential rental-equity addressable stock), T1/T2/T3"
- "CCS — TPS-Created from local-currency velocity, T1/T2/T3"
- "SRU — MEST compression vs transfer-agent + escrow rails"
- "SBI — RVC (XRD fees + Confidence-Farm TVL), T2/T3"

A capsule is complete when it has a T1/T2/T3 range, a confidence tag, cited
sources, shown calculations (inline or in `workings/`), and passes validation.

## Standard Run Steps

### A · Orient
1. Read `notes/last_session.md` (skip on first run).
2. Read `notes/research_agenda.md` — the priority queue.
3. `./run.sh scout` — refresh the venture/category backlog.
4. Check `analysis/README.md` for what's done. Plan capsule selection inside-out.

### B · Research — produce capsules (target 48+)
For each venture in prize-priority order:
- If no methodology exists, design it (Architect: adoption-tier model + unit economics).
- Staff the capsule via the Bureau (reuse UoF souls + the LoFi roster).
- Collect data, compute each applicable lens at T1/T2/T3, cite sources.
- Write to `analysis/<sector>/<venture>/REPORT.md` + `data.json`; charts where useful.
- Run validation gates; commit the capsule (`[LU] <venture>: ...`).
Cross-pollinate: a source found for SRU that also sizes DAO-JOBS gets noted.

### C · Taxonomy review
After the 48 floor: missing ventures? split/merge? (See TAXONOMY.md open questions —
esp. SBI-vs-RUBIS separation, a possible V7 receivables venture.) Log to
`notes/taxonomy_changes.md`.

### D · Retrospective
Stale tiers, cross-venture double-counting (does SRU rent overlap CCS transactions?),
confidence upgrades, methodology fixes. Fix quick wins; queue the rest.

### E · Session end
Write `notes/last_session.md` (capsules produced, ventures researched, key findings,
taxonomy changes, unfinished work) and update `notes/research_agenda.md` (next
priority queue). Commit both `[LU] session-notes:`.

## Supporting-file layout
```
analysis/<sector>/<venture>/
├── REPORT.md      # reader-facing, every number hyperlinked, T1/T2/T3 ranges
├── data.json      # structured, per-lens per-tier, with source URLs
├── charts/
└── workings/      # calculations.md, source_notes.md, assumptions.md
```

## Citation & confidence standards
Same as UoF: every number links to a primary-preferred, dated source; derived
numbers show the math inline or in `workings/`; conflicting sources → report the
range and explain. Counterfactual assumptions (adoption %, velocity, leakage
rate) are documented explicitly in `workings/assumptions.md` — they are the main
source of uncertainty and must never be buried.
