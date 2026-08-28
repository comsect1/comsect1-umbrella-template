# Umbrella Fork Adoption

1. Replace template identity in `README.md` and `AGENTS.md`.
2. Record the Comsect1 upstream URL and exact baseline commit.
3. Select the downstream umbrella license without relicensing the retained
   Comsect1 scaffold or any member repository.
4. Replace the subtype placeholder in `.instructions/kind/README.md` and record
   why that umbrella-kind classification applies.
5. Put durable downstream-specific classification vocabulary, integration
   constraints, and operating guidance in `.instructions/local/`, with every
   file indexed from `.instructions/local/README.md`.
6. Create the required numbered `<NN>_u-<category>/` directories and give each
   a boundary `README.md`; do not retain a generic member placeholder.
7. Add `.gitmodules` with the first member. Do not create another membership
   manifest.
8. Confirm no unit-repository scaffold was introduced at the umbrella root.
9. Confirm every member retains independent history, instructions, Cell
   authority, license, and notice.
10. Retain the root `.gitattributes` and `.editorconfig`, configure umbrella
   generators for LF, and run `.instructions/text-format.ps1 -Apply` once
   before the first publication.
11. Confirm template synchronization updates common files while preserving
    `.instructions/kind/`, `.instructions/local/`, and every member repository.
