# Comsect1 Umbrella Template Instructions

## Authority and repository boundary

- This repository classifies and pins independent member repositories. It does
  not own or absorb member implementation, history, Cell authority, or license.
- `.gitmodules` and the committed gitlinks are the sole membership authority.
- Register every member directly below one numbered category named
  `<NN>_u-<category>/`. A category is an ordinary umbrella-owned directory, not
  a repository or a Cell.
- The template standardizes that category form, not a global taxonomy. Each
  downstream umbrella owns its category vocabulary, ordering, and boundaries.
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
- Umbrella-owned text follows [the text-format policy](./.instructions/text-format-policy.md).
  The policy does not propagate through gitlinks; each member requires its own
  repository-root policy.

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

## Version and compatibility invariants

- The committed gitlink is the umbrella's member snapshot authority. Do not
  invent, mirror, rewrite, or infer a member product version from category names,
  paths, branches, work revisions, or umbrella metadata.
- Do not use `legacy`, `old`, `v1`/`v2`, `r{n}`, or similar labels to create
  parallel categories, duplicate membership, compatibility aliases, or pin
  selection logic. An `r{n}` umbrella work revision is non-semantic traceability
  only.
- Replace obsolete umbrella structure completely. Do not preserve unreleased or
  temporary umbrella layouts through aliases, redirects, shims, or parallel
  membership paths.
- Release and compatibility authority remains member-local. The umbrella may
  record a published member release but must not create or extend its contract.
- Apply the full [version and compatibility policy](./.instructions/version-and-compatibility.md)
  during umbrella and member-pin updates.

## Instruction ownership and precedence

- Root `.instructions/*.md` files supplied by this template are common umbrella
  instructions and may be updated by template synchronization.
- `.instructions/kind/` is the downstream-owned umbrella-kind layer. Record the
  umbrella subtype and durable guidance shared by that kind there.
- `.instructions/local/` is the downstream-owned repository-local layer. Put
  durable umbrella-specific classification vocabulary, integration constraints,
  and operating guidance there; template synchronization must never overwrite it.
- Member-local instructions remain inside each member and are never absorbed by
  an umbrella `local` layer. Task-only authority remains in separately owned
  work records and is not a durable instruction by default.
- Kind and local guidance may narrow or strengthen common rules but may not
  weaken common invariants or member authority.
- Apply the full [instruction layers policy](./.instructions/instruction-layers.md)
  whenever umbrella instructions are created, promoted, or synchronized.

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
- [Version and compatibility](./.instructions/version-and-compatibility.md)
- [Instruction layers](./.instructions/instruction-layers.md)
- [Umbrella-kind instructions](./.instructions/kind/README.md)
- [Umbrella-local instructions](./.instructions/local/README.md)
- [Text format policy](./.instructions/text-format-policy.md)
