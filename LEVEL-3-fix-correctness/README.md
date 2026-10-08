# Level 3 - Fix a Small Correctness Issue

## Goal
Fix a well-scoped correctness bug: wrong output, off-by-one, incorrect edge
case handling, wrong default, misleading docs that cause wrong usage.

## Bar for done
- Root cause identified and stated in plain language (not just "changed line
  X to Y").
- Fix is minimal - no drive-by refactors bundled in.
- Regression test from Level 2 (or a new one) passes.
- You can explain why the old behavior was wrong and why the new behavior
  is correct, including any edge cases the fix does or doesn't cover.

## Why this matters
This is usually the first PR that actually merges. The discipline here is
scope control: fix the bug, not everything near it.

## Log
See CONTRIBUTIONS.md in this folder.
