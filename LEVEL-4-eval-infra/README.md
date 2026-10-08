# Level 4 - Improve Evaluation / Test Infrastructure

## Goal
Improve how correctness or performance is measured for an ML system:
eval harnesses, benchmark scripts, CI test infra, metrics/observability
definitions and documentation (e.g. clarifying aggregation semantics),
flaky-test fixes, test speed/isolation improvements.

## Bar for done
- You understand what the infra currently measures and where that's defined
  in code (not just in docs).
- Your change makes the measurement more correct, more precise, or more
  understandable - and you can show the before/after.
- If it's a docs change about behavior (e.g. metric semantics), you traced
  the actual implementation (where produced, where aggregated, where
  surfaced) before writing a word, and you can produce a concrete example
  (e.g. "Worker A + Worker B -> aggregation -> reported value").
- Passes the project's own validation steps (doc build, linters, relevant
  tests) using their documented commands, not guessed ones.

## Why this matters
Bad eval/observability infra lets real bugs hide. Understanding it deeply
(rather than editing prose) is what turns a "docs PR" into something you can
actually defend in an interview.

## Log
See CONTRIBUTIONS.md in this folder.
