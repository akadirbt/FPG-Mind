# FPGA-Mind

> A private-first technical AI workspace for grounded assistance, durable project continuity, and real engineering flow.

`FPGA-Mind` is the public-facing name of the project.
`Gozde` is the internal assistant persona and working system identity inside the private repo.

This project is not centered on the usual "memory AI" pitch.
Its real focus is building an AI system that behaves like a disciplined engineering tool:

- continuity-aware across sessions
- explicit about when to recall, search, or stay deterministic
- useful for technical work, not just conversational demos
- modular enough to evolve without collapsing into prompt chaos

## What FPGA-Mind Actually Tries To Solve

The hard part is not storing old messages.

The hard part is building a system that can:

- carry technical context across sessions without re-explaining everything
- separate memory recall from fresh-information search
- keep grounded answers from turning into confident invention
- preserve system control as the architecture grows

In practice, that means handling flows closer to:

- continuing a KV260 debugging thread across multiple sessions
- recalling prior AXI or SystemVerilog discussion without confusing it with fresh web facts
- switching cleanly between deterministic retrieval, search-backed answers, and model-only reasoning

## Proof Points

The current private system already has concrete engineering signals behind it:

- a `70-step` adversarial memory/search/cursor/provenance gauntlet in the E2E suite
- explicit routing boundaries between memory, search, and model-only behavior
- a local Qwen-centered runtime with bounded use of external higher-tier models for narrower roles
- a modular backend/frontend structure instead of a single giant prompt wrapper

This public repo does not expose the full private implementation, but it does reflect a real working system rather than a concept page.

## Why The Name Fits

The project is shaped by an engineering mindset.

The same instincts that matter in FPGA and systems work matter here too:

- boundaries matter
- observability matters
- correctness matters
- structure beats magic

That mindset is a better description of the project than "AI that remembers."

## Core Characteristics

- private-first by design
- continuity-aware without overselling memory
- grounded over theatrical
- technical and project-oriented
- architecture-minded instead of prompt-hacked
- built as a long-running system, not a one-shot demo

## In This Public Repo

- project framing
- high-level architecture
- setup philosophy
- API response style
- privacy and security posture

The private repo, local memory data, secrets, audits, and internal planning docs stay out of this public surface.

## Public Docs

- [`docs/ARCHITECTURE.md`](./docs/ARCHITECTURE.md)
- [`docs/SETUP.md`](./docs/SETUP.md)
- [`docs/API.md`](./docs/API.md)
- [`docs/SECURITY.md`](./docs/SECURITY.md)

## Who It Is For

FPGA-Mind is for people interested in AI systems that feel closer to:

- a serious technical copilot
- a private project workspace
- a continuity-aware engineering tool

than to a generic chatbot with a memory label attached.

## Status

The main working codebase remains private.

This public repo exists to document the philosophy, architecture shape, and public-facing identity of the project without leaking the internals that make the private system work.
