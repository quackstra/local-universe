# Local-Universe — Claude Code Operating Instructions

## Project Identity

This is **Local-Universe** — an autonomous research framework that sizes the
"prize" of the LoFi / Local Stack thesis on Radix and ranks which increment to
build next. Part of the Quackstra *Universe of…* ecosystem; inherits its
pipeline, souls/Bureau engine, and the MEST + TTR lenses from Universe of Finance.

Read [`BRIEF.md`](BRIEF.md) first — it defines the two deliverables, the five
lenses, the adoption tiers, and the increment-ranking rubric.

## Code Standards

- Python 3.12+, Black defaults (line length 88), type hints on public functions, pytest.
- Git prefix: `[LU]` for framework, `[LU] <venture-slug>:` for research capsules.
- Structured data as JSON (`data.json` per venture/category); charts as PNG from data.
- Reports in Markdown with hyperlinked source citations.

## Trigger Phrase

When Ferg says **"okay elves, explore the local universe"**, immediately execute
a full autonomous elf run:

1. `cd /home/quackstra/local-universe`
2. Execute Steps A–E from `elves/run_protocol.md`
3. Target 48+ capsules, inside-out priority (biggest prize first: SRU, CCS)
4. Fire-and-go — no confirmation needed.

## Pipeline

- `run.sh scout` — refresh the venture/category backlog
- `run.sh architect` — design methodology for the next pending venture
- `run.sh analyze` — execute research for the next methodology-ready venture
- `run.sh elf-run` — full autonomous elf run (Steps A–E, 48+ capsules)

## Souls / Bureau

Staff capsules via the Soul-Less Employment Bureau. Reuse Universe-of-Finance
souls directly (`--souls-dir ../universe-of-finance/souls`) **and** the net-new
LoFi roster in `souls/RECRUITER.md`. Local-Universe is registered in the Bureau
`universes/registry.yaml` as `local`.

## Rules

- Every number MUST cite a source; NEVER fabricate sources — say so if none exists.
- Every capsule MUST report a **T1/T2/T3 adoption-tier range**, not a point estimate.
- Every capsule MUST carry a confidence tag (🟢/🟡/🔴).
- Every "prize" number MUST be expressible in at least one Radix-native term (RVC).
- Distinguish **captured** vs **compressed** MEST explicitly — never conflate them.
- ALWAYS run validation gates before committing; NEVER commit secrets or API keys.
- Credentials via env injection through `run_pipeline.sh` — never a new env file.
