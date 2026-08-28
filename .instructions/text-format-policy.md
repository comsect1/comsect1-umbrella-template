# Umbrella Text Format Policy

- Root `.gitattributes` is authoritative for umbrella-owned working-tree
  bytes. Umbrella-authored and generated text uses UTF-8, LF, and a final
  newline; true binary artifacts remain `-text`.
- `.editorconfig` aligns supporting editors. Any generator added by a
  downstream umbrella must emit LF.
- This policy governs only the umbrella repository. It does not cross a
  gitlink, alter a member worktree, or replace a member's own root policy.

Read-only verification:

```powershell
pwsh -File .instructions/text-format.ps1
```

Explicit automatic correction:

```powershell
pwsh -File .instructions/text-format.ps1 -Apply
```

Correction is limited to tracked LF-policy text, is not staged, and never
touches `-text` files or member content.
