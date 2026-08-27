# Comsect1 Umbrella Template Instructions

## Authority and repository boundary

- This repository classifies and pins independent member repositories. It does
  not own or absorb member implementation, history, Cell authority, or license.
- `.gitmodules` and the committed gitlinks are the sole membership authority.
- Register every member directly below one numbered category named
  `<NN>_u-<category>/`. A category is an ordinary umbrella-owned directory, not
  a repository or a Cell.
- Never infer a Cell from membership or category placement. A Cell exists only
  inside a member repository where a local `comsect1.json` declares it.
- Before changing member content, enter that repository and read its own
  `AGENTS.md` and local instructions. An umbrella task alone authorizes only
  umbrella files and gitlink pins.

## Umbrella-owned material

- The umbrella owns only its root governance files, instructions, category
  boundary READMEs, `.gitmodules`, and gitlink pins.
- Do not create project roots such as `10_pkg/`, `20_ops/`, `30_cert/`,
  `90_temps/`, or `99_trash/` in an umbrella.
- Do not store implementation, build output, Gate evidence, Forge journals,
  release packages, or member copies in the umbrella index.

## Member operations

- Pin only published member commits. Report dirty or uninitialized members and
  never reset, clean, move, or remove them implicitly.
- A member refactor and an umbrella pin update are separate repository changes:
  complete and publish the member change first, then update its gitlink.
- Gate may enumerate members from `.gitmodules` and inspect their locally
  declared Cells. Keep its run directory outside the umbrella and every
  inspected member repository.
- Forge authority remains member-local. An umbrella progress event or Gate
  finding never grants authority to modify a member.

## Routed instructions

- [Instruction index](./.instructions/README.md)
- [Repository boundary](./.instructions/member-repository-boundary.md)
- [Classification](./.instructions/classification.md)
- [Membership](./.instructions/membership.md)
- [Branches](./.instructions/branches.md)
- [Umbrella verification](./.instructions/verification.md)
- [Artifact placement](./.instructions/artifact-placement.md)
- [Temporary output and cleanup](./.instructions/temporary-output-and-cleanup.md)
- [Fork adoption](./.instructions/fork-adoption.md)
- [Licensing policy](./.instructions/licensing-policy.md)
- [Refactoring and updates](./.instructions/refactoring-and-updates.md)
