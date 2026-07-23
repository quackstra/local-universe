# Local-Universe — Research Brief

> **The size-of-prize study for LoFi on Radix.** How much new economic
> activity — measured in the language the Radix community already speaks
> (TPS, MEST, tokenized resources, network value) — would the full
> **ScryptDole + Local Stack** thesis create if built and adopted, and
> **which single next increment** gives the Radix community the best
> ROI / net-impact per unit of build effort?

Sister project to [Universe of Finance](../universe-of-finance) — it inherits
the same Scout→Architect→Elves→Publish pipeline, the same souls/Bureau engine,
and two of its headline lenses (MEST, TTR). Source theses live in [`sources/`](sources/).

---

## The two deliverables

1. **The Prize Map** — the total addressable prize of the whole LoFi stack,
   expressed as *net-new* Radix-native activity across the lenses below, at
   three adoption tiers (Beachhead / Regional / Movement).
2. **The Increment Ranking** — a weighted 0–100 score of the six LoFi ventures,
   answering: *if the Radix community builds exactly one thing next, which one
   returns the most impact per unit of effort?*

Everything else in this repo is the audit trail for those two artifacts.

---

## What makes this different from Universe of Finance

UoF is **descriptive** — it counts financial activity that already happens on
Earth. Local-Universe is **counterfactual / prescriptive** — it measures demand
that *does not yet exist on any ledger* and asks what it would be worth if the
Local Stack routed it onto Radix. That means:

- Every number is a **projection under an explicit adoption tier**, never a
  present-day measurement. Point estimates are banned; every capsule reports a
  range across the three tiers.
- The unit of analysis is a **LoFi venture** (SRU, CCS, …), not a transaction
  category. Each venture is decomposed into its measurable economic events.
- "Size of prize" is only persuasive to the Radix community if it lands in
  **Radix terms** — so we add a network-capture lens (RVC) the finance
  universe never needed.

---

## The lenses (metric framework)

Local-Universe reports **five lenses**. Two are inherited from UoF; three are
coined here. Each venture is scored on each lens at each adoption tier.

### 1. TPS-Created — *the Big Number* (inherited, re-pointed)
Net-new on-ledger transactions/sec the full stack generates. Bottom-up per
venture from its atomic economic events:
- **SRU** → rent payments × households × per-payment equity-accrual events
- **CCS** → local-currency transactions (velocity × float, BerkShares-calibrated)
- **RUBIS / SBI** → monthly mint + redemption events per enrolled capita
- **Business Ops** → on-ledger payroll / inventory / royalty-split events
- **DAO–JOBS** → governance votes + equity-distribution events

### 2. MEST — Mutual Economic State Transitions (inherited, *inverted*)
UoF's insight: a legacy card swipe fires ~7 MESTs; crypto fires 60–80% fewer.
For Local-Universe the prize is **dual**:
- **(a) new MEST captured** — economic events that today happen off-ledger (or
  don't happen at all) and would become atomic on Radix; and
- **(b) MEST compression** — the state-transition *savings* vs the legacy rails
  each venture displaces (escrow agents, transfer agents, cap-table admins,
  clearing legs). This is the quantitative core of the *"why Radix specifically"*
  argument: atomic composability collapses the 7.4× legacy multiplier to ~1×.

### 3. TTR-Local — Tokenizable Resources, LoFi-scoped (inherited, scoped)
The slice of UoF's ~$890T / ~170B-item tokenizable universe that the Local
Stack *specifically* unlocks: residential rental equity, SMB / local-business
equity, complementary-currency float, community UBI units, local receivables.
Usually the largest raw prize number; anchors the "why this matters" headline.

### 4. VRL — Value Retained Locally *(coined here)*
$/sec of economic leakage **recaptured** by the community. The Local Stack's
entire thesis (per Stoller/BIG) is fighting extraction; VRL is the number that
proves it. This is the **net-impact-for-communities** axis — the moral case,
quantified. Method: leakage-rate × local GDP × recapture-fraction per venture.

### 5. RVC — Radix Value Capture *(coined here)*
The network's own cut, in Radix terms — the literal answer to *"why should the
**Radix community** care?"*: XRD transaction fees + component **royalties** to
early blueprint builders + net-new **active accounts** + **TVL** the stack would
drive. Converts the whole prize into the metrics an XRD holder and a Radix dev
actually optimize for.

> Coined-metric discipline (house style): each universe invents memorable,
> defensible sub-metrics (UoF→MEST/TTR, Frynance→MUSHT, Onion→VOPS/GOVI).
> VRL and RVC are ours. If a sixth is needed it must be nameable and computable.

---

## Adoption tiers (mandatory for every capsule)

Because the prize is counterfactual, every number is reported at three tiers —
this replaces UoF's "three projection scenarios" rule:

| Tier | Name | Scale | Anchor |
|------|------|-------|--------|
| **T1** | Beachhead | 1 flagship town, ~3–10k people | El Zonte / "Bitcoin Beach" |
| **T2** | Regional | 100–1,000 communities | BerkShares network scale |
| **T3** | Movement | ~1% of global local economies | Stoller-scale structural shift |

A capsule without a T1/T2/T3 range is incomplete.

---

## The Increment Ranking rubric (deliverable #2)

Each of the six ventures scored 0–100, weighted (scoring-over-pass/fail, house
rule). Proposed weights — **open for Ferg's calibration**:

| Criterion | Weight | Measures |
|-----------|:------:|----------|
| Prize size | 0.25 | TTR-Local + TPS-Created + VRL at T2 |
| Build feasibility on Radix *today* | 0.20 | blueprint complexity, post-Babylon readiness |
| Radix-fit / composability leverage | 0.15 | does it *uniquely* need atomic composability? |
| Adoption velocity | 0.20 | time-to-first-real-user; existing off-chain demand |
| Regulatory risk (inverse) | 0.10 | securities / money-transmission exposure (JD lens) |
| Compounding | 0.10 | does shipping it unlock other stack pieces? |

**Prior (to be tested, not assumed):** SRU likely leads — largest TTR-Local
(real-estate equity), proven off-chain demand (Up&Up), immediate two-sided
benefit. CCS second (BerkShares precedent, high TPS, badge-gated composability
is a genuine Radix showcase). SBI/RUBIS highest ceiling but highest Sybil +
regulatory risk. The study exists to confirm or overturn this.

---

## How we tackle it (pipeline, reusing the machine)

- **Scout** seeds the venture taxonomy (6 ventures × measurement categories) →
  `scout/config.yaml`, `scout/backlog.yaml`.
- **Architect** designs one methodology per venture: adoption-tier model + unit
  economics + which lenses apply.
- **Elves** produce capsules **inside-out**: start at the biggest prize (SRU
  real-estate equity, CCS float), expand to smaller ventures, then to MEST-
  compression and RVC once the base TPS/TTR numbers exist.
- **Souls / Bureau** staff every capsule. Reuse UoF souls directly via
  `bureau ... --souls-dir ../universe-of-finance/souls` (`rwa-tokenisation-analyst`,
  `market-sizing-specialist`, `crypto-forensics-analyst`, `emerging-tech-forecaster`,
  `cbdc-digital-currency-researcher`, `gaming-economy-analyst`) **plus** the
  net-new LoFi roster in [`souls/RECRUITER.md`](souls/RECRUITER.md).
- **Publish** → `index.html` + the two deliverable maps in `reports/`.

## First-run target
One elf run = the T1/T2/T3 Prize Map for **SRU and CCS** (the two biggest,
best-precedented ventures) + a first-pass Increment Ranking with the other four
ventures at 🔴 confidence, to be upgraded on run 2. 48-capsule floor applies.

## Non-goals
- Not a build/spec repo — it sizes the prize and picks the target; the winning
  increment gets its own build repo afterward.
- Not a token-price model for XRD.
- Not a rewrite of the source theses — it measures them.
