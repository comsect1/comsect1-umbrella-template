# Member Repository Boundary

An umbrella coordinates repositories; it does not become their authoring root.

- Discover membership only from `.gitmodules` and committed gitlinks.
- Discover Cells only from `comsect1.json` inside a member's immutable tree.
- Read the member's own `AGENTS.md` and local instructions before modifying it.
- Do not copy a Cell authoring policy into the umbrella and claim it governs all
  members. Propagate upstream policy through an explicit member-template update.
- Do not add, remove, or rewrite member `comsect1.json`, source, sidecars, or
  licenses as part of an umbrella-only classification or pin update.
- Gate may scan member Cells, but each result remains bound to the member commit
  and Cell snapshot. Store run output outside inspected members.
- Forge executes only under separately established member-local authority.
  Publish that member commit before advancing the umbrella gitlink.
