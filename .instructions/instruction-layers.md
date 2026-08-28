# Umbrella Instruction Layers and Precedence

Every durable umbrella instruction must have one declared ownership layer. The
classification protects downstream umbrella knowledge without absorbing member
authority.

## Layers

1. **Common umbrella** — Root `.instructions/*.md` files supplied by this
   template. They define invariants shared by umbrella repositories and are
   template-managed.
2. **Umbrella kind** — `.instructions/kind/`. The downstream umbrella owns its
   subtype classification and durable guidance shared by that kind of umbrella.
3. **Umbrella local** — `.instructions/local/`. The downstream umbrella owns
   durable repository-specific classification vocabulary, integration
   constraints, and operating rules.
4. **Member local** — Instructions inside each independent member repository.
   The umbrella may route to them but cannot copy, override, or absorb them.
5. **Task-scoped** — Separately authorized work records. They govern a bounded
   operation and do not become durable umbrella policy without review.

The template fixes the repository class as an umbrella index but does not impose
a global subtype or category taxonomy. A downstream umbrella must declare its
own subtype and rationale.

## Precedence and conflict

- Governing contracts, licenses, and member-local authority retain their own
  boundaries.
- Kind and local layers may narrow or strengthen common umbrella instructions
  but may not weaken them or expand umbrella authority into a member.
- Task records do not override durable instructions merely because they are
  newer.
- Resolve conflicts by changing the owning layer through an authorized decision,
  never by duplication, file order, or an umbrella copy of member guidance.

## Template synchronization boundary

Template synchronization may update common files and common routing in
`AGENTS.md`. It must never overwrite, delete, reset, or silently reclassify
`.instructions/kind/`, `.instructions/local/`, category-local boundaries, or
member repository instructions. Report conflicts for explicit review.
