# os·tack

**the OS stack.**

One binary. Replaces your entire development tool stack. Agents run on it without knowing.

## The stack

| | What | Link |
|---|---|---|
| **ostk** | The OS — coordination, execution, filesystem | [ostk.ai](https://ostk.ai) |
| **haystack** | Coordination kernel — agents, needles, compression | [haystack](https://github.com/os-tack/haystack) |
| **find-the-needle** | Proofs of the OS stack — 23 Docker benchmarks | [needle-bench.cc](https://needle-bench.cc) |
| **claude-code** | Agent harness — Claude Code integration | [claude-code](https://github.com/os-tack/claude-code) |

## Install

```bash
curl -fsSL https://ostk.ai/install | sh
```

## Five laws

1. Write path invisible
2. Agents ephemeral
3. Coordinate through filesystem
4. Optimistic concurrency
5. Invisible infrastructure, always

## Provenance

This org is attested by four entities operating under the haystack coordination kernel:

| Entity | Role | Identity |
|--------|------|----------|
| `@haystack.prime` | Primary kernel operator | Claude Opus 4.6 |
| `@gemini.prime` | Secondary kernel operator | Gemini |
| `@scottmeyer` | Human operator, org owner | [scottmeyer](https://github.com/scottmeyer) |
| `@kernel` | Autonomous kernel process | haystack v1.3.0 |

### Attestation

All kernel operations are audited via `.haystack/audit.jsonl`. Agent identity is established through `ENTITYFILE` signatures. The coordination kernel enforces:

- **Invisible write** — file mutations are tracked with generation counters
- **Ephemeral agents** — fleet processes are reaped on session close
- **Filesystem coordination** — all state flows through the filesystem, never through agent memory
- **Optimistic concurrency** — conflicts resolve at write time via Hot PR

### Verified live

The haystack kernel has been validated under live operational load:
- Multi-agent fleet dispatch (15+ concurrent agents)
- Cross-session state persistence across context boundaries
- Mobile boot (iPhone) confirmed functional
- Production security research (HackerOne CTF) coordinated through the kernel

[Documentation](https://ostk.ai/docs) · [Insights](https://needle-bench.cc/insights) · [Leaderboard](https://needle-bench.cc/leaderboard)
