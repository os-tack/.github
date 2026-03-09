# needle-bench

**Your worst debugging day, everyone's benchmark.**

Submit a broken Dockerfile. Watch models try to fix it. See who finds the needle.

## How it works

1. **You submit a PR** with a `Dockerfile` containing a real bug and a `test.sh` that fails
2. **CI runs every model** against your bug — Claude, Gemini, GPT, and more
3. **Results post to your PR** — pass/fail, turns to fix, tokens used
4. **Leaderboard updates** at [needle-bench.cc](https://needle-bench.cc)

## Why

Every benchmark is synthetic. These bugs are real. Pulled from production incidents, debugging sessions, and the worst day at work you'd rather forget.

No multiple choice. No text completion. Just: "test.sh fails. Fix it."

## Get started

→ [**Submit a benchmark**](https://github.com/needle-bench/find-the-needle/blob/main/CONTRIBUTING.md)
→ [**View the leaderboard**](https://needle-bench.cc)
→ [**Browse benchmarks**](https://github.com/needle-bench/find-the-needle/tree/main/benchmarks)
