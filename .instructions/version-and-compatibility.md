# Umbrella Version and Compatibility Policy

This policy keeps umbrella indexing and member product authority separate.

## Snapshot and release authority

- `.gitmodules` and the committed gitlink identify umbrella membership and the
  exact integrated member snapshot.
- The member repository owns its official release version, external contracts,
  compatibility decisions, and release records.
- The umbrella may report an official member release but must not assign,
  translate, infer, or extend it.
- An umbrella work revision such as `r{n}` is non-normative traceability only.
  It must not select a category, member, branch, gitlink, or integration path.

## Prohibited umbrella versioning

Do not encode `legacy`, `old`, `v1`, `v2`, `r{n}`, dates, release waves, or
similar history labels in category names, member paths, duplicate membership,
parallel gitlinks, aliases, redirects, integration modes, or pin-selection
logic. Branch hints and category placement are not product versions.

Replace an obsolete, unreleased umbrella layout completely. Do not keep a
compatibility shim or parallel structure for temporary indexing history.
Historical membership remains available through Git and umbrella records.

If a released external integration contract genuinely requires compatibility,
its owning repository must authorize and define that contract, its consumers,
support period, verification, and retirement decision. The umbrella must not
manufacture compatibility on a member's behalf.
