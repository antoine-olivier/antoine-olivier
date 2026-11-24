# How I work

I design the questions, protocols, benchmarks, and checks; AI agents write most of the code and run the experiments under my direction. I am responsible for every published claim; no AI system is an author.

## Verification layers

Not every project uses every check; each study repository and the [research register](https://github.com/antoine-olivier/research-register) states exactly which checks ran and what remains unverified.

- **Pre-registered protocols and sealed corpora:** benchmark files and analysis rules are frozen and hashed before inference runs (any post-hoc redo is declared explicitly).
- **Exact or interval arithmetic:** mathematical bounds are verified in exact integer, exact rational, or interval arithmetic, not floating-point rounding.
- **Independent checkers and replay scripts:** a separate program (often written by another model family) or public replay script re-computes the counts and bounds from raw data.
- **Cross-vendor hostile review:** a fresh reviewer from another model family tries to break the claims, scopes, and numbers before publication.

## Where results go

- **AI safety and control:** public GitHub repositories with protocols, anonymized or synthetic sealed corpora, raw score logs, and replay scripts (`code-oversight-bench`, `underreported-refusals-pilot`, `sleight-bench-open-weights-monitor`).
- **Mathematics and reference tables:** submitted directly to reference table maintainers (Andries Brouwer's table, Henry Cohn's spherical-codes and stealth tables, OEIS, catalog maintainers) and archived on Zenodo. Every entry, including superseded bounds and negative findings, is tracked in [research-register](https://github.com/antoine-olivier/research-register).

## Tools

- **Coding agents:** Claude Code, Google Antigravity, and Codex under deterministic hook-based guards.
- **Local inference:** Ollama and PyTorch/Transformers on a consumer GPU (RTX 3070 8 GB) and Colab GPUs for open-weights monitor evaluations.
- **Cross-vendor verification:** independent model families (Claude, GPT/Codex, Gemini, DeepSeek) used across projects for blind coding, second checkers, and adversarial review (each repo states which families ran on that study).

[Back to the profile](https://github.com/antoine-olivier)
