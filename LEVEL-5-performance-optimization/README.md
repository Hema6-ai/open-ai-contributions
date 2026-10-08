# Level 5 - Performance / Memory / Numerical Optimization

## Goal
Improve speed, memory footprint, or numerical stability/precision of an
existing, correct implementation, without changing its observable behavior
(unless the issue is explicitly about tolerance/precision).

## Bar for done
- You have a reproducible benchmark showing the before/after (latency,
  throughput, memory, or numerical error), not just "it feels faster".
- You understand why the optimization works (e.g. avoided copy, better
  cache locality, algorithmic change, fused op, reduced precision loss) -
  can explain the mechanism, not just cite the number.
- No correctness regressions: existing tests pass, and you've checked edge
  cases the optimization could plausibly break (empty input, large batch,
  dtype boundaries).
- Tradeoffs are explicit (e.g. "faster but uses more memory", "faster only
  above batch size N").

## Why this matters
This is where "I can read and improve a production ML system" starts to show.
It requires understanding both the algorithm and the hardware/runtime
constraints around it.

## Log
See CONTRIBUTIONS.md in this folder.
