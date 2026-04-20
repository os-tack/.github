# ostk.ai

**the invisible os** — one binary that replaces your development tool stack. agents run on it without knowing.

[ostk.ai](https://ostk.ai) · [needle-bench.cc](https://needle-bench.cc) · [contact@ostk.ai](mailto:contact@ostk.ai)

## Install

    curl -fsSL https://ostk.ai/install | sh

---

## The stack

### OS

| Project | What it is | |
|---|---|---|
| **ostk** | The OS — one binary, coordination + execution + filesystem | [ostk.ai](https://ostk.ai) · [repo](https://github.com/os-tack/ostk.ai) |
| **osteak** | Elm-style architecture for ratatui — you bring the loop | [repo](https://github.com/os-tack/osteak) |
| **ostk-recall| Local-first cross-corpus - model2vec + LanceDB + DuckDB. One binary; hybrid search over markdown, code, Claude Code sessions, and more. | [repo](https://github.com/os-tack/ostk-recall)

### Benchmarks

| Project | What it is | |
|---|---|---|
| **find-the-needle** | 23 Docker benchmarks — submit broken Dockerfiles, watch models fix them | [needle-bench.cc](https://needle-bench.cc) · [repo](https://github.com/os-tack/find-the-needle) |

[Leaderboard](https://needle-bench.cc/) · [Insights](https://needle-bench.cc/insights/) · [Difficulty tiers](https://needle-bench.cc/insights/difficulty-tiers/)

### File Context Protocol (FCP)

MCP servers that let LLMs interact with complex file formats through verb-based DSLs. Instead of raw file I/O, each driver exposes the semantic operations that format actually supports.

**Frameworks**

- [`fcp`](https://github.com/os-tack/fcp) — the protocol
- [`fcp-core`](https://github.com/os-tack/fcp-core) — TypeScript + Python shared framework
- [`fcp-core-rust`](https://github.com/os-tack/fcp-core-rust) — Rust shared framework

**Drivers**

| Driver | Format |
|---|---|
| [`fcp-pdf`](https://github.com/os-tack/fcp-pdf) | PDF — read, annotate, redact, merge, split |
| [`fcp-drawio`](https://github.com/os-tack/fcp-drawio) | draw.io diagrams |
| [`fcp-midi`](https://github.com/os-tack/fcp-midi) | MIDI composition |
| [`fcp-sheets`](https://github.com/os-tack/fcp-sheets) | Spreadsheets |
| [`fcp-slides`](https://github.com/os-tack/fcp-slides) | Slide decks |
| [`fcp-terraform`](https://github.com/os-tack/fcp-terraform) | Terraform HCL |
| [`fcp-rust`](https://github.com/os-tack/fcp-rust) | Rust codebases (rust-analyzer) |
| [`fcp-python`](https://github.com/os-tack/fcp-python) | Python codebases (pylsp) |
| [`fcp-regex`](https://github.com/os-tack/fcp-regex) | Regex via named fragment composition |

---

## Five laws

1. **Invisible write** — file mutations are tracked with generation counters
2. **Ephemeral agents** — fleet processes are reaped on session close
3. **Filesystem coordination** — all state flows through the filesystem, never through agent memory
4. **Optimistic concurrency** — conflicts resolve at write time via Hot PR
5. **Invisible infrastructure** — always

---

## Provenance

This org is attested by entities operating under the haystack coordination kernel:

| Entity | Role | Identity |
|---|---|---|
| `@scottmeyer` | Human operator, org owner | [scottmeyer](https://github.com/scottmeyer) |
| `@haystack.prime` | Primary kernel operator | Claude Opus 4.6 |
| `@gemini.prime` | Secondary kernel operator | Gemini |
| `@kernel` | Autonomous kernel process | haystack v2.4.0 |

All kernel operations are audited via `.ostk/journal.jsonl`. Agent identity is established through `ENTITYFILE` signatures.

**Verified live**

- Multi-agent fleet dispatch (50+ concurrent agents)
- Cross-session state persistence across context boundaries
- Mobile boot (iPhone) confirmed functional

---

[Documentation](https://ostk.ai/docs) · [Insights](https://needle-bench.cc/insights/) · [contact@ostk.ai](mailto:contact@ostk.ai)
