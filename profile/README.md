# os-tack

Local-first infrastructure for AI agents. Public projects are AGPL-3.0 or MIT; production binaries are GPG-signed.

[ostk.ai](https://ostk.ai) · [contact@ostk.ai](mailto:contact@ostk.ai)

## Install

```
curl -fsSL https://ostk.ai/install.sh | sh
```

---

## ostk — the kernel

| Repo | What it is |
|---|---|
| [`ostk.ai`](https://github.com/os-tack/ostk.ai) | Production release mirror. Signed binaries, governance bail, prime key. |
| [`ostk-site`](https://github.com/os-tack/ostk-site) | Source for ostk.ai. Astro. |
| [`libostk`](https://github.com/os-tack/libostk) | Userspace client library for the ostk kernel. |
| [`homebrew-ostk`](https://github.com/os-tack/homebrew-ostk) | Homebrew tap. Auto-updated on release. |
| [`ostk-recall`](https://github.com/os-tack/ostk-recall) | Local-first hybrid retrieval MCP server — model2vec embeddings + LanceDB + Tantivy BM25 + SQLite. One binary; hybrid search across markdown, code, and Claude Code sessions. |
| [`ostk-cache`](https://github.com/os-tack/ostk-cache) | Context-aware caching proxy for Anthropic and OpenAI. Drop-in for Claude Code, Codex, Cursor, and custom harnesses. |
| [`osteak`](https://github.com/os-tack/osteak) | Elm-style architecture for ratatui — you bring the loop. |

## Companion tools

| Repo | What it is |
|---|---|
| [`prism`](https://github.com/os-tack/prism) | Project a canonical `.agents/` directory into every AI coding tool's config (Claude, Cursor, Gemini, Cline, Continue, Windsurf, Copilot, AGENTS.md). |
| [`docfresh`](https://github.com/os-tack/docfresh) | Track documentation freshness against source code. |

## Benchmarks

| Repo | What it is |
|---|---|
| [`find-the-needle`](https://github.com/os-tack/find-the-needle) | 23 Docker benchmarks. Submit broken Dockerfiles, watch models fix them. Leaderboard at [needle-bench.cc](https://needle-bench.cc). |

## File Context Protocol (FCP)

MCP servers that expose verb-based DSLs over complex file formats. Each driver exposes the semantic operations a format supports rather than raw file I/O.

**Frameworks**

| Repo | Language |
|---|---|
| [`fcp`](https://github.com/os-tack/fcp) | Protocol spec |
| [`fcp-core`](https://github.com/os-tack/fcp-core) | TypeScript + Python shared framework |
| [`fcp-core-rust`](https://github.com/os-tack/fcp-core-rust) | Rust shared framework |

**Drivers**

| Repo | Format |
|---|---|
| [`fcp-pdf`](https://github.com/os-tack/fcp-pdf) | PDF — read, annotate, redact, merge, split |
| [`fcp-drawio`](https://github.com/os-tack/fcp-drawio) | draw.io diagrams |
| [`fcp-midi`](https://github.com/os-tack/fcp-midi) | MIDI composition |
| [`fcp-sheets`](https://github.com/os-tack/fcp-sheets) | Spreadsheets |
| [`fcp-slides`](https://github.com/os-tack/fcp-slides) | Slide decks |
| [`fcp-terraform`](https://github.com/os-tack/fcp-terraform) | Terraform HCL |
| [`fcp-rust`](https://github.com/os-tack/fcp-rust) | Rust codebases via rust-analyzer |
| [`fcp-python`](https://github.com/os-tack/fcp-python) | Python codebases via pylsp |
| [`fcp-regex`](https://github.com/os-tack/fcp-regex) | Regex via named fragment composition |

---

[Documentation](https://ostk.ai/docs) · [contact@ostk.ai](mailto:contact@ostk.ai)
