# Level 7 - Cross-Component Architectural Contribution

## Goal
Make a change that spans multiple subsystems or changes a structural
boundary: a new abstraction used across modules, a refactor that changes how
components talk to each other, a contribution that required coordinating
with multiple maintainers/areas of the codebase.

## Bar for done
- You can draw the system boundaries before and after your change (which
  components, what crosses which boundary).
- You understand the blast radius: what else depends on the thing you
  changed, and how you verified they still work.
- The change was discussed/designed with maintainers before large code was
  written (RFC, design doc, or issue discussion), not just a surprise PR.
- You can articulate the tradeoffs of the architecture you chose vs at least
  one alternative you rejected.

## Why this matters
This is "I can be trusted with the shape of the system", not just "I can fix
things inside it". Few contributions reach here - treat every one as worth a
written retrospective.

## Log
See CONTRIBUTIONS.md in this folder.
