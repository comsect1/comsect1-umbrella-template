# Umbrella Refactoring and Member Updates

## Umbrella-only changes

Classification, category README, `.gitmodules`, integration tooling, and
umbrella records are owned here. Use numbered `<NN>_u-<category>/` directories;
never flatten or absorb a member repository.

Replace obsolete umbrella structure directly. Do not retain old categories,
duplicate gitlinks, aliases, redirects, parallel pins, or `legacy`/`v1`/`v2`
paths to preserve an unreleased or temporary layout. Umbrella `r{n}` work
revisions are record-only and must not select structure or member snapshots.

Classify durable guidance discovered during a refactor. Template-wide umbrella
rules remain common; subtype rules belong in `.instructions/kind/`; downstream
umbrella-specific vocabulary and integration constraints belong in
`.instructions/local/`. Never copy member-local guidance into the umbrella.

## Design before umbrella edits

Before changing classification, membership, gitlinks, or integration behavior,
derive the intended umbrella state from its public purpose, local instructions,
`.gitmodules`, and committed gitlinks:

1. umbrella-owned meaning, classification invariants, and integration effects;
2. the category ownership map without inventing a global taxonomy;
3. the expected membership graph and exact member commit transitions;
4. member authority, license, publication, and dirty-worktree boundaries; and
5. umbrella structure, pin, and integration acceptance checks.

Complete and reconcile this design before editing umbrella files. A cleaner
tree, a lower Gate finding count, or a resolvable member path does not prove a
correct membership transition. Stop when the intended graph, published target
commit, or member authority cannot be established without inference.

## Member changes

1. Establish separate authority in the member repository.
2. Read its local instructions and preserve its license and history.
3. Derive the intended member change, acceptance checks, and exact published
   commit transition before implementation.
4. Complete, verify, commit, and publish the member change there.
5. Return to the umbrella and update only the reviewed gitlink and related
   umbrella records.
6. Run integration verification in an explicit external run directory.
7. Commit the gitlink transition without copying member records into the umbrella.

The member owns its official release version and compatibility decisions. The
umbrella records only the published commit it pins and must not infer or create
a member version or compatibility promise.

Never use an umbrella refactor to modify a member Cell, normalize its layout,
relicense it, or silence its Gate findings. Gate and Forge outputs are
snapshot-bound inputs to separately authorized member work.
