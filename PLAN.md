# Repository Improvement Plan

Date: 2026-08-26

## Goal

Turn this certification-practice repository into a cleaner technical learning record while preserving the original lab artifacts and course structure.

## Audit findings

- The README is currently very short despite the repository containing exercises from multiple courses/labs.
- There is no CI that validates the Python lab files.
- The only workflow is an hourly stale-PR workflow using an outdated moving `actions/stale@v4` reference; hourly stale processing is unnecessary for a small learning repository.
- Original course artifacts should remain recognizable and should not be refactored just to satisfy style preferences.

## Atomic commit plan

1. Document the audit.
2. Add lightweight Python compile/smoke CI with immutable action pins.
3. Modernize and reduce the stale-PR schedule with least privileges.
4. Expand the README into a useful course/lab index and clarify provenance.

## Validation

- Compile all tracked `.py` files without executing lab network/system behavior.
- Keep original lab inputs and service files untouched.
- CI must require only read permissions; stale automation receives only pull-request/issues write permissions it needs.

## Risk / rollback

Low. Application/lab behavior will not be changed. CI and documentation commits can be reverted independently.
