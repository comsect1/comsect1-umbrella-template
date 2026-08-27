# Membership

- `.gitmodules` is the sole path, remote, and branch authority after the first
  member exists; the gitlink pins the reviewed commit.
- Each member is a gitlink directly below one `<NN>_u-<category>/` directory.
- Each category has a boundary `README.md` and is never itself a submodule.
- Verify a new pin exists at its declared remote before publication.
- Report dirty or uninitialized members; never reset or clean them implicitly.
- Membership never authorizes member migration, Cell changes, or relicensing.
