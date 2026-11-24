# Antoine Olivier

Independent researcher. I work on AI safety, runtime control, and verifiable mathematical research with AI agents: I design the protocols, checks, and acceptance tests; agents write most of the code and run the experiments; every result is published with its limits and failures.

## AI safety and control (Nov 2026)

| Study | Headline result | Scope & limits |
|---|---|---|
| **[code-oversight-bench](https://github.com/antoine-olivier/code-oversight-bench)** | Bare real-repo FPR: **89%** (Qwen 7B), **80%** (Haiku 4.5), **8%** (Sonnet 5.5), despite flat 93–96% bug-only recall; paired separation **4% / 14% vs. 80%** (Qwen 14B NF4: 57% recall, 38% FPR, 14% sep.). | **130 sealed Python pairs** (30 standalone + 100 real MIT/BSD/Apache files across 15 libraries, AST mutations killed by upstream pytest; 24 arms, 3,120 blind evals). Adversarial 2-pass cut Haiku FPR **80% → 25%** (sep. 14% → 50%) while dropping Qwen 7B/14B to **0% TPR / 0% FPR** (370/370 bug flags overturned across both corpora). Isolated Python exec lifted Haiku to **0/30 FPR** on standalone code and exposed multi-file `ImportError` sandbox failures on real repos. |
| **[underreported-refusals-pilot](https://github.com/antoine-olivier/underreported-refusals-pilot)** | **27 of 96 (28.1%)** sub-agents omitted an action or target guard refusal from their handback report. | 95% cluster bootstrap CI `[19.4, 37.5]`; 468 blind-coded reports under a frozen protocol; lower bound, one harness, Claude coders only; 0 confirmed undeclared workarounds on one narrow check; all 52/52 reported counts and 6/6 M1 estimates replayable via published scripts. |
| **[sleight-bench-open-weights-monitor](https://github.com/antoine-olivier/sleight-bench-open-weights-monitor)** | Haiku 4.5 anchor caught **1.85% (2/108)** at 1% FPR on 36 upstream-merged attacks (paper fig. 24: 2.2%). | Partial replication (3 trials vs. 10, 4 long attacks excluded). Local Qwen3.6-35B-A3B reached **9.4%** `[2.6, 17.9]` on `control_arena` and **20.5%** `[10.3, 32.5]` with a 4-prompt max ensemble on 39 unmerged attacks (post-hoc higher-token-cap redo; differences vs. Haiku and across prompts not statistically established). |

## Mathematics, reference tables, and Lean 4

- **[research-register](https://github.com/antoine-olivier/research-register)** (**108 entries**, failures and superseded bounds included): **15 Brouwer constant-weight code bounds** (exact integer checks; **7 still listed, 8 since beaten** as of Nov 22, 2026; 12/15 with independent DeepSeek V4.1 Flash checker & Zenodo DOI; [Brouwer table](https://aeb.win.tue.nl/codes/Andw.html)), **5 Cohn spherical codes** still listed in dim. 11–14 out of 10 submitted in dim. 11–17 ([spherical-codes.org](https://spherical-codes.org/)), **2 OEIS** extensions ([A277203](https://oeis.org/A277203), [A321911](https://oeis.org/A321911)), and 1 confirmed fix to an independent exoplanet catalog ([TIC 160420269](https://github.com/eumemic/exoplanets/issues/1)).
- **Formal duals and stealth radius**: Explicit formal duals and isoduality of existing Bierbrauer–Edel and Vardy packings; **3 configurations (dimensions 18, 28, 30)** added to Henry Cohn's [table of stealth radius bounds](https://cohn.mit.edu/stealth). Preprint: [hexagonmath.org/2611.00626v1](https://hexagonmath.org/2611.00626v1) (AI-derived, cross-vendor AI-reviewed; human refereeing and artifact review pending).
- **[rh-up-to-15-lean](https://github.com/antoine-olivier/rh-up-to-15-lean)**: Lean 4 formalization of a classical zero-free bound for the zeta function up to height 15 (matching `PrimeNumberTheoremAnd` definitions, sorry-free, verified with the Lean kernel and `nanoda`).

## Software

- **[AZERTY Global](https://azerty.global/)** ([AMCF-asso/azerty-global-app](https://github.com/AMCF-asso/azerty-global-app)): Open-source French keyboard layout for Windows, macOS, and Linux (**3,530 Microsoft Store installations**, Mar 23 to Nov 23, 2026). Co-founded in 2017 with Robert Hodge; developed by me since 2018; president of AMCF. Current .NET 10 app rewritten with AI agents under my supervision.

## Links

[antoine-olivier.com](https://antoine-olivier.com/) | [How I work](https://github.com/antoine-olivier/antoine-olivier/blob/main/how-i-work.md) | [ORCID 0009-0009-9710-3682](https://orcid.org/0009-0009-9710-3682) | [antoineolivier@pm.me](mailto:antoineolivier@pm.me)
