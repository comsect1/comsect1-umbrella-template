# Umbrella Verification

For every umbrella change:

1. Confirm the root contains no unit-repository scaffold directories.
2. Confirm every `<NN>_u-<category>/` has a boundary `README.md`.
3. Confirm every gitlink path, URL, and branch agrees with `.gitmodules`.
4. Confirm no category directory is itself a submodule.
5. Confirm each new pin exists at its declared remote.
6. Report dirty and uninitialized members without changing them.
7. Confirm all local instruction links resolve.
8. Confirm no umbrella-only change modified member content or licensing.
9. Run `.instructions/text-format.ps1` and require a canonical UTF-8/LF
   umbrella worktree before publication.

This assesses the umbrella index. It is not a Gate run and cannot aggregate or
reinterpret member Cell verdicts.
