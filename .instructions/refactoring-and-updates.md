# Umbrella Refactoring and Member Updates

## Umbrella-only changes

Classification, category README, `.gitmodules`, integration tooling, and
umbrella records are owned here. Use numbered `<NN>_u-<category>/` directories;
never flatten or absorb a member repository.

Replace obsolete umbrella structure directly. Do not retain old categories,
duplicate gitlinks, aliases, redirects, parallel pins, or `legacy`/`v1`/`v2`
paths to preserve an unreleased or temporary layout. Umbrella `r{n}` work
revisions are record-only and must not select structure or member snapshots.

## Member changes

1. Establish separate authority in the member repository.
2. Read its local instructions and preserve its license and history.
3. Complete, verify, commit, and publish the member change there.
4. Return to the umbrella and update only the reviewed gitlink and related
   umbrella records.
5. Run integration verification in an explicit external run directory.
6. Commit the gitlink transition without copying member records into the umbrella.

The member owns its official release version and compatibility decisions. The
umbrella records only the published commit it pins and must not infer or create
a member version or compatibility promise.

Never use an umbrella refactor to modify a member Cell, normalize its layout,
relicense it, or silence its Gate findings. Gate and Forge outputs are
snapshot-bound inputs to separately authorized member work.
