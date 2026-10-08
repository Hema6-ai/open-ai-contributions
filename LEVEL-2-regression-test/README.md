# Level 2 - Add a Regression Test

## Goal
Given a reproduced bug (Level 1) or an existing gap in coverage, write a test
that fails before the fix and passes after it.

## Bar for done
- Test fails on main for the right reason (not flaky, not failing on an
  unrelated assertion).
- Test is minimal - tests one behavior, not a bundle of unrelated things.
- Test follows the project's existing test conventions (fixtures, naming,
  markers/tags).
- Test would catch a future regression of the same bug.

## Why this matters
A fix without a regression test is a fix that can silently come back. This is
also usually the fastest way to prove you understood the bug, before writing
the actual fix.

## Log
See CONTRIBUTIONS.md in this folder.
