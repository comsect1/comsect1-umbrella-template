# Umbrella Refactoring and Member Updates

## Umbrella-only changes

Classification, category README, `.gitmodules`, integration tooling, and
umbrella records are owned here. Use numbered `<NN>_u-<category>/` directories;
never flatten or absorb a member repository.

## Member changes

1. Establish separate authority in the member repository.
2. Read its local instructions and preserve its license and history.
3. Complete, verify, commit, and publish the member change there.
4. Return to the umbrella and update only the reviewed gitlink and related
   umbrella records.
5. Run integration verification in an explicit external run directory.
6. Commit the gitlink transition without copying member records into the umbrella.

Never use an umbrella refactor to modify a member Cell, normalize its layout,
relicense it, or silence its Gate findings. Gate and Forge outputs are
snapshot-bound inputs to separately authorized member work.
