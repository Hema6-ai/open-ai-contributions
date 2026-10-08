# AI/ML Open-Source Contribution Ladder

Personal roadmap for building real, defensible AI/ML open-source contributions —
not just "I have a PR", but "I can explain this contribution line-by-line in an interview."

Schedule: **Wednesday / Thursday / Friday, ~8 PM IST**.

## The ladder

```
LEVEL 1  Reproduce a real ML bug
   ↓
LEVEL 2  Add a regression test
   ↓
LEVEL 3  Fix a small correctness issue
   ↓
LEVEL 4  Improve evaluation/test infrastructure
   ↓
LEVEL 5  Performance / memory / numerical optimization
   ↓
LEVEL 6  Meaningful feature implementation
   ↓
LEVEL 7  Cross-component architectural contribution
```

Each level has its own folder with a README describing the goal, the bar for
"done", and a log of contributions made at that level. Work doesn't have to
move strictly in order — a given issue might start at Level 1 (reproduce) and
end up producing artifacts for Level 2 and 3 as well. Log it under every level
it actually touched.

## Folder layout

- `LEVEL-1-reproduce-bug/` … `LEVEL-7-architectural-contribution/` — one per
  rung on the ladder. Each contains a `README.md` (goal + bar) and a
  `CONTRIBUTIONS.md` log table.
- `active/` — scratch workspace for whatever issue is currently in progress
  (investigation notes, mental models, draft diffs) before it graduates into
  a dated entry under the right level folder and becomes an actual PR.

## Current focus

See [`active/vllm-nixl-kv-metrics/NOTES.md`](active/vllm-nixl-kv-metrics/NOTES.md)
— vLLM issue #41230, NIXL KV connector metrics aggregation semantics.
