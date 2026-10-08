# Level 1 - Reproduce a Real ML Bug

## Goal
Take a reported bug (from an issue tracker, not one you invented) and reproduce
it reliably from source: same inputs, same environment, same failure.

## Bar for done
- You can trigger the exact reported failure (error, wrong output, crash,
  divergence) on a clean checkout.
- You know the minimal reproduction: smallest model/config/input that still
  triggers it.
- You have written down why it happens at a surface level (which call,
  which line, which condition) - not yet necessarily the full fix.
- You can tell someone else how to reproduce it in under 5 steps.

## Why this matters
Most people skip this and jump to fixing based on guesswork. Reproduction
first means every later claim about the bug is testable, not assumed.

## Log
See CONTRIBUTIONS.md in this folder.
