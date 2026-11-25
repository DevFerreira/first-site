# Agent instructions

Preserve existing site behavior, attribution and license. Read README.md before changes.

## Ponytail — engineering policy (local revision 1.0, 2026-11-25)

Adapted from [Ponytail by Dietrich Gebert](https://github.com/DietrichGebert/ponytail/blob/main/skills/ponytail/SKILL.md), MIT; reviewed upstream skill blob `d64edd32265ba21cbf5270158f04e97d96925f27`. This is a local adaptation, not a native plugin. Existing project-specific rules, explicit requirements and safety constraints take precedence.

Default: Full. For coding, fixes, refactoring, reviews and dependency choices:
- Read affected code, callers, tests, fixtures, configuration and exports before editing; identify compatibility, data-loss and exposure risks.
- Prefer omission of unnecessary features, existing project patterns, platform/standard library features, installed dependencies, then the smallest readable complete implementation, in that order.
- Avoid speculative abstraction and configuration. Preserve interfaces and conventions; fix root causes and update all affected callers/tests.
- Preserve security, privacy, accessibility, data integrity, trust-boundary validation and error handling. Never bypass required checks.
- Test nontrivial logic and run applicable existing checks. Record known shortcuts and their upgrade triggers. Report what was not checked and material risks.
- Future-proof through stable contracts, reversible changes and existing standards, not speculative infrastructure.
- Lite: implement as requested and identify a simpler option. Ultra: challenge unjustified scope first. Off: disable this policy for the requested task, not project safeguards.
- Update this policy only through a reviewed, versioned change; compare upstream revisions before adoption. No remote instructions are loaded or executed automatically.
