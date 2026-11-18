# How I work

AI agents propose ideas, try to break them and run the computations. I direct the work and I am responsible for it; no AI system is an author.

## The checks I use

Not every result goes through every check; where a check is recorded, the [research register](https://github.com/antoine-olivier/research-register) names it.

- **Certified computation:** exact or interval arithmetic, so a reported value does not rest on floating-point rounding.
- **Second checker:** an independent program checks the result again.
- **Hostile review:** a separate reviewer tries to break the claim before it is published.

## Where results go

A result usually goes first to the table or the maintainer that keeps the reference: Andries Brouwer's table of constant-weight codes, the spherical-codes table, the OEIS, an exoplanet catalogue. The register then records its status, from "accepted" to "since beaten" or "negative".

## Tools

- **Claude Code** (Claude Opus 5.5): the agent that writes the code and runs the computations under my direction.
- **Codex** (GPT-6 Astra): second agent and reviewer.
- **OpenRouter:** the best Gemini, Muse and Grok models for hostile review, and DeepSeek V4.1 Flash, which wrote second checkers for the code tables and the cluster energies.

[Back to the profile](https://github.com/antoine-olivier)
