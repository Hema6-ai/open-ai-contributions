# vLLM Issue #41230 - NIXL KV Connector Metrics Aggregation Semantics

Repo: vllm-project/vllm
Issue: https://github.com/vllm-project/vllm/issues/41230
Type: [Docs] Document NIXL KV connector metrics aggregation semantics
Target level: Level 4 (Improve Evaluation / Test Infrastructure) - this is an
observability/metrics-semantics doc fix, not a bug repro or a feature.

Status: NOT STARTED - do not claim the issue until assignment/open-PR state
is checked immediately before starting.

## Pre-flight checklist (do before writing anything)
- [ ] Re-check issue #41230 on GitHub right now: is it still open, still
      unassigned, no existing linked PR already covering it?
- [ ] Read CONTRIBUTING.md in vllm-project/vllm.
- [ ] Clone vllm locally (NOT inside this folder - clone elsewhere, e.g. a
      sibling `vendor/vllm` or a separate workspace dir, since this repo is
      for contribution tracking/notes, not for vendoring other projects).

## Investigation questions (answer from code, not guesses)
1. What is the NIXL KV connector?
2. What metrics does it expose?
3. Where are those metrics produced (which file/class/function)?
4. Where are they aggregated?
5. What does "aggregation" mean here exactly?
6. Are metrics per-request / per-worker / per-connector / cumulative /
   averaged / summed?
7. What happens when multiple workers/connectors contribute?
8. Difference between local metrics, aggregated metrics, and
   Prometheus-visible metrics?
9. What terminology does the code use vs what current docs say?
10. Concrete worked example of the aggregation (Worker A + Worker B ->
    aggregation -> reported metric)?

## Mental model (fill in as understood)
```
Metric
  |
  v
Where generated?
  |
  v
What object owns it?
  |
  v
Who updates it?
  |
  v
Who aggregates it?
  |
  v
What does the user finally observe (e.g. Prometheus)?
```

## Files found (fill in once cloned/grepped)
- grep results for "NIXL":
- grep results for "metric" (narrowed to KV connector area):
- metric definition file(s):
- aggregation code location(s):
- existing docs covering NIXL/KV connector/observability:

## Gap between code and docs
(What the docs are missing or get wrong, once identified - don't invent
behavior not seen in code.)

## Planned doc change (smallest useful version)
Metric name -> Meaning -> Scope -> Aggregation rule -> Example -> Interpretation

## Validation commands (fill in with the actual commands from CONTRIBUTING.md)
```bash
# doc build / lint commands go here once confirmed from the repo
```

## Open questions for review before opening PR
-
